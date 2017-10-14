# Data Mining

## Pendahuluan

Ada baiknya untuk sedikit mengulas materi aljabar linear, kalkulus, dan statistika Anda sebelum memulai kuliah ini. Silakan lihat [*crib sheet*](http://www.inf.ed.ac.uk/teaching/courses/it/cribsheet.2up.pdf) yang disediakan oleh Iain Murray. Untuk pemahaman lebih lanjut, Anda juga bisa melihat materi probabilitas untuk ilmu komputer yang sangat menarik di kuliah [Stanford: CS109](http://web.stanford.edu/class/cs109/index.html).

!!! info "Referensi"
    Kuliah ini banyak mengadaptasi materi dari [Introductory Applied Machine Learning](http://www.inf.ed.ac.uk/teaching/courses/iaml/) dari the University of Edinburgh.

Karena kuliah ini akan menggunakan Python sebagai bahasa pengantarnya, silakan cek [tutorial singkat untuk Python dan Numpy](http://cs231n.github.io/python-numpy-tutorial/). Anda juga akan menggunakan Jupyter notebook ke depannya. Silakan lihat petunjuk instalasinya di [sini](http://jupyter.org/install.html).

Anda dapat membuat *clone* dari repositori mata kuliah ini di [sini](https://github.com/aliakbars/uai-dm).

## Konsep Data Mining

[Salindia minggu ke-1: Pendahuluan](https://github.com/aliakbars/uai-dm/raw/master/01-intro.pdf)

Apa yang menjadi hubungan antara *data mining* dengan *big data*? Apa saja yang menjadi bagian dari *data mining*?
Pertanyaan seperti ini mungkin sering muncul dalam kehidupan kita sehari-hari. Kuliah ini membahas betapa dekatnya data dengan kehidupan kita sehari-hari
dan bagaimana proses pencarian pola dalam data tersebut dapat menjadi hal yang sangat menyenangkan untuk dilakukan.

[Salindia minggu ke-2: Tipe dan Jenis Data](https://github.com/aliakbars/uai-dm/raw/master/02-data.pdf)

Apakah ada hubungannya antara kebiasaan menambahkan kecap dan kacang pada [preferensi untuk mengaduk bubur ayam](http://tentangdata.github.io/assets/buburayam.jpg)? Lalu, bagaimana gambar dapat direpresentasikan sebagai data yang dapat diolah oleh algoritma *machine learning*? Materi di minggu ini membahas tipe dan jenis data serta bagaimana merepresentasikannya. Kasus-kasus seperti [*imbalanced dataset*](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.96.9248&rep=rep1&type=pdf) juga akan menjadi poin penting dari kuliah ini.


## Eksplorasi Data

[Salindia minggu ke-3: Jarak Antardata dan Eksplorasi Data](https://github.com/aliakbars/uai-dm/raw/master/03-eksplorasi.pdf)

[Praktikum 1: Eksplorasi dan Visualisasi](https://nbviewer.jupyter.org/github/aliakbars/uai-dm/blob/master/scripts/lab1.ipynb)

Visualisasikan data Anda! Visualisasi data dapat membantu dalam memahami tren dan pola-pola menarik dari data Anda. Anda mungkin perlu melihat salindia [ini](https://nces.ed.gov/forum/pdf/NCES_table_design.pdf) untuk membantu merancang tabel dan grafik dengan lebih baik. Materi kali ini juga dilengkapi dengan praktikum yang diharapkan dapat memberikan gambaran tentang penggunaan konsep-konsep yang disampaikan di minggu ini.

Rumus Minkowski distance saat *r* (atau dalam rumus di bawah ini *p*) mendekati tak hingga adalah selisih antara dua titik terjauh dalam bidang cartesian. Perhitungan jarak ini juga dikenal dengan nama [Chebyshev distance](https://en.wikipedia.org/wiki/Chebyshev_distance). Dengan kata lain, rumusnya menjadi:

![Chebyshev distance](https://wikimedia.org/api/rest_v1/media/math/render/svg/a25e6422d6342df00a038d97507e8ff9a6d56b04)

Intuisi yang lebih baik untuk Mahalanobis distance bisa dibaca di [sini](http://stats.stackexchange.com/questions/62092/bottom-to-top-explanation-of-the-mahalanobis-distance). Penjelasan tersebut memberikan gambaran bahwa Mahalanobis distance bekerja seperti Euclidean distance, tetapi sumbu-sumbunya disusun berdasarkan sebaran dari datanya. Kita akan mencari arah sumbu baru beserta panjangnya. Dalam kuliah reduksi dimensi nanti, kita akan melihat hubungan Mahalanobis distance dengan Principal Component Analysis.


## Tugas 1

[Notebook Tugas 1](https://nbviewer.jupyter.org/github/aliakbars/uai-dm/blob/master/scripts/tugas1b.ipynb)

[Dataset Tugas 1](https://github.com/aliakbars/uai-dm/raw/master/dataset/movie_metadata.csv)

Dalam tugas ini, Anda diminta untuk melakukan eksplorasi, analisis, dan visualisasi terhadap dataset yang berisi film dari IMDB. Anda akan mencari tahu hal-hal yang berkaitan dengan kesuksesan sebuah film. Berdasarkan perhitungan *similarity*, Anda akan diminta juga melakukan klasifikasi sederhana terhadap data baru yang diberikan. Tugas ini dikumpulkan melalui situs e-learning UAI.

!!! warning "Tenggat"
    Kamis, 12 Oktober 2017, pukul 23.55 WIB

## Klasifikasi

[Salindia minggu ke-4: Klasifikasi: Naive Bayes](https://github.com/aliakbars/uai-dm/raw/master/04-naivebayes.pdf)

[Latihan 1: Naive Bayes](https://github.com/aliakbars/uai-dm/raw/master/latihan-1.pdf)

[Praktikum 2: Klasifikasi](https://nbviewer.jupyter.org/github/aliakbars/uai-dm/blob/master/scripts/lab2.ipynb)

Salah satu metode klasifikasi yang cukup sederhana tetapi berfungsi dengan cukup baik pada praktiknya adalah Naive Bayes. Metode ini tidak memerlukan *hyperparameter tuning* seperti banyak metode klasifikasi yang lebih kompleks lainnya. Idenya pun didasari pada asumsi naif bahwa setiap atribut *conditionally independent* jika diberikan kelasnya. Namun, asumsi ini ternyata bisa jadi efektif, seperti yang diteliti dalam makalah [ini](http://venus.unive.it/romanaz/complstat/hand_naive_bayes.pdf).

Asumsi lain yang digunakan dalam algoritma ini adalah distribusi Gaussian yang dipakai untuk data yang kontinu. Untuk menyegarkan kembali ingatan Anda tentang materi distribusi Gaussian, Anda bisa melihat [tulisan Iain Murray](http://www.inf.ed.ac.uk/teaching/courses/mlpr/2016/notes/w2b_univariate_gaussian.html) (2016). Selain itu, sangat disarankan untuk melihat video dari [Stats 110](https://www.youtube.com/watch?v=72QjzHnYvL0&list=PL2SOU6wwxB0uwwH80KTQ6ht66KWxbzTIo&index=13") dari Harvard University untuk membantu pemahaman Anda tentang probabilitas dan peubah acak. Beberapa orang juga menyarankan untuk membaca ulasan materi probabilitas dan statistika dari buku Deep Learning (Goodfellow et al., 2016). Materinya bisa Anda akses di [sini](http://www.deeplearningbook.org/contents/prob.html).

Berikut ini adalah [video](https://www.youtube.com/watch?v=os-NaA0ldGs&list=PLBv09BD7ez_6CxkuiFTbL3jsn2Qd1IU7B) oleh Victor Lavrenko yang dapat Anda gunakan untuk membantu pemahaman Anda terhadap materi Naive Bayes.

[Salindia minggu ke-5: Klasifikasi: Decision Trees](https://github.com/aliakbars/uai-dm/raw/master/05-dt.pdf)

Pohon keputusan merupakan algoritma klasifikasi yang memudahkan pengguna untuk memahami jalannya proses klasifikasi suatu data. Bagi *end-user*, tidak perlu pemahaman statistika yang mendalam untuk tahu apa yang terjadi. Di sisi lain, algoritma ini bisa jadi cukup efektif. Terbukti, pengembangan algoritma ini, yaitu XGBoost dan Random Forest, sering dipakai di berbagai kompetisi dan makalah *data mining*. Materi minggu ini membahas tentang bagaimana kita bisa membentuk pohon keputusan untuk melakukan klasifikasi, termasuk bagaimana kita dapat mengevaluasi hasil klasifikasi tersebut.


<!-- ## Tugas 2

[Notebook Tugas 2](https://nbviewer.jupyter.org/github/aliakbars/uai-dm/blob/master/scripts/tugas2.ipynb)

[Dataset Tugas 2: Training](https://github.com/aliakbars/uai-dm/raw/master/dataset/train.p)

[Dataset Tugas 2: Validation](https://github.com/aliakbars/uai-dm/raw/master/dataset/val.p)

[Dataset Tugas 2: Test](https://github.com/aliakbars/uai-dm/raw/master/dataset/test.p)

Dalam tugas ini, Anda diminta untuk melakukan klasifikasi dengan menggunakan algoritma Naive Bayes dan Decision Trees. Anda diminta menjelaskan dan mengimplementasikan beberapa komponen dari kedua jenis algoritma tersebut. Silakan merujuk ke materi praktikum 2 untuk mencari beberapa referensi kode yang dapat digunakan. Tugas ini dikumpulkan melalui situs e-learning UAI.

!!! warning "Tenggat"
    Jumat, 14 April 2017, pukul 23.55 WIB -->

## Evaluasi Model

[Salindia minggu ke-6: Evaluasi Model]()

Kapan akurasi tidak cukup lagi untuk dijadikan satu-satunya *metrics*? Bagaimana pula cara untuk menghasilkan model yang optimal? Kita akan mengeksplorasi penggunaan *metrics* lain yang dapat dihitung dari *confusion matrix*. Selain itu, akan dikenalkan juga ROC curves serta AUC yang biasa digunakan pada kasus *imbalanced dataset*.

## Ulasan Materi

[Salindia minggu ke-7: Ulasan Materi](https://github.com/aliakbars/uai-dm/raw/master/07-review.pdf)

Minggu ini ada sedikit materi tambahan. Silakan cek kembali materi praktikum 2 untuk tambahan tentang klasifikasi dengan pohon keputusan. Kelas akan digunakan untuk mengulas materi yang telah lalu dan menyampaikan beberapa pengumuman terkait ujian dan tugas.

## Model Linear

[Salindia minggu ke-8: Model Linear](https://github.com/aliakbars/uai-dm/raw/master/08-linear.pdf)

[Praktikum 3: Model Linear](https://nbviewer.jupyter.org/github/aliakbars/uai-dm/blob/master/scripts/lab3.ipynb)

Setelah berkutat dengan beberapa algoritma klasifikasi, materi minggu ini berisikan salah satu tugas dalam *machine learning* yang lain: regresi. Anda akan dikenalkan dengan regresi linear sederhana dan beberapa pengembangannya. Selain itu, Anda juga akan melihat bagaimana ide regresi linear kemudian bisa diubah untuk kebutuhan klasifikasi. Dalam materi minggu ini, Anda akan melihat dengan lebih jelas perbedaan model generatif dan diskriminatif.

## Model Berdasarkan Perhitungan Jarak

[Salindia minggu ke-9: k-Nearest Neighbours &amp; k-Means Clustering](https://github.com/aliakbars/uai-dm/raw/master/09-knn.pdf)

[Praktikum 4: k-Nearest Neighbours &amp; k-Means](https://nbviewer.jupyter.org/github/aliakbars/uai-dm/blob/master/scripts/lab4.ipynb)

Tidak ada hubungan yang khusus antara kedua algoritma yang dikenalkan minggu ini, kecuali keduanya didasarkan pada perhitungan jarak antarobjek. k-NN merupakan algoritma yang bisa digunakan untuk klasifikasi dan juga regresi (*supervised learning*), semenara k-Means merupakan algoritma untuk *clustering* (*unsupervised learning*). Akan ada beberapa algoritma *clustering* lain yang akan dikenalakan di materi selanjutnya setelah k-Means.

## Clustering

[Salindia minggu ke-10: Gaussian Mixture Models &amp; Hierarchical Clustering](https://github.com/aliakbars/uai-dm/raw/master/10-gmm.pdf)

[Praktikum 5: Gaussian Mixture Models](https://nbviewer.jupyter.org/github/aliakbars/uai-dm/blob/master/scripts/lab5.ipynb)

Materi minggu ini merupakan pengembangan dari algoritma k-Means. Dengan menggunakan pendekatan parametrik, kita bisa menghasilkan clustering dengan model generatif. Lihat kembali tentang materi distribusi Gaussian untuk memahami dengan lebih baik materi minggu ini. Selain itu, kita juga akan melihat bahwa alih-alih menentukan nilai K dari awal, kita bisa membuat level granularity dari klaster yang dihasilkan dengan membuat hierarki.

## Reduksi Dimensi

[Salindia minggu ke-11: Dimensionality Reduction](https://github.com/aliakbars/uai-dm/raw/master/11-dim.pdf)

Dimensionality reduction merupakan bagian dari *unsupervised learning* yang biasanya digunakan untuk bermacam hal, misalnya membantu visualisasi, mempercepat proses klasifikasi, hingga *noise filtering*. Minggu ini, kita akan membahas salah satu algoritma yang umum digunakan untuk reduksi dimensi, yaitu Principal Component Analysis (PCA).

<!-- ## Tugas 3
[Notebook Tugas 3](https://nbviewer.jupyter.org/github/aliakbars/uai-dm/blob/master/scripts/tugas3.ipynb)

Dalam tugas ini, Anda diminta untuk melakukan klasifikasi dan *clustering* dengan menggunakan algoritma k-Nearest Neighbours dan k-Means. Anda juga akan melihat efek dari penerapan reduksi dimensi dengan Principal Component Analysis terhadap hasil klasifikasi dan *clustering*. Tugas ini dikumpulkan melalui situs e-learning UAI.

!!! warning "Tenggat"
    Sabtu, 27 Mei 2017, pukul 23.55 WIB -->

## Analisis Keranjang Belanja

Materi minggu ke-12 akan diisi oleh Ir. Endang Ripmiatin, M.T.

## Sistem Rekomendasi

[Salindia minggu ke-13: Sistem Rekomendasi](https://github.com/aliakbars/uai-dm/raw/master/13-recsys.pdf)

Materi ini dapat dianggap sebagai salah satu implementasi dari semua materi yang telah diberikan sebelumnya. Kita akan mengulas kembali konsep jarak antarobjek, klasifikasi, *clustering*, dan reduksi dimensi dalam membuat sistem rekomendasi. Materi ini sekaligus jadi materi terakhir dalam kuliah ini. Silakan baca lebih lanjut di buku Mining of Massive Datasets pada Chapter 9 untuk tahu detailnya.

<!-- ## Tugas 4

[Notebook Tugas 4](https://nbviewer.jupyter.org/github/aliakbars/uai-dm/blob/master/scripts/tugas4.ipynb)

[Dataset Tugas 4: Movies](https://github.com/aliakbars/uai-dm/raw/master/dataset/ml/movies.csv)

[Dataset Tugas 4: Ratings](https://github.com/aliakbars/uai-dm/raw/master/dataset/ml/ratings.csv)

[Dataset Tugas 4: Tags](https://github.com/aliakbars/uai-dm/raw/master/dataset/ml/tags.csv)

Tugas kali ini merupakan gabungan materi dari beberapa kuliah sebelumnya. Anda diminta untuk membangun dan membandingkan beberapa metode sistem rekomendasi. Tugas ini dikumpulkan melalui situs e-learning UAI.

!!! warning "Tenggat"
    Rabu, 21 Juni 2017, pukul 23.55 WIB -->