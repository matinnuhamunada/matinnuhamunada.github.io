---
title: 'Ribut Rumpun Ilmu Kemdikbud'
date: 2024-06-17
permalink: /posts/2024/06/rumpunilmu
tags:
  - Indonesia
  - SINTA
  - Dosen
---

| ![Rumpun Ilmu Kemdikbud](https://www.kemdikbud.go.id/assets/imgs/kemdikbud_64x64.png) |
|:--:| 
| [Hierarki Rumpun Ilmu Kemdikbud](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/articles/31608506732057-Informasi-Umum-Rumpun-Ilmu) |

### Kisruh Akhir Pekan
Pada bulan Mei lalu, dunia akademisi Indonesia dihebohkan dengan pemetaan data rumpun ilmu oleh Kementerian Pendidikan dan Kebudayaan. Saya pun tidak luput dari keributan ini. Pada Jumat sore, saya tiba-tiba mendapat undangan rapat di akhir pekan bersama anggota lab di Jogja. Karena mendadak, saya tidak sempat mempelajari latar belakang dan detail pemetaan bidang ilmu ini. Seingat saya, ahun sebelumnya kami pernah mengisi formulir terkait pengembangan ilmu di lab. Materi yang tersedia untuk rapat akhir pekan tersebut hanyalah tautan pdf berjudul `Daftar Rumpun, Pohon, dan Cabang Ilmu (2024).pdf` yang dibagikan dari grup WhatsApp, berisi tabel daftar cabang ilmu sepanjang 38 halaman. Kami diminta memilih satu cabang ilmu yang akan melekat sepanjang karir kami sebagai dosen.

### Mencari Cabang Ilmu yang Sesuai

| ![Rumpun Ilmu Kemdikbud](https://pusatinformasi.sister.kemdikbud.go.id/hc/article_attachments/32738952650777) |
|:--:| 
| [Hierarki Rumpun Ilmu Kemdikbud](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/articles/31608506732057-Informasi-Umum-Rumpun-Ilmu) |

Setelah mencoba memahami situasi ini, saya menemukan bahwa informasi lengkapnya bisa diakses di [laman Kemdikbud](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/articles/31608506732057-Informasi-Umum-Rumpun-Ilmu). Kesesuaian cabang ilmu harus didasarkan pada pendidikan formal dosen, yaitu ijazah tertinggi yang mereka miliki (S2/S3). Hal ini seharusnya mempermudah anggota lab dalam memilih cabang ilmu yang tepat, karena tinggal menyesuaikannya dengan bidang studi yang mereka tekuni saat sekolah dan rekam jejak publikasi mereka.

Kerumitan yang banyak dihadapi kolega dosen adalah mencari istilah cabang ilmu yang disediakan oleh kemdikbud. Setelah menilik lebih jeli, ternyata, PDF tersebut sudah direvisi beberapa kali, dan saya tidak menggunakan dokumen yang terbaru:
- [versi awal](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/article_attachments/32104508638617)
- [revisi 28 Mei 2024](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/article_attachments/33027824852633)
- [revisi 5 Juni 2024](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/article_attachments/33394150376985)

_To be honest_, Kemdikbud bisa saja memberikan tabel (.csv, .excel?) untuk mempermudah pencarian istilah daripada dalam bentuk PDF. Selain itu, banyaknya kategori di rumpun ilmu terapan membuat pencarian istilah cabang ilmu semakin sulit. Saya penasaran bagaimana teman-teman di Kemdikbud bisa mendapatkan istilah-istilah cabang ilmu sebanyak ini. Sepertinya ini adalah daftar program studi yang sudah ada di Indonesia selama ini.

Untuk mempermudah pencarian (dan juga sedikit prokrastinasi dari menulis thesis), saya menyempatkan diri membuat repository untuk membaca tabel secara otomatis dari file PDF. Data ini kemudian divisualisasi menggunakan `sunburst chart` dari `plotly`. Ini sangat membantu dalam melihat struktur dan cabang ilmu secara lebih intuitif.

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

### Profil Cabang Ilmu di Fakultas Biologi UGM
Saat ini, pihak Fakultas sedang mempersiapkan cabang-cabang ilmu dari dosen yang ada di home base-nya, melalui proses diskusi dan negosiasi di masing-masing laboratorium. Pada postingan berikut, saya mencoba mengeksplorasi dan mengelompokkan bidang ilmu masing-masing dosen melalui sepak terjang penelitiannya. Hal ini sejalan dengan pentingnya mencocokkan bidang ilmu dengan pendidikan formal dan publikasi yang telah dilakukan dosen, seperti yang saya temui sebelumnya dalam proses pemetaan rumpun ilmu.

Sebagai informasi, Fakultas Biologi memiliki 12 laboratorium yang masing-masing menampung dosen-dosen dengan kepakaran yang serumpun. Pertanyaannya, apakah jumlah dan nama laboratorium ini masih relevan dengan profil dosen-dosen di dalamnya? Menurut saya, mungkin akan lebih bijaksana jika penempatan keahlian tidak terlalu kaku berdasarkan nama lab. Macam bidang ilmu sangat dinamis dan terus berkembang, terutama di era modern saat ini di mana banyak bidang ilmu interdisipliner sulit dimasukkan ke dalam kategori yang _rigid_. Oleh karena itu, kembali lagi, penempatan keahlian sebaiknya didasarkan pada pendidikan dan _track record_ penelitian dari masing-masing dosen, sehingga mereka dapat terus berkembang sesuai dengan keahlian dan minat mereka.

#### Klusterisasi Keilmuan Dosen Berdasarkan Judul Penelitian
Disini saya mencoba menggunakan judul penelitian dari google scholar untuk mengelompokkan dosen-dosen yang memiliki bidang kepakaran yang mirip.

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

Langkah pertama yang dilakukan adalah menemukan kata-kata yang paling sering muncul dalam setiap kelompok keilmuan. Ini dapat dilakukan dengan menghitung nilai TF-IDF (Term Frequency-Inverse Document Frequency), yaitu metode yang digunakan dalam _text mining_ dan _natural language processing_ untuk mengevaluasi seberapa penting suatu kata dalam suatu dokumen relatif terhadap kumpulan dokumen lainnya (_corpus_). Selanjutnya, kita perlu memfilter _stop words_ (kata-kata umum yang diabaikan) dalam bahasa Inggris dan Indonesia agar hasil analisis lebih relevan. _Stop words_ ini diambil dari pustaka `TfidfVectorizer` dan ditambahkan dengan kata-kata khusus dari bahasa Indonesia yang sering muncul dalam judul penelitian tapi kurang bermakna (e.g. dan, atau, terhadap, etc). Kemudian kita lakukan preprocessing dan vektorisasi teks dimana judul-judul penelitian diproses menjadi bentuk yang bisa dianalisis dengan menghitung nilai TF-IDF untuk setiap kata dalam judul tersebut. Proses ini dilakukan untuk semua judul penelitian dosen. Selanjutnya kita lakukan agregasi data dan reduksi dimensi menggunakan PCA (Principal Component Analysis). PCA mengubah data ke dalam tiga komponen utama yang menjelaskan variasi terbesar dalam data. Hasil PCA ini kemudian kita gunakan untuk mengelompokkan dosen (Clustering) dengan algoritma KMeans ke dalam 12 kelompok (_hopefuly it represents the labs?_).

Hasil dari pengelompokan ini divisualisasikan dalam bentuk diagram yang menunjukkan bagaimana dosen-dosen dikelompokkan berdasarkan keahlian penelitian mereka. Semakin dekat posisi satu dosen dengan dosen lainnya, kepakaran mereka semakin dekat (_based on publication_). Meskipun demikian, hasil clustering menunjukkan Silhouette Score sebesar 0.33 dan persentase variance explanation yang rendah. Nilai yang mendekati 0 ini menunjukkan bahwa objek berada di perbatasan antara dua kluster, yang berarti pengelompokan kurang jelas atau tumpang tindih. Tentu saja banyak faktor yang mempengaruhi hasil analisis dan kita tidak bisa serta merta mengambil kesimpulan bahwa pengelompokkan dosen berdasarkan lab kurang sesuai dengan kepakaran. Beberapa faktor penting yang perlu dipertimbangkan yaitu: (1) kita hanya menggunakan judul penelitian, bukan abstrak, jadi banyak informasi penting mengenai riset dosen yang belum tertangkap; (2) tidak semua dosen sudah mengupdate profile google scholar mereka; (3) penggunaan algoritma dan metode kurang sesuai untuk merepresantasi fitur keilmuan dosen.

#### Kolaborasi Antar Dosen

<a href="/files/co-author_subgraph_network_reduced.graphml.png" data-title="Jejaring co-authorship dosen Fakultas Biologi UGM">
    <img src="/files/co-author_subgraph_network_reduced.graphml.png" alt="Jejaring co-authorship dosen Fakultas Biologi UGM">
</a>

> Jejaring co-authorship dosen Fakultas Biologi UGM. Hanya co-author yang terhubung dengan lebih dari satu main author (dosen) ditunjukkan pada ilustrasi.

Hal lain yang dapat kita lihat adalah bagaimana para dosen terhubung dengan dosen lainnya melali jejaring co-authorship. Di sini, jejaring saya simplifikasi dengan menghilangkan banyak co-author eksternal yang hanya terhubung dengan satu dosen. Dari jejaring ini, kita bisa melihat siapa berkolaborasi dengan siapa. Meskipun informasi yang digunakan belum lengkap, dapat dilihat bahwa sudah cukup banyak dosen yang menulis paper bersama (_BTW, kita juga bisa lihat relasi mahasiswa-pembimbing dalam jejaring ini_). Jika dilihat, sebagian dosen tidak terhubung dengan dosen lainnya walaupun kita tahu mereka sudah banyak berkolaborasi satu sama lain. Sekali lagi, jejaring ini dibuat dengan menggunakan informasi dari google scholar, dimana belum semua dosen mengupdate daftar co-author mereka.

Sudah sewajarnya kolega dari lab yang berbeda mampu berkolaborasi satu sama lain. Hal itu juga terlihat dari jejaring co-authorship yang ada di Fakultas. Daripada berpusing-pusing mengkotak-kotakan ilmu, lebih baik kita tingkatkan semangat kolaborasi di antara kita :)

### Disclaimer
Analisis dilakukan berdasarkan data dari SINTA dan juga Google Scholar. Tentu saja hasil analisis bergantung dari kualitas informasi yang mampu diambil dari portal data tersebut. Jika dilihat lebih detail, informasi tentang Prof. Kumala Dewi tidak akurat, karena script yang saya buat tidak berhasil memperoleh ID Google Scholar beliau. Selain itu, banyak informasi di Google Scholar yang perlu dilengkapi oleh masing-masing dosen supaya datanya akurat.
