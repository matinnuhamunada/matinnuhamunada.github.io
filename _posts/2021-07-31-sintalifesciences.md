---
title: 'Memetakan Peneliti Life Sciences di Indonesia'
date: 2021-07-30
permalink: /posts/2021/07/sintalifesciences
tags:
  - Indonesia
  - SINTA
---
| ![SINTA](https://sinta.ristekbrin.go.id/assets/img/sinta_logo.png) |
|:--:| 
| [SINTA - Database peneliti dan dosen Indonesia](https://sinta.ristekbrin.go.id/)

_Check the source_ [**_here_**](https://github.com/matinnuhamunada/SINTA_data_mining)

## _Goals_
Tulisan ini bertujuan untuk memetakan peneliti _life sciences_ di Indonesia. Dengan memetakan bidang keahlian peneliti _life sciences_, diharapkan kita dapat dengan mudah mencari kolaboran di berbagai institusi di Indonesia.

## _Warning & Caveats_
* _I am by no means someone experienced with bibliometric analyses_
* Informasi hanya didasarkan pada database SINTA sehingga afiliasi dan data peneliti belum tentu akurat
* Proyek ini tidak ditujukan untuk merangking atau membandingkan kualitas peneliti di suatu institusi. Indeks sitasi tidak sepenuhnya dapat digunakan untuk menilai kualitas seorang peneliti. _Recommended read_ di [*https://theconversation.com*](https://theconversation.com/jalan-evolusi-bibliometrik-indonesia-104781)
* Pemilihan institusi dan bidang ilmu peneliti sepenuhnya subjektif (bidang ilmu apa saja yang termasuk _Life Sciences?_)

## _The Result_
<div class="container">
  <iframe src="/files/bio_sinta.html"
      sandbox="allow-same-origin allow-scripts"
      width="100%"
      height="700"
      scrolling="no"
      seamless="seamless"
      frameborder="0">
  </iframe>
</div>

## _Backstory_
Proyek iseng scraping peneliti _life sciences_ di Indonesia ini berawal dari kesulitan saya menjawab pertanyaan seorang kolega di tahun 2018: **"Siapa sih pakar biologi molekuler di UGM? Penelitiannya tentang apa?"** 

_Well_, biologi molekuler sendiri merupakan bidang ilmu yang cukup luas, apalagi dengan trend interdisiplin saat ini, cukup susah rasanya untuk mendefinisikan apa yang dimaksud oleh yang bertanya. Tentu saja, hal yang pertama saya lakukan adalah membuka mbah google, dan menelusuri laman2 di bawah domain ugm.ac.id.... sampai saya menyerah 1 jam kemudian.

Disini, saya mencoba mencari jawabannya dengan menggunakan informasi dari SINTA [Science and Technology Index](https://sinta.ristekbrin.go.id), sebuah database peneliti yang diperkenalkan oleh Kementerian Riset, Teknologi, dan Pendidikan Tinggi di tahun 2017. Kebetulan saat itu para staf pengajar di UGM juga sedang didata untuk dimasukkan ke dalam database tersebut.

Pada awal mula saya mencoba _scraping data_ dari SINTA, belum terdapat fitur departemen pada afiliasi. Terpaksa saat itu saya harus mencoba scraping data dari laman masing-masing kampus yang ingin saya bandingkan. _Trust me you don't want to go through all the efforts!_

Baru tiga tahun kemudian saya mendapat kesempatan untuk melanjutkan proyek ini. Selain dikarenakan libur musim panas di Denmark yang cukup panjang, semangat untuk menyelesaikan proyek ini juga dimotivasi oleh komentar dosen senior mengenai produktifitas staf-staf muda. 

Saya beruntung, ternyata [@rendicahya](https://github.com/rendicahya) membuat [sinta-scraper](https://github.com/rendicahya/sinta-scraper) yang memudahkan semua proses pengambilan data.

## Bagaimana kamu bisa berkontribusi?
Tentu analisis ini masih jauh dari sempurna dan dibuat demi keisengan semata. Oleh karena itu, saya mengajak anda untuk berkontribusi dengan cara:
* Melakukan kurasi terhadap data, baik dengan mengisi tabel identitas peneliti secara manual, atau juga memberikan informasi mengenai peneliti yang sudah pensiun / tidak aktif.
* Memberikan rekomendasi peneliti atau institusi _life sciences_
* Mengolah dan menganalisis data
* Memberikan kritikan dan masukan
* _Check the source_ [**_here_**](https://github.com/matinnuhamunada/SINTA_data_mining)

Terima kasih sudah membaca tulisan ini :)
