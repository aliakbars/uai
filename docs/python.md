# Python Programming


Materi yang diberikan di kelas dan referensi tambahan mengenai kuliah Pemrograman Python. Silakan *clone* repositori yang tersedia di [sini](https://github.com/aliakbars/uai-python/") untuk mendapatkan kode yang digunakan di kelas. Jawaban ujian bisa dilihat di [sini](https://www.dropbox.com/s/bau4ejxozqh41xh/jawaban.py?dl=0).

!!! warning "Umpan balik"
    Mohon untuk mengisi formulir umpan balik perkuliahan di [sini](https://goo.gl/forms/0bc40xTTApSznz3y2)

## Hello, World!

[Salindia minggu ke-1: Hello, Python!](https://github.com/aliakbars/uai-python/raw/master/01-hello.pdf)

Kuliah ini akan menggunakan Python 2.7 dengan asumsi bahwa Anda sudah familiar dengan pengembangan program secara umum. Akan ada beberapa script yang disediakan untuk menunjang perkuliahan, silakan unduh sebelum kelas dimulai.

[Salindia minggu ke-2: Struktur Data &amp; Pemrograman Fungsional](https://github.com/aliakbars/uai-python/raw/master/02-struktur-data.pdf)

Untuk tahu lebih lanjut tentang bahasa pemrograman fungsional dan apa yang bisa dilakukan, silakan melihat bahasa pemrograman seperti [LISP](https://www.common-lisp.net/) atau (lebih disarankan) [Haskell](https://www.haskell.org). Pemrograman dengan paradigma fungsional dimaksudkan untuk meniru pola fungsi matematis sehingga memudahkan saat *debugging*. Akan menyulitkan di awal untuk mengubah pola pikir [imperatif menjadi deklaratif](https://tylermcginnis.com/imperative-vs-declarative-programming/), tetapi seharusnya bisa berguna di kemudian hari.

!!! note
    Silakan evaluasi jawaban kuis Anda di situs [Google Code Jam](https://code.google.com/codejam/contest/32016/dashboard#s=p0).

## Pemrograman Berorientasi Objek

[Salindia minggu ke-3: Pemrograman Berorientasi Objek](https://github.com/aliakbars/uai-python/raw/master/03-oop.pdf)

Setelah membahas tentang Python dalam paradigma pemrograman fungsional, kali ini akan diulas tentang Python dalam paradigma pemrograman berorientasi objek (OOP). Namun, kuliah ini tidak membahas secara mendalam tentang konsep-konsep dalam OOP itu sendiri, e.g. *inheritance, dynamic binding, encapsulation*. Fokus dari materi kali ini adalah bagaimana konsep-konsep tersebut diterjemahkan secara sintaksis dalam bahasa Python. Dokumentasi Python tentang [modul](https://docs.python.org/2.7/tutorial/modules.html) dan [kelas](https://docs.python.org/2.7/tutorial/classes.html) dapat sangat membantu pemahaman Anda. Untuk belajar bagaimana menganalisis dan mendesain dalam OOP dengan lebih baik, saya sangat menyarankan untuk membaca Head First Object-Oriented Analysis and Design (McLaughlin, et al. 2006).

## Tugas 1

[Deskripsi Tugas 1](https://github.com/aliakbars/uai-python/raw/master/tugas-1.pdf)

[Kode Tugas 1](https://github.com/aliakbars/uai-python/blob/master/scripts/tugas/tugas1.py)

Dalam tugas pertama ini, Anda diminta untuk menyelesaikan kerangka dari sebuah program untuk permainan poker. Tugas ini akan mengevaluasi kemampuan Anda dalam membuat fungsi, pengolahan string, dan membuat kasus-kasus uji. Harapannya, tugas ini membantu Anda untuk melihat bahwa kasus yang terlihat kompleks ternyata dapat dipecah menjadi potongan-potongan fungsi sederhana yang diintegrasikan.

!!! warning "Tenggat"
    Selasa, 21 Maret 2017 pukul 23.55

## Pemrograman Web

[Salindia minggu ke-4: Pemrograman Web: Flask](https://github.com/aliakbars/uai-python/raw/master/04-flask.pdf)

Flask merupakan *microframework* yang dapat memudahkan pembuatan web sederhana dalam bahasa Python. Dengan menggunakan Flask, implementasi pemrograman web dalam Python bisa semudah mengerjakan web dalam bahasa PHP. Namun, kemudahan ini tentu ada harganya: hilangnya beberapa komponen penting untuk aplikasi skala besar. Tidak adanya kemampuan Flask untuk sanitasi input maupun pembuatan basis data dengan *Object Relational Mapper* (ORM) secara bawaan terkadang bisa membuat kode jadi lebih rumit. Namun, perlu diingat sekali lagi bahwa Flask memang ditujukan untuk program skala kecil, misalnya untuk pembuatan purwarupa.


[Salindia minggu ke-5: Pemrograman Web: Scraping](https://github.com/aliakbars/uai-python/raw/master/05-scraping.pdf)

Terkadang, kita perlu untuk mengambil sendiri data dari laman web. Beberapa web yang tidak menyediakan API mengharuskan kita untuk membuka sendiri laman tersebut lalu mengekstraksi informasinya satu per satu. Dengan melakukan *scraping*, kita bisa mengotomasi proses tersebut. Python mempunyai pustaka untuk melakukan hal tersebut dengan cukup mudah: Requests dan Beautiful Soup. Namun, ingat bahwa *scraping* sejatinya sering berada di posisi abu-abu - antara boleh atau tidak. Jadi, *be responsible*!

## Tugas 2

[Deskripsi Tugas 2](https://github.com/aliakbars/uai-python/raw/master/tugas-2.pdf)

[Pembagian Tim Tugas 2](https://github.com/aliakbars/uai-python/raw/master/tim.txt)

Anda akan mengerjakan tugas kedua dengan *pair programming*. Kelompoknya sudah dibagikan seperti file yang dilampirkan di atas. Selain itu, Anda diwajibkan menggunakan repositori yang telah disediakan di [GitHub](https://github.com/uai-python). Perhatikan bahwa **pengumpulan tugas** tetap harus dilakukan melalui **situs e-learning**!

!!! warning "Tenggat"
    Rabu, 5 April 2017 pukul 23.55

## Ulasan Materi

[Salindia minggu ke-7: Ulasan](https://github.com/aliakbars/uai-python/raw/master/07-review.pdf)

Minggu ini tidak ada materi tambahan. Kelas akan digunakan untuk mengulas materi yang telah lalu dan menyampaikan beberapa pengumuman terkait ujian dan sisa perkuliahan.

## Proposal Tugas Akhir

[Python Projects](/projects/)

[Template Proposal](https://github.com/aliakbars/uai-python/raw/master/proposal.pdf)

Untuk tugas akhir ini, Anda diminta untuk membuat proposal pengajuan topik dan ruang lingkup dari tugas yang Anda akan kerjakan. Secara berkala, Anda juga akan diminta melaporkan progres dari pekerjaan Anda. Dengan demikian, diharapkan pada akhir perkuliahan nanti, setiap mahasiswa dapat menyelesaikan proyeknya sehingga layak untuk didemokan. Setiap materi yang berkaitan dengan tugas akhir ini akan dipos melalui tautan di atas.

!!! warning "Pengumpulan"
    Submit proposal Anda melalui situs e-learning dengan **format PDF** paling lambat hari **Kamis, 11 Mei 2017 pukul 23.55**.

## Data

[Salindia minggu ke-8: Pengolahan Data](https://github.com/aliakbars/uai-python/raw/master/08-data.pdf)

Materi minggu ini berkaitan dengan pengolahan, analisis, dan visualisasi data. Beberapa materi akan membutuhkan pengetahuan statistik dan aljabar linear, tetapi akan dibuat sesederhana mungkin sehingga bisa dipahami dengan materi yang pernah diajarkan sejak SMA hingga kuliah tingkat awal. Untuk sisa materi, kita akan banyak berkutat dengan [Jupyter Notebook](http://jupyter.org/) sebagai editor dan tempat penyimpanan hasil pekerjaan -- termasuk tugas! Untuk pengguna Windows, disarankan untuk menggunakan [Anaconda](https://www.continuum.io/downloads) untuk Python 2.7[.](https://www.dropbox.com/s/mcjkwd9sskuv52x/kuis.pdf?dl=0")

[Salindia minggu ke-9: Visualisasi Data](https://github.com/aliakbars/uai-python/raw/master/09-visual.pdf)

Di minggu ini, Anda akan belajar tentang penggunaan matplotlib sebagai pustaka standar untuk melakukan visualisasi data di Python. Meski agak tertinggal dibandingkan pustaka visualisasi yang lebih interaktif di bahasa lain seperti D3.js, penting untuk memahami dasar-dasar visualisasi dan pustaka yang sebetulnya sangat mumpuni ini. Salindia minggu ini tidak terlalu banyak isinya karena akan lebih banyak didemokan di kelas. Silakan lihat materi visualisasi di [notebook ini](http://nbviewer.jupyter.org/github/aliakbars/uai-python/blob/master/scripts/week9/visualisation.ipynb).

## Tugas 3

[Deskripsi Tugas 3](http://nbviewer.jupyter.org/github/aliakbars/uai-python/blob/master/scripts/tugas/tugas3.ipynb)

Anda akan mengerjakan tugas ketiga secara perorangan dan materinya akan berhubungan dengan manipulasi dan visualisasi data. Untuk tugas ketiga ini, Anda hanya perlu mengumpulkan file tugas3.ipynb saja melalui situs e-learning!

!!! warning "Tenggat"
    Selasa, 16 Mei 2017 pukul 23.55

## Artificial Intelligence

[Salindia minggu ke-10: Machine Learning &amp; Pattern Recognition](https://github.com/aliakbars/uai-python/raw/master/10-mlpr.pdf)

Sebagai lanjutan dari materi minggu lalu, kali ini Anda akan dikenalkan dengan pustaka Python untuk melakukan pembelajaran mesin dan pengenalan pola. Karena materi ini membutuhkan keahlian khusus yang mungkin baru didapatkan di tingkat tiga (sebagian juga masuk ke kuliah pilihan), maka banyak materi yang tidak disampaikan saat ini. Harapannya, sedikit contoh ini bisa memberikan gambaran kepada Anda tentang apa yang bisa dilakukan dalam salah satu area kecerdasan buatan yang sedang sangat berkembang ini.

[Salindia minggu ke-11: Natural Language Processing](https://github.com/aliakbars/uai-python/raw/master/11-nlp.pdf)

Salah satu cabang dari ilmu *artificial intelligence* (AI) adalah pemrosesan bahasa alami atau *natural language processing* (NLP). Minggu ini, kita akan membahas beberapa tugas yang biasa dilakukan dalam NLP menggunakan salah satu pustaka yang umum digunakan, yaitu Natural Language Toolkit (NLTK). Kita juga akan melihat hubungan dari NLP dengan pembelajaran mesin yang telah dipelajari minggu lalu.

## Tugas 4

[Deskripsi Tugas 4](https://nbviewer.jupyter.org/github/aliakbars/uai-python/blob/master/scripts/tugas/tugas4.ipynb)

[Dataset Tugas 4](https://drive.google.com/open?id=0B5Ei3oQejW8NUkViTXkzOXVpN3c)

[Label Dataset Tugas 4](https://drive.google.com/open?id=0B5Ei3oQejW8Nd0ZWYlV0QTJJYlE)

Tugas Anda kali ini adalah melakukan klasifikasi gambar untuk dua jenis dataset: digit dan hewan. Dataset tersebut menggunakan MNIST dan Quick Draw yang baru dirilis oleh Google. Anda hanya akan menggunakan subset dari dataset Quick Draw. Anda mungkin akan perlu untuk belajar sedikit pustaka Keras di [sini](https://drive.google.com/open?id=10V2iEm1KfvjXtJ-tfBt87FVGMeKf0njoHuetmmb3O3w). Subset ini telah disiapkan pada tautan di atas. Untuk tugas keempat ini, Anda hanya perlu mengumpulkan file tugas4.ipynb saja melalui situs e-learning!

!!! warning "Tenggat"
    Selasa, 6 Juni 2017 pukul 23.55

## Implementasi Lain

[Salindia minggu ke-12: Beyond Python](https://github.com/aliakbars/uai-python/raw/master/12-beyond.pdf)

Materi terakhir dalam kuliah Pemrograman Python berisi tentang pengenalan beberapa implementasi interpreter Python dalam berbagai bahasa. Selain itu, dikenalkan juga Cython sebagai bahasa superset dari Python. Terdapat pula penjelasan tentang pemakaian Python di industri.

## Tugas Akhir

Submit file tugas akhir dalam bentuk folder yang telah di-zip **(ingat, ekstensinya harus .zip, bukan yang lain)**. Sertakan pula file **requirements.txt** yang berisi *dependencies* dari proyek yang kalian kerjakan. Berikan file **readme** jika diperlukan untuk mengetahui cara menjalankan aplikasi yang telah dibuat. Tugas ini dikumpulkan melalui e-learning.

!!! warning "Tenggat"
    Jumat, 23 Juni 2017 pukul 23.55