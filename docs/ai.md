# Artificial Intelligence

## Pendahuluan

Inteligensi buatan atau *artificial intelligence* (AI) sedang mengambil perhatian orang dalam beberapa tahun terakhir. Hal ini salah satunya disebabkan oleh peningkatan kemampuan komputasi yang berdampak pada berkembangnya penggunaan algoritma *artificial neural networks* (ANN atau NN) yang kini juga populer dengan nama *deep learning*. Namun, penggunaan algoritma pembelajaran mesin (*machine learning*) secara umum sejatinya telah mengubah pandangan klasik terhadap solusi untuk berbagai permasalahan. Kuliah ini dirancang untuk mengenalkan Anda pada berbagai algoritma AI secara umum dan kegunaannya dalam kasus yang dekat dengan keseharian Anda.

!!! info "Referensi"
    Kuliah ini mengikuti alur penyampaian materi dari [CS221: Artificial Intelligence: Principles and Techniques](http://web.stanford.edu/class/cs221/) dari Stanford University. Selain itu, beberapa materi diadaptasi dari [CS154: Artificial Intelligence](http://courses.cms.caltech.edu/cs154/) dari Caltech.

Kuliah ini akan menggunakan Python dan/atau Java sebagai bahasa pengantarnya. Jadi, bagi Anda yang masih belum familiar dengan Python, silakan cek [tutorial singkat untuk Python dan Numpy](http://cs231n.github.io/python-numpy-tutorial/). Sangat disarankan bagi Anda yang masih mengalami kesulitan dengan pendekatan matematis untuk menguatkan kemampuan pemrograman Anda agar dapat mengikuti kecepatan penyampaian materi di kelas.

!!! info "Referensi"
    Anda yang telah familiar dengan Java mungkin juga bisa membuka materi kuliah [Pemrograman Python](/python).

Anda dapat membuat *clone* dari repositori mata kuliah ini di [sini](https://github.com/aliakbars/uai-ai).

!!! warning "Perhatian"
    Saat ini, masih banyak materi yang berada dalam tahap penulisan. Silakan perbarui repositori Anda secara berkala. Saya sangat terbuka jika ada masukan atau koreksi terhadap materi yang disampaikan.

## Pengenalan Inteligensi Buatan

[Salindia minggu ke-1: Pengenalan Inteligensi Buatan](https://github.com/aliakbars/uai-ai/raw/master/01-intro.pdf)

[Catatan minggu ke-1](https://github.com/aliakbars/uai-ai/raw/master/notes-01.pdf)

"Apa itu Artificial Intelligence?" Meski banyak yang sudah mendengar namanya, tapi ternyata tidak banyak yang menyadari bahwa inteligensi buatan sudah menjadi bagian dari keseharian kita. Google yang Anda gunakan hampir setiap hari itu terdiri dari berbagai komponen cerdas yang dibangun oleh para insinyur di dalamnya. Ada beberapa pertanyaan filosofis tentang inteligensi buatan yang juga akan dicoba dijawab dalam pertemuan ini. Pertemuan ini akan menjelaskan lebih lengkap tentang alur penyampaian materi kuliah ini selama satu semester ke depan.

## Regresi dan Optimasi

[Salindia minggu ke-2: Regresi Linear](https://github.com/aliakbars/uai-ai/raw/master/02-regresi.pdf)

[Catatan minggu ke-2](https://github.com/aliakbars/uai-ai/raw/master/notes-02.pdf)

Inteligensi pada tingkatan paling rendah adalah model yang diberikan kemampuan refleks. Salah satu cara untuk membentuk model tersebut adalah dengan melihat tugas yang dihadapi sebagai masalah regresi. Materi ini membahas bagaimana kita bisa memprediksi suatu nilai numerik berdasarkan nilai-nilai lain yang diketahui, misalnya mencari nilai *likes* di Facebook berdasarkan jumlah *share* dan komentar suatu pos. Proses pencarian model yang optimal tersebut juga akan dibahas dalam pertemuan kali ini. *Time to brush up your calculus and linear algebra skills!*

[Salindia minggu ke-3: Klasifikasi: Regresi Logistik](https://github.com/aliakbars/uai-ai/raw/master/03-klasifikasi.pdf)

[Catatan minggu ke-3](https://github.com/aliakbars/uai-ai/raw/master/notes-03.pdf)

Bagaimana kalau yang ingin kita prediksi nilainya berupa kategori? Misalnya, jika diberikan suatu teks, apakah teks tersebut spam atau bukan? Setelah berkutat dengan data numerik, kita akan mengeksplorasi penggunaan model linear lebih lanjut untuk melakukan klasifikasi. Berbeda dengan regresi linear, regresi logistik menggunakan metode optimasi yang berbeda, optimasi numerik. Oleh karena itu, kita akan belajar lebih lanjut tentang metode *gradient descent*. Ini akan menjadi modal dasar Anda untuk mempelajari materi berikutnya: *neural networks*.

## Neural Networks

[Salindia minggu ke-4: Neural Networks](https://github.com/aliakbars/uai-ai/raw/master/04-nets.pdf)

[Catatan minggu ke-4](https://github.com/aliakbars/uai-ai/raw/master/notes-04.pdf)

*Deep learning* yang saat ini sedang populer di banyak tempat berakar pada algoritma *artificial neural networks*. Algoritma ini pun sebetulnya sangat berkaitan erat dengan regresi linear dan logistik. Dengan menggunakan pengembangan dari metode optimasi *gradient descent*, *neural networks* saat ini digunakan untuk berbagai permasalahan pengenalan pola hingga pembuatan model generatif.

Beberapa *framework* yang cukup banyak digunakan dalam bahasa Python untuk mengembangkan neural networks antara lain: [TensorFlow](https://www.tensorflow.org/), [PyTorch](http://pytorch.org/), dan [Caffe2](https://caffe2.ai/). Untuk level abstraksi yang lebih tinggi, mungkin Anda akan tertarik untuk menggunakan [Keras](https://keras.io/) sebagai awal. Keras juga punya versi JavaScript sehingga model yang telah Anda latih di Python dapat dimuat di web dengan [Keras.js](https://transcranial.github.io/keras-js/).

Untuk yang sifatnya lebih teoritis, Anda bisa melihat buku [Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/) (sangat direkomendasikan!) atau buku [Deep Learning](http://www.deeplearningbook.org/). Buku yang terakhir ini juga direkomendasikan bagi Anda yang masih perlu mengulas kembali materi tentang matematika yang dibutuhkan untuk pengembangan algoritma machine learning secara umum. Semua buku ini tersedia secara legal dan gratis di internet. *Do read it if you are interested in this field!*

## Tugas 1

[Notebook Tugas 1](https://nbviewer.jupyter.org/github/aliakbars/uai-ai/blob/master/scripts/tugas1.ipynb)

[Dataset Tugas 1: Regresi](https://github.com/aliakbars/uai-dm/raw/master/datasets/advertising.csv)

[Dataset Tugas 1: Klasifikasi](https://github.com/aliakbars/uai-dm/raw/master/datasets/food.npy)

[Dataset Tugas 1: Label](https://github.com/aliakbars/uai-dm/raw/master/datasets/food_labels.npy)

Dalam tugas ini, Anda akan mengeksplorasi regresi linear dan logistik, serta menggunakan neural networks yang didasarkan pada kedua algoritma tersebut.

!!! warning "Tenggat"
    Rabu, 18 Oktober 2017, pukul 23.55 WIB

## Nearest Neighbours

[Salindia minggu ke-5: k-Nearest Neighbours](https://github.com/aliakbars/uai-ai/raw/master/05-knn.pdf)

[Catatan minggu ke-5](https://github.com/aliakbars/uai-ai/raw/master/notes-05.pdf)

Salah satu cara paling alamiah untuk mengambil keputusan bagi kita sebagai manusia adalah dengan bertanya kepada "tetangga". Orang-orang terdekat di sekeliling kita, bagaimana pun cara pengukuran kedekatannya, sering kita jadikan referensi sebelum menggunakan keputusan mayoritas mereka sebagai keputusan pribadi. Ide itu yang juga digunakan dalam algoritma Nearest Neighbours. Pada pertemuan kali ini, Anda akan belajar bagaimana metode ini dapat digunakan dalam kasus regresi maupun klasifikasi.

## Clustering: k-Means

[Salindia minggu ke-6: k-Means](https://github.com/aliakbars/uai-ai/raw/master/06-clustering.pdf)

[Catatan minggu ke-6](https://github.com/aliakbars/uai-ai/raw/master/notes-06.pdf)

Pada pertemuan kali ini, kita akan beralih ke algoritma *machine learning* yang masuk ke dalam kategori *unsupervised learning*. Berbeda dengan beberapa algoritma yang telah kita bahas di pertemuan-pertemuan sebelumnya, algoritma ini tidak membutuhkan label sehingga cara mengevaluasinya juga lebih bervariasi. Untuk kebutuhan mata kuliah ini, kita hanya akan membahas tentang salah satu algoritma untuk melakukan pengelompokan data (*clustering*), yaitu k-Means.

## Tugas 2

[Notebook Tugas 1](https://nbviewer.jupyter.org/github/aliakbars/uai-ai/blob/master/scripts/tugas2.ipynb)

Dalam tugas ini, Anda akan mengeksplorasi penggunaan k-NN untuk klasifikasi dan regresi, serta melakukan *clustering* dan klasifikasi dengan memanfaatkan algoritma k-Means untuk gambar angka.

!!! warning "Tenggat"
    Minggu, 19 November 2017, pukul 23.55 WIB