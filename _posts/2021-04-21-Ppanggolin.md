---
title: 'Trying out Ppanggolin'
date: 2021-04-21
permalink: /posts/2012/08/blog-post-4/
tags:
  - Conda
---

![ppanggollin](https://github.com/labgem/PPanGGOLiN/blob/master/images/logo.png)

Hi, came across these tools that utilises graph assembly to visualize pangenomes.

I was having a problem installation following their [installation guides](https://github.com/labgem/PPanGGOLiN/wiki/Installation). 

It seems to get trouble with dependencies, so I try out [this](https://github.com/labgem/PPanGGOLiN/issues/60) and it worked!

```sh
mamba create -n ppanggolin_env python=3.7
mamba install -n ppanggolin_env -c bioconda -c conda-forge -c r ppanggolin=1.1.136
```
