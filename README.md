# Semester4-MachineLearningApps

## Tentang Proyek Ini
Proyek ini adalah tugas akhir semester empat yang dikerjakan oleh 5 orang. Dengan goal membuat aplikasi mobile dan web yang terintergrasi oleh Machine Learning. Berikut nama anggota kelompok kami:

1. (E31231392) Mahayoga Ksatria Hanafi Bahtiar (Ketua)
2. (E31231430) Kahfi Adam Munajad (Anggota)
3. (E31231623) Affan Ardiansyah (Anggota)
4. (E31231594) Fila Indayani (Anggota)
5. (E31231704) Muamar Rosyidin (Anggota)

Proyek kami berisikan tentang intergrasi Machine Learning pada aplikasi mobile dan web menggunakan endpoint atau API (Flask) untuk menghubungkan antara model dengan aplikasi. Kami membuat website menggunakan framework yaitu Laravel, membuat aplikasi mobile menggunakan Flutter, dan terakhir membuat model ML dengan menggunakan Python.

Berikut adalah goal dari sistem kami:

1. [Model Machine Learning (ML)](https://github.com/Mahayoga/Semester4-MachineLearningModel.git)
   
   Membuat sebuah model dengan algoritma tertentu untuk bisa memprediksi suatu variabel dengan data sebelumnya. Data yang kami pilih adalah dengan tema pasien diabetes. Dataset dan detailnya bisa diperiksa [di sini](https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset).

2. [Website](https://github.com/Mahayoga/Semester4-WebApps.git) (Laravel)
   
   Kami membuat website dengan menggunakan framework Laravel 12. Goal dari website kami adalah memungkinkan pengguna (user) bisa memeriksa apakah user tersebut menderita diabetes atau tidak, melalui parameter seperti tekanan darah, BMI, umur, kehamilan, dan lain lain. Website kami juga memungkinkan untuk membuat halaman administrator untuk pemilik (admin) bisa menggunakan data user untuk dilakukan analisis lebih lanjut.

3. [Mobile](https://github.com/Mahayoga/Semester4-MobileApps.git) (Flutter)
   
   Aplikasi mobile kami sendiri tidak lain sama dengan website yang akan kami buat, tetapi hanya untuk halaman user saja. Aplikasi mobile kami ditujukan untuk memudahkan user untuk membuka aplikasi mobile dibanding mengakses web yang memerlukan data seluler.

4. API (Flask)
   
   Untuk API sendiri, kami menggunakan Flask, karena lebih mudah menggunakan bahasa pemrograman yang sama dengan pembuatan model yaitu Python agar memudahkan kami. Pembuatan API juga untuk menghubungkan antara permintaan dan respon dari atau ke aplikasi kami. 

5. Database (MongoDB)

   Database yang kami gunakan adalah MongoDB. Karena MongoDB tidak menggunakan konsep yang sama dengan MySQL, yaitu Structured Query Language (SQL). Yang memungkinkan performa yang dihasilkan oleh MongoDB ini lebih cepat dibanding MySQL. Mengingat data yang akan digunakan mungkin lebih dari 5000 baris, maka penggunaan MongoDB ini sangat disarankan.

### Pembagian Tugas
Kami juga sudah membagi tugas atau pekerjaan masing masing secara adil. Berikut detailnya:

1. Mahayoga Ksatria Hanafi Bahtiar
   
   Untuk Mahayoga, akan mengambil semua tugas (ML, Website, Mobile, dan API), tetapi yang utama adalah bertugas sebagai pembuatan ML. Sekaligus koordinator dari pembuatan ML.

2. Kahfi Adam Munajad

   Untuk Adam, akan mengambil tugas pembuatan Mobile, sekaligus koordinator dari bidang ini.

3. Affan Ardiansyah

   Untuk Affan, akan mengambil tugas pembuatan mobile dan website.

4. Fila Indayani

   Untuk Fila, akan mengambil tugas pembuatan website. Sekaligus menjadi koordinator dalam bidang ini.

5. Muamar Rosyidin

   Untuk Amar, akan mengambil tugas pembuatan ML. Membantu Mahayoga untuk pembuatan dan menyempurnakan model.

## Daftar Isi

## Sebelum Memulai

Hal hal yang harus diperhatikan sebelum meng-clone projek ini adalah menginstal beberapa kebutuhan untuk proyek ini, yaitu:

1. Program

   - PHP (versi 8.2 keatas)
   - Composer (untuk pelengkapan dependensi dari Laravel)
   - Node.js (versi terbaru)
   - Flutter SDK
   - Python (versi 3.12 keatas)
   - MongoDB (versi 8.0 keatas)
   - Git
   - Chrome
   - Visual Studio Code

2. Library Python
   
   - `pandas`
   - `scikit-learn`
   - `joblib`
   - `numpy`
   - `jupyter notebook` atau `jupyter lab`

### Aturan clone, pull, push, branch, merge

Selanjutnya adalah aturan untuk berkontribusi dalam proyek ini, terutama untuk para anggota kelompok harap diperhatikan agar kontribusi pada GitHub terhitung dan bisa menjadikan bukti bahwa telah ikut berkontribusi.

1. Clone
   
   Untuk clone sendiri tidak ada aturan khusus. Yanf perlu diperhatikan adalah satu repositori ini berisikan tiga folder, yaitu Model, Website, dan Mobile. Jika akan mengerjakan salah satu dari bidang diatas, maka masuk pada folder tersebut yang akan dikerjakan.

2. Pull

   Untuk melakukan pull sendiri, harap diperhatikan branch lokal dan branch remot yang akan di lakukan pull. Karena perintah pull sendiri adalah menimpa semua perubahan pada branch lokal ke branch remote.

3. Branch

   Aturan untuk branch sendiri adalah untuk mengerjakan masalah secara terpisah. Ini memungkinkan kita untuk menghindari error yang tercampur akibat perubahan yang tidak berhasil dilakukan. Dan harap diingat bahwasannya branch utama adalah bernama `main`. Jangan **PERNAH PUSH** ke dalam branch `main`.

4. Push

   Untuk push sendiri, tidak ada aturan khusus kecuali ke branch `main`. Dilarang push ke dalam branch `main` karena branch tersebut adalah branch **UTAMA** yang tidak terdapat sama sekali error.

5. Merge

   Merge akan dilakukan oleh pemilik dari repositori ini. Semua pull-request akan ditinjau agar tidak terjadi kesalahan pada branch `main`.

## Goal Aplikasi

Masing masing bidang memiliki target pembuatan. Sebelum masuk ke poin tersebut, kami akan membuat rancangan pembuatan terlebih dahulu untuk memudahkan pengembangan atau pembuatan aplikasi. Berikut rancangan yang kami buat:

- ERD (Entity Relationship Diagram)
- Use Case Diagram
- Flowchart
- Design Mockup Aplikasi

Selanjutnya kami akan mendeskripsikan jalannya sistem kami, mulai dari website, mobile, API, dan model yang akan dibuat.

1. Model Machine Learning (ML)

   Model kami bertujuan untuk memprediksi suatu data yang diberikan dari hasil latihan dataset yang sudah dilatih sebelumnya. Pembuatan model akan dilakukan dengan bahasa pemrograman Python.
   
   Pada proses pembuatan, akan dilakukan analisis hasil latihan model, seperti akurasi, confusion matrix, juga laporan klasifikasi. Setelah semuanya sudah sempurna, maka model sudah siap dilakukan dump menjadi file agar nantinya tidak menjalankan training secara berulang.

   Algoritma yang kami akan gunakan untuk sementara pembuatan model klasifikasi ini adalah Logistic Regression. Pilihan algoritma klasifikasi ini banyak yang salah satunya seperti Decision Tree, Linear Regression, SVM, KNN, dan lain lain. Nantinya kami akan mencoba semua algoritma diatas dan membandingkan hasil dari semua algoritma tersebut, mana yang lebih baik diatara semuanya.

2. API 

   Jembatan yang akan digunakan untuk komunikasi antara aplikasi dengan model adalah API (Flask). Pembuatan API akan sederhana karena hanya akan menerima request data dan response.

   Juga kemungkinan melakukan input CRUD data ke dalam MongoDB akan melalui API.

3. Website

   Website kami akan menampilkan beberapa menu yaitu diantara lain:

   - Dashboard (analisis data)

      Dashboard kami akan menampilkan analisis data pasien yang baru melakukan periksa maupun data sebelumnya yang belum ada. Kami akan menggunakan data tersebut untuk menampilkan statistik pasien seperti karakteristik dari data pasien diabetes. Dashboard juga akan dibuat untuk pengambilan keputusan.

   - Data Master

      Data master akan berisikan CRUD data pasien.

   - Menu prediksi data untuk pengguna admin

      Menu prediksi akan sama dengan menu pada tampilan pengguna (user).

4. Mobile

   Aplikasi mobile kami akan menampilkan beberapa menu yaitu diantara lain:

   - Tampilan beranda pasien
   - Menu prediksi pasien diabetes


# Stats

- Penulis: Mahayoga
- Revisi (perubahan README.md): 1
- Perubahan terakhir: 18 April 2025
- Kemungkinan terdapat revisi: sangat mungkin
- Status proyek: belum selesai (0%)
- Start: 7 Maret 2025
- End: -