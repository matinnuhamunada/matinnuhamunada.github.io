---
title: 'Trying out Ppanggolin'
date: 2021-04-04
permalink: /posts/2012/08/blog-post-4/
tags:
  - Conda
---

### Trying out Ppanggolin
Problem installation https://github.com/labgem/PPanGGOLiN/wiki/Installation. Having trouble with dependencies, tryout this:
https://github.com/labgem/PPanGGOLiN/issues/60

```sh
mamba create -n ppanggolin_env python=3.7
mamba install -n ppanggolin_env -c bioconda -c conda-forge -c r ppanggolin=1.1.136
```
