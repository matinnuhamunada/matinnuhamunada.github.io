---
title: 'Setting up Jupyter using Conda in WSL2'
date: 2021-04-04
permalink: /posts/2021/04/blog-post-1/
tags:
  - Conda
  - Jupyter
---

Hi, in this post I would like to share about my working environment (Windows with WSL2) and daily routine using Jupyter with conda and also setting those environment in remote server. 

# Set Up Local Environment 
## Install WSL2 with Ubuntu
I'm used to using Windows PC (not a fan of mac), and that's what I got from the center. Unfortunately, it is just not possible to do bionformatics with Windows (horrible experience with dual boot and Linux VM). No worries there, WSL2 has been available for those of us who doesn't want to part with Windows but would like to learn/develop using Linux.

So far I don't have many problem using WSL2 with Ubuntu-20.04 and have been using it for my daily routine. You can find WSL2 docs here: https://docs.microsoft.com/en-us/windows/wsl/install-win10 and there are many blogs out there describing how to install it in your PC.

## Install conda
I don't know what people say, but to me conda is a nice tool to manage Python and other packages for bioinformatics. 

After finishing your WSL2 and Ubuntu installation, run the ubuntu terminal and install Anaconda (or miniconda) following the docs here: https://docs.anaconda.com/anaconda/install/

## Create env with Jupyter Lab
Always work in separate environment! You don't want to go into the nigthmare of figuring out conflicted packages, so run your projects in different environment. Learn more about conda environment here: https://docs.conda.io/projects/conda/en/4.6.1/user-guide/tasks/manage-environments.html

There are many IDEs out there to try, but what I find quite easy as a beginner is using Jupyter Lab. So, start by creating your project environment and install Jupyter Lab following this docs: https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html

## Run Jupyter lab
Run Jupyter Lab by typing:
'''sh
conda activate [your environment name]
jupyter lab
'''

You might get something like this:
'''sh
http://localhost:8888/?token=6e62a781727536b7621e031c97924753fcd483fc0f06aaa0
'''

Copy paste the link to your favorite browser (honestly, don't use google chrome). You can also type localhost:8888 (or whichever port was chosen) in the browser, but it might ask you for the token (which is the characters after ?token=)

# Set Up Jupyter Server for remote working
## Access the server using SSH from WSL2
Sometimes (and more frequently) I need extra computational power to crunch those data (RAM), or running intensive algorithms (CPU/GPU). Fortunately, I have access to a workstation in the office with nice spec. You can also set up a cloud server in AWS, google cloud, microsoft azure, or other available platform out there. 

You can access this remote server (which often run in Ubuntu/Linux) by using SSH. You will need the IP address and your account (and maybe password or key). In my case, I need a VPN connection to use SSH.

You can do this by running WSL2, and typing something like this:

```sh
ssh myaccount@12.34.5.67
```

You need to change it with your [user account]@[IP Address] of course.

## Create env with Jupyter Lab
If your remote server runs on ubuntu/linux, then you can start by setting up a conda environment and installing Jupyter Lab.

## tmux for parallel access
As I want to leave the server running, and don't want to make the jupyter server terminate when losing connection, I use tmux, which will run a session in the server background (more like parallel session) even when you close my ssh session. 

The command is:

```sh
tmux
```

## Run jupyter server with tunnel
Activate your environment, and run Jupyter lab:

```sh
conda activate [your environment]
jupyter lab --no-browser --port 8889  
```

Here, we run jupyter lab server without browser in port 8889. We can change the port as we like, but make sure it doesn't conflict with other already existing port. As we run it using tmux in a parallel session, we can close our ssh connection without terminating our server. 

PS: "take note of the jupyter token, or maybe set up a password"

## SSH tunnel
To access our remote Jupyter server, we can initiate SSH session with specific port (which is our remote server port):

```sh
ssh -N -L 8889:localhost:8889 myaccount@12.34.5.67  
```

Then, we can access Jupyter in our browser by accessing Localhost:8889 (use the same port of our server)

# Something else to try
Jupyter is nice, but it might not be the best code editors out there. I've been trying (atom hydrogen)[https://atom.io/packages/hydrogen] but to no success integrating with WSL2. Right now I'm trying out [Microsoft Visual Studio Code](https://code.visualstudio.com/) which works really nicely with WSL2.
