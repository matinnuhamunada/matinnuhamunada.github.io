---
title: 'Trying out Ppanggolin'
date: 2021-04-21
permalink: /posts/2012/08/blog-post-4/
tags:
  - Conda
---

! [ppanggollin](https://storage.googleapis.com/plos-corpus-prod/10.1371/journal.pcbi.1007732/2/pcbi.1007732.g001.PNG_L?X-Goog-Algorithm=GOOG4-RSA-SHA256&X-Goog-Credential=wombat-sa%40plos-prod.iam.gserviceaccount.com%2F20210414%2Fauto%2Fstorage%2Fgoog4_request&X-Goog-Date=20210414T124020Z&X-Goog-Expires=3600&X-Goog-SignedHeaders=host&X-Goog-Signature=057a5095c990bfad0e6b711b354be6733859b1a659acb26db4dbc200fef3f19485f97146a5d669b3570bcbe40d43858ed8f4f05e5cbf044c0e255f07b0fe575dfdc4dd504b74267e18c98c5acac596614ce0475b020f885956fcb4886b1bfb02f30b2f2b1d909ca3e839d62a03f2e29ecbfe55e7b10b4d825ffe9b9c88a1304a2c5b66fe6343d7955d38b9030a432d3cbd0070d6b71068f44c271a2f70c8a4480f16e5718f1b13ce626156b1700171b7de8a135ac2fe7bc02e28a21b7a3ddc608e2e7e664d45c025e885edc8d220d47b85d734f8d0e3d5614b330aea2a162675d91ba2c351eff27f3ace8e66c33c1ef9ec2532a9bebf7af67b9513aec7fe920a)

Hi, came across these tools that utilises graph assembly to visualize pangenomes.

I was having a problem installation following their [installation guides](https://github.com/labgem/PPanGGOLiN/wiki/Installation). 

It seems to get trouble with dependencies, so I try out [this](https://github.com/labgem/PPanGGOLiN/issues/60) and it worked!

```sh
mamba create -n ppanggolin_env python=3.7
mamba install -n ppanggolin_env -c bioconda -c conda-forge -c r ppanggolin=1.1.136
```
