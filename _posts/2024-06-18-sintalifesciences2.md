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

## Klasifikasi Rumpun Ilmu Kemendikbud dan Peta Ilmu Hayati Indonesia
Di [postingan sebelumnya](https://matinnuhamunada.github.io/posts/2024/06/rumpunilmu), saya mengulik tentang pengalaman pribadi saya di UGM terkait dengan pemilihan rumpun ilmu Dosen berdasarkan kriteria yang ditentukan oleh Kemendikbud. Tentu saja, penyematan label bidang ilmu pada tiap dosen akan mempermudah birokrasi untuk mencari ahli yang dibutuhkan dengan mudah. Meskipun demikian, klasifikasi yang ada cukup rumit dan kadang _overlap_, terutama bagi dosen yang bergiat pada ranah interdisipliner.

<div class="container">
  <iframe src="https://htmlpreview.github.io/?https://github.com/lab-biotek-bio-ugm/rumpun_ilmu_kemdikbud/blob/main/figures/3_sunburst_chart_bio_INDONESIA.html"
      sandbox="allow-same-origin allow-scripts"
      width="100%"
      height="600"
      scrolling="yes"
      seamless="seamless"
      frameborder="2">
  </iframe>
<figcaption style="text-align: center;">Sunburst chart untuk ilmu hayati dan kesehatan <a href="https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/article_attachments/33394150376985">revisi 5 Juni 2024</a>. File tabel (`.tsv`) dapat diunduh di <a href="https://github.com/lab-biotek-bio-ugm/rumpun_ilmu_kemdikbud/blob/main/data/processed/Daftar_Rumpun_Pohon_dan_Cabang_Ilmu_(Diperbarui_05_Juni_2024).tsv">sini</a>. <i>Source code</i> dapat diakses di GitHub <a href="https://github.com/lab-biotek-bio-ugm/rumpun_ilmu_kemdikbud"><b>lab-biotek-bio-ugm</b></a>.</figcaption>
</div>

## Peta Peneliti Life Sciences di Indonesia
Disini saya akan mencoba mengaplikasikan analisis yang sama terhadap sedikit sampel dosen (yang mungkin berkecimpung di dunia _life sciences_) dari lima Universitas di Indonesia (yang saya pilih seenak jidat). Anda dapat mengakses data dan kode yang digunakan untuk analisis ini di repository [lab-biotek-bio-ugm/sinta_bio_ugm](https://github.com/lab-biotek-bio-ugm/sinta_bio_ugm).

<div class="container">
  <iframe src="/files/01_clusterplot_publication_titles_ALL.html"
      sandbox="allow-same-origin allow-scripts"
      width="100%"
      height="280"
      scrolling="yes"
      seamless="seamless"
      frameborder="1">
  </iframe>
  <figcaption style="text-align: center;">Estimasi jumlah kluster keilmuan dengan berbagai metriks.</figcaption>
</div>

Tantangan pertama dari analisis ini adalah menentukan jumlah kluster keilmuan yang ada pada dataset. Untuk itu, saya hanya menggunakan informasi dari beberapa matriks, dan sepertinya k=6 adalah _sweet spot_.

<div class="container">
  <iframe src="/files/01_PCA_publication_titles_ALL.html"
      sandbox="allow-same-origin allow-scripts"
      width="100%"
      height="620"
      scrolling="yes"
      seamless="seamless"
      frameborder="1">
  </iframe>
  <figcaption style="text-align: center;">PCA dari ekstraksi <i>word feature</i> berdasarkan judul publikasi dosen di Google Scholar.</figcaption>
</div>

Hasil klustering ini tentunya tidak sempuran dan memiliki eksplanasi varians yang sangat rendah. Meskipun demikian, ada dua klaster yang cukup jelas terlihat pada plot, yaitu klaster 3 dan klaster 4. Klaster 3 sepertinya mendeskripsikan peneliti-peneliti di bidang biosistematika, konservasi, dan ekologi, sementara klaster 4 mendeskripsikan peneliti-peneliti di bidang fisiologi dan pemuliaan tanaman. _Nevertheless_, kita bisa melihat secara manual beberapa klaster kecil yang mengelompokkan dosen-dosen dengan profil penelitian yang mirip.

<figure>
  <a href="/files/co-author_subgraph_network_all.graphml.png" data-title="Jejaring co-authorship dosen">
      <img src="/files/co-author_subgraph_network_all.graphml.png" alt="Jejaring co-authorship dosen">
  </a>
<figcaption style="text-align: center;">
    Jejaring co-authorship dosen life science dari lima Universitas di Indonesia. Hanya co-author yang terhubung dengan lebih dari satu main author (dosen) ditunjukkan pada ilustrasi. Legend:<br>
    <img src="https://placehold.co/15x15/E41A1C/E41A1C.png" alt="#E41A1C" style="display: inline-block; vertical-align: middle; width: 15px; height: 15px;"> <span style="display: inline-block; vertical-align: middle;">IPB</span> 
    <img src="https://placehold.co/15x15/377EB8/377EB8.png" alt="#377EB8" style="display: inline-block; vertical-align: middle; width: 15px; height: 15px;"> <span style="display: inline-block; vertical-align: middle;">ITB</span>
    <img src="https://placehold.co/15x15/4DAF4A/4DAF4A.png" alt="#4DAF4A" style="display: inline-block; vertical-align: middle; width: 15px; height: 15px;"> <span style="display: inline-block; vertical-align: middle;">UB</span>
    <img src="https://placehold.co/15x15/984EA3/984EA3.png" alt="#984EA3" style="display: inline-block; vertical-align: middle; width: 15px; height: 15px;"> <span style="display: inline-block; vertical-align: middle;">UGM</span>
    <img src="https://placehold.co/15x15/FF7F00/FF7F00.png" alt="#FF7F00" style="display: inline-block; vertical-align: middle; width: 15px; height: 15px;"> <span style="display: inline-block; vertical-align: middle;">UI</span>
</figcaption>
</figure>

Jika kita melihat sekilas dari jejaring co-authorship yang ada, tidak dipungkiri bahwa kebanyakan kolaborasi berasal dari institusi yang sama. Hal ini sangat kuat terlihat di dua institusi, yaitu UGM dan ITB. Dari jejaring ini juga bisa kita identifikasi individu-individu yang menjadi pusat kolaborasi baik di dalam institusi maupun antar institusi.

## Disclaimer
Analisis dilakukan berdasarkan data dari SINTA dan juga Google Scholar. Tentu saja hasil analisis bergantung dari kualitas informasi yang mampu diambil dari portal data tersebut. Selain itu, banyak informasi di Google Scholar yang perlu dilengkapi oleh masing-masing dosen supaya datanya akurat.
