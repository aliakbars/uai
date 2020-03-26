description: Kebutuhan untuk mengolah dan mengambil pengetahuan dari big data menjadi topik yang sedang hangat dibicarakan industri. Kuliah ini mengajarkan berbagai algoritma machine learning seperti naives bayes, nearest neighbor, linear regression, k-means, serta penerapannya untuk kasus natural language processing dan computer vision.

# Pengenalan Pola

## Pendahuluan

Ada baiknya untuk sedikit mengulas materi aljabar linear, kalkulus, dan statistika Anda sebelum memulai kuliah ini. Beberapa orang merekomendasikan untuk belajar dari bagian pertama buku [Deep Learning](http://www.deeplearningbook.org/) yang ditulis oleh Ian Goodfellow dkk. Untuk pemahaman lebih lanjut, Anda juga bisa melihat materi probabilitas untuk ilmu komputer yang sangat menarik di kuliah Stanford [CS109: Probability for Computer Scientists](http://web.stanford.edu/class/cs109/index.html).

!!! info "Referensi"
    Kuliah ini banyak mengadaptasi materi dari [Introductory Applied Machine Learning](http://www.inf.ed.ac.uk/teaching/courses/iaml/) dan [Machine Learning & Pattern Recognition](http://www.inf.ed.ac.uk/teaching/courses/mlpr/) dari the University of Edinburgh, serta [CS229: Machine Learning](http://cs229.stanford.edu/) dari Stanford University.

Beberapa materi kuliah ini juga diadaptasi dari kuliah [Data Mining](http://uai.aliakbars.com/data-mining/). Namun, alur penyampaian kuliah akan sedikit diubah. Selain itu, contoh-contoh kasusnya akan lebih banyak berkaitan dengan masalah-masalah dalam *computer vision*.

Anda dapat membuat *clone* dari repositori mata kuliah ini di [sini](https://github.com/aliakbars/uai-mlpr).

!!! tip "Pre-test"
    Coba soal latihan [ini](https://github.com/aliakbars/uai-dm/raw/master/latihan-0.pdf) untuk mengetahui apakah Anda punya cukup pengetahuan untuk mengikuti kelas ini atau tidak.

## Konsep Probabilistik dalam Pengenalan Pola

[Salindia minggu ke-1: Pendahuluan](https://github.com/aliakbars/uai-mlpr/raw/master/01-intro.pdf)

Apa hubungannya *data mining*, *machine learning*, dan pengenalan pola? Uraian singkat mengenai materi yang akan dipelajari selama kuliah ini akan disampaikan pada pertemuan pertama perkuliahan. Anda diminta proaktif dalam mencari materi tambahan untuk belajar lebih banyak lagi.

[Salindia minggu ke-2: Probabilitas](https://github.com/aliakbars/uai-mlpr/raw/master/02-probability.pdf)

Di minggu ini, kita akan membahas tentang konsep peluang, peubah acak, dan beberapa materi lainnya yang berkaitan dengan ketidakpastian yang akan membantu untuk memahami materi-materi di beberapa pertemuan berikutnya. Sangat disarankan bagi Anda untuk melihat kuliah Stanford CS109 dan [Harvard Stats 110](https://www.youtube.com/watch?v=KbB0FjPg0mw&list=PL2SOU6wwxB0uwwH80KTQ6ht66KWxbzTIo).

[Salindia minggu ke-3: Distribusi Diskrit](https://github.com/aliakbars/uai-mlpr/raw/master/03-discrete.pdf)

[Salindia minggu ke-4: Distribusi Kontinu](https://github.com/aliakbars/uai-mlpr/raw/master/04-kontinu.pdf)

Sebagi dasar untuk masuk ke materi berikutnya tentang Naive Bayes, di minggu ini kita akan membahas beberapa jenis distribusi yang akan sering dijumpai untuk pemodelan data. Anda akan belajar untuk mengestimasi nilai parameter dari suatu distribusi yang dapat menjelaskan data dengan baik (Maximum Likelihood Estimation). Gunakan [SciPy](https://www.scipy.org/) untuk melakukan pemodelan probabilistik dari contoh-contoh data yang tersedia, misalnya [data menu McDonald's](https://github.com/aliakbars/uai-dm/blob/master/dataset/menu.csv).

!!! tip "Soal Latihan Probabilitas dan Statistika"
    Silakan coba kerjakan soal yang telah saya kurasi di [sini](https://docs.google.com/document/d/19eJuNJJvCIl_ssjAaNLyeflKTqytlTC5frsUzpVL41Q/edit?usp=sharing). Kunci jawaban dapat diminta setelah Anda menunjukkan hasil pekerjaan Anda.

## Tugas 1

[Notebook Tugas 1](https://colab.research.google.com/github/aliakbars/uai-mlpr/blob/master/scripts/tugas1b.ipynb)

Dalam tugas ini, Anda akan melakukan eksplorasi data dan pemilihan model dari data konsumsi bensin mobil.

!!! warning "Tenggat"
    Kamis, 19 Maret 2020, pukul 23.55 WIB

[Salindia minggu ke-5: Naive Bayes](https://github.com/aliakbars/uai-mlpr/raw/master/05-nb.pdf)

[Video minggu ke-5: Naive Bayes](https://www.youtube.com/watch?v=IKG_HcOdhEs)

[Praktikum 1: Distribusi Gaussian dan Naive Bayes](https://colab.research.google.com/github/aliakbars/uai-mlpr/blob/master/scripts/lab1.ipynb)

Memanfaatkan konsep yang sudah dipelajari minggu lalu, minggu ini kita akan melihat bagaimana berbagai distribusi tersebut dapat digunakan untuk melakukan klasifikasi. Pelajari multivariate Gaussian dan Bernoulli distribution secara lebih intensif untuk bisa memahami materi ini.

## Dimensionality Reduction

[Salindia minggu ke-6: Dimensionality Reduction](https://github.com/aliakbars/uai-mlpr/raw/master/06-dim.pdf)

[Video minggu ke-6: Naive Bayes](https://www.youtube.com/watch?v=Qq9v4AyTdAo)

Dalam multivariate Gaussian, Anda menghitung matriks kovariansi yang menggambarkan variansi dari tiap variabel dan hubungan antarvariabel. Ingat bahwa dalam kasus MNIST, selalu ada variabel yang tidak pernah berubah nilainya. Jadi, apakah kita masih membutuhkan variabel tersebut? Metode yang akan Anda pelajari di minggu ini akan membantu Anda dalam mereduksi dimensi yang tinggi menjadi beberapa dimensi yang bermakna saja. Untuk melakukan hal tersebut, Anda memerlukan kovariansi matriks yang dihitung tadi.

## Tugas 2

[Notebook Tugas 2](https://colab.research.google.com/github/aliakbars/uai-mlpr/blob/master/scripts/tugas2b.ipynb)

Dalam tugas ini, Anda akan mengulas materi tentang Naive Bayes dan PCA dengan menerapkannya pada dataset wajah.

!!! warning "Tenggat"
    Sabtu, 4 April 2020, pukul 23.55 WIB

<!-- ## Model Linear

[Salindia minggu ke-6: Model Linear](https://github.com/aliakbars/uai-mlpr/raw/master/06-linear.pdf)

Model linear secara umum sudah pernah dibahas di mata kuliah Kecerdasan Buatan. Kali ini, kita akan melihat bagaimana prosesnya untuk bisa mendapatkan solusi dari regresi linear dengan asumsi Gaussian noise. Untuk itu, pelajari kembali materi distribusi Gaussian dan MLE-nya. Selain itu, materi tambahan kali ini adalah regularisasi dan dampaknya ke model yang dihasilkan.

## Evaluasi Model

[Salindia minggu ke-7: Evaluasi Model](https://github.com/aliakbars/uai-mlpr/raw/master/07-eval.pdf)

Apakah model *machine learning* selalu hanya berupa *trial and error*? Pada minggu ini, topik yang akan dibahas adalah bagaimana kita dapat mengevaluasi model dan menentukan perbaikan seperti apa yang dapat dilakukan terhadap model tersebut. Beberapa konsep penting yang akan dibahas antara lain *bias-variance trade-off*, *underfitting*, *overfitting*, dan beberapa metrik yang dapat digunakan untuk mengevaluasi model dalam kasus klasifikasi maupun regresi.



## Neural Networks, k-NN, dan k-Means

Untuk materi empat minggu ini, akan diisi oleh Bapak Firmansyah.

## Tugas 3

Tugas 3 akan diberikan oleh Bapak Firmansyah.

## Gaussian Mixture Models

[Salindia minggu ke-12: Gaussian Mixture Models](https://github.com/aliakbars/uai-mlpr/raw/master/12-gmm.pdf)

setelah mendapat materi tentang k-Means di beberapa pertemuan sebelumnya, kali ini yang dibahas adalah Gaussian Mixture Models yang dapat melakukan *soft clustering*. Materi ini akan berkaitan dengan materi konsep probabilitas dan distribusi yang disampaikan di beberapa pertemuan awal.

## Tugas 4

[Notebook Tugas 4](https://colab.research.google.com/github/aliakbars/uai-mlpr/blob/master/scripts/tugas4.ipynb)

[Dataset Tugas 4](https://github.com/aliakbars/uai-mlpr/raw/master/datasets/bbc.csv)

Dalam tugas ini, Anda akan mencoba melakukan *clustering* dengan menggunakan k-Means dan Gaussian Mixture Models pada dataset artikel berita dari BBC.

!!! warning "Tenggat"
    Minggu, 24 Juni 2018, pukul 23.55 WIB -->