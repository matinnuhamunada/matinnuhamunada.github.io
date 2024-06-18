---
title: 'Kisruh Rumpun Ilmu Kemdikbud'
date: 2024-06-17
permalink: /posts/2024/06/rumpunilmu
tags:
  - Indonesia
  - SINTA
---

| ![SINTA](https://pusatinformasi.sister.kemdikbud.go.id/hc/article_attachments/32738952650777) |
|:--:| 
| [Hierarki Rumpun Ilmu Kemdikbud](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/articles/31608506732057-Informasi-Umum-Rumpun-Ilmu)

Pada bulan Mei kemarin, dunia perdosenan Indonesia sempat ribut dengan pemadanan data rumpun ilmu dari Kemendikbud. Saya pun tidak luput dari keributan ini, mendadak mendapat undangan rapat di akhir pekan bersama anggota lab di Jogja. Karena mendadak, saya tidak sempat memahami latar belakang dan duduk perkara pemetaan bidang ilmu ini. Seingat saya, tahun sebelumnya kami pernah bersama-sama mengisi form terkait pengembangan ilmu di lab. Yang tersedia hanyalah tautan pdf berjudul `Daftar Rumpun, Pohon, dan Cabang Ilmu (2024).pdf` dari grup WhatsApp, yang berisi tabel daftar cabang ilmu sebanyak 38 halaman dimana kami diminta untuk memilih satu cabang ilmu yang akan melekat sepanjang karir kami sebagai dosen.

### Mencari Cabang Ilmu yang Sesuai
Setelah mencoba memahami duduk perkara ini, ternyata informasinya dapat diakses di [laman kemdikbud](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/articles/31608506732057-Informasi-Umum-Rumpun-Ilmu). Selain itu, kesesuaian cabang ilmu juga harus berdasarkan pendidikan formal dosen, yaitu sesuai ijazah tertinggi dan terakhir (S2/S3). Tentu hal ini seharusnya mempermudah para anggota lab untuk memilih cabang ilmu, karena tinggal melihat bidang ilmu yang ditekuni saat sekolah dan track record publikasi.

Masalah yang saya hadapi adalah mencari istilah yang sudah disediakan oleh kemdikbud. Ternyata, PDF tersebut sudah direvisi beberapa kali!
- [versi awal](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/article_attachments/32104508638617)
- [revisi 28 Mei 2024](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/article_attachments/33027824852633)
- [revisi 5 Juni 2024](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/article_attachments/33394150376985)

_To be honest_, kemdikbud bisa saja memberikan tabel untuk mempermudah pencarian istilah, daripada bentuk PDF. Selain itu, banyaknya kategori di rumpun ilmu terapan membuat pencarian istilah cabang ilmu semakin sulit. Saya penasaran bagaimana teman-teman di kemendikbud bisa mendapatkan istilah-istilah cabang ilmu sebanyak ini. Sepertinya ini daftar program studi yang sudah ada di Indonesia selama ini.

Untuk mempermudah diri (dan juga prokrastinasi), saya menyempatkan diri membuat repo untuk membaca tabel secara otomatis dari file PDF. Data kemudian divisualisasi menggunakan sunburst chart dari Plotly.

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

> Sunburst chart untuk ilmu hayati dan kesehatan [revisi 5 Juni 2024](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/article_attachments/33394150376985). File tabel (`.tsv`) dapat diunduh di [sini](https://github.com/lab-biotek-bio-ugm/rumpun_ilmu_kemdikbud/blob/main/data/processed/Daftar_Rumpun_Pohon_dan_Cabang_Ilmu_(Diperbarui_05_Juni_2024).tsv)

### Profil Cabang Ilmu di Fakultas Biologi UGM
Saat ini, pihak Fakultas sedang mempersiapkan cabang-cabang ilmu dari dosen yang ada di home base-nya, jadi kita belum tahu secara resmi siapa yang ditugaskan untuk bidang ilmu apa (_apparently it's not up to individuals to decide_). Meskipun belum jelas, sebenarnya ada cara yang lebih adil untuk memastikan kesesuaian bidang ilmu dari masing-masing dosen, yaitu melalui track record penelitiannya.

<div class="container">
  <iframe src="/files/01_PCA_publication_titles.html"
      sandbox="allow-same-origin allow-scripts"
      width="100%"
      height="600"
      scrolling="yes"
      seamless="seamless"
      frameborder="2">
  </iframe>
</div>

> PCA dari ekstraksi _word feature_ berdasarkan judul publikasi dosen di Google Scholar.

Sebagai informasi, Fakultas Biologi memiliki 12 laboratorium yang kurang lebih masing-masing menampung dosen-dosen dengan kepakaran yang serumpun. Pertanyaannya, apakah jumlah dan nama laboratorium ini masih relevan dengan profil dosen-dosen di dalamnya? Hmm, _interesting thought_! Menurut saya, agak sulit kalau memaksa individu untuk berganti bidang hanya karena terhalang dengan nama lab yang diampu. Bidang ilmu juga dinamis. Di era modern saat ini, banyak sekali bidang ilmu interdisipliner yang sulit untuk dimasukkan ke dalam "kotaknya" sendiri. Akhirnya, penempatan keahlian harus dikembalikan ke pendidikan dan juga track record penelitian dari masing-masing dosen.

<a href="/files/co-author_subgraph_network_reduced.graphml.png" data-title="Jejaring co-authorship dosen Fakultas Biologi UGM">
    <img src="/files/co-author_subgraph_network_reduced.graphml.png" alt="Jejaring co-authorship dosen Fakultas Biologi UGM">
</a>

> Jejaring co-authorship dosen Fakultas Biologi UGM.

Selain itu, sudah sewajarnya kolega dari lab yang berbeda mampu berkolaborasi satu sama lain. Hal itu juga terlihat dari jejaring co-authorship yang ada di Fakultas. Daripada berpusing-pusing mengkotak-kotakan ilmu, lebih baik kita tingkatkan semangat kolaborasi di antara kita :)

### Disclaimer
Analisis dilakukan berdasarkan data dari SINTA dan juga Google Scholar. Tentu saja hasil analisis bergantung dari kualitas informasi yang mampu diambil dari portal data tersebut. Jika dilihat lebih detail, informasi tentang Prof. Kumala Dewi tidak akurat, karena script yang saya buat tidak berhasil memperoleh ID Google Scholar beliau. Selain itu, banyak informasi di Google Scholar yang perlu dilengkapi oleh masing-masing dosen supaya datanya akurat.
