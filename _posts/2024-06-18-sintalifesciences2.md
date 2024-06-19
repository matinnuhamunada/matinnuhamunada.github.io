---
title: 'Memetakan Peneliti Life Sciences di Indonesia Part 2'
date: 2024-06-18
permalink: /posts/2024/06/sintalifesciences2
tags:
  - Indonesia
  - SINTA
  - Dosen
---

| ![SINTA](https://sinta.kemdikbud.go.id/public/assets/img/brand_sinta.png) |
|:--:| 
| [SINTA - Database peneliti dan dosen Indonesia](https://sinta.kemdikbud.go.id/)

### Klasifikasi Rumpun Ilmu Kemendikbud dan Peta Ilmu Hayati Indonesia

<div class="container">
  <iframe src="https://htmlpreview.github.io/?https://github.com/lab-biotek-bio-ugm/rumpun_ilmu_kemdikbud/blob/main/figures/3_sunburst_chart_bio_INDONESIA.html"
      sandbox="allow-same-origin allow-scripts"
      width="100%"
      height="600"
      scrolling="yes"
      seamless="seamless"
      frameborder="2">
  </iframe>
</div>

> Sunburst chart untuk ilmu hayati dan kesehatan [revisi 5 Juni 2024](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/article_attachments/33394150376985). File tabel (`.tsv`) dapat diunduh di [sini](https://github.com/lab-biotek-bio-ugm/rumpun_ilmu_kemdikbud/blob/main/data/processed/Daftar_Rumpun_Pohon_dan_Cabang_Ilmu_(Diperbarui_05_Juni_2024).tsv). *Source code* dapat diakses di GitHub [**lab-biotek-bio-ugm**](https://github.com/lab-biotek-bio-ugm/rumpun_ilmu_kemdikbud).

### Menentukan Jumlah Klaster Keilmuan?
<div class="container">
  <iframe src="/files/01_clusterplot_publication_titles_ALL.html"
      sandbox="allow-same-origin allow-scripts"
      width="100%"
      height="280"
      scrolling="yes"
      seamless="seamless"
      frameborder="1">
  </iframe>
</div>

> Estimasi jumlah kluster keilmuan dengan berbagai metriks.

### Peta Peneliti Life Sciences di Indonesia
<div class="container">
  <iframe src="/files/01_PCA_publication_titles_ALL.html"
      sandbox="allow-same-origin allow-scripts"
      width="100%"
      height="620"
      scrolling="yes"
      seamless="seamless"
      frameborder="1">
  </iframe>
</div>

> PCA dari ekstraksi _word feature_ berdasarkan judul publikasi dosen di Google Scholar.

<a href="/files/co-author_subgraph_network_all.graphml.png" data-title="Jejaring co-authorship dosen">
    <img src="/files/co-author_subgraph_network_all.graphml.png" alt="Jejaring co-authorship dosen">
</a>

> Jejaring co-authorship dosen life science dari lima Universitas di Indonesia. Hanya co-author yang terhubung dengan lebih dari satu main author (dosen) ditunjukkan pada ilustrasi. Legend:
![#E41A1C](https://placehold.co/15x15/E41A1C/E41A1C.png) `IPB`
![#377EB8](https://placehold.co/15x15/377EB8/377EB8.png) `ITB`
![#4DAF4A](https://placehold.co/15x15/4DAF4A/4DAF4A.png) `UB`
![#984EA3](https://placehold.co/15x15/984EA3/984EA3.png) `UGM`
![#41A1C](https://placehold.co/15x15/FF7F00/FF7F00.png) `UI`
