description: Kecerdasan buatan, inteligensi buatan, atau artificial intelligence sedang menarik perhatian banyak orang saat ini. Kuliah ini membahas berbagai aspek AI, mulai dari machine learning, neural networks/deep learning, reinforcement learning, searching, dynamic programming, hingga game theory.

# Artificial Intelligence

## Pendahuluan

Kecerdasan buatan, inteligensi buatan, atau *artificial intelligence* (AI) sedang mengambil perhatian orang dalam beberapa tahun terakhir. Hal ini salah satunya disebabkan oleh peningkatan kemampuan komputasi yang berdampak pada berkembangnya penggunaan algoritma *artificial neural networks* (ANN atau NN) yang kini juga populer dengan nama *deep learning*. Namun, penggunaan algoritma pembelajaran mesin (*machine learning*) secara umum sejatinya telah mengubah pandangan klasik terhadap solusi untuk berbagai permasalahan. Kuliah ini dirancang untuk mengenalkan Anda pada berbagai algoritma AI secara umum dan kegunaannya dalam kasus yang dekat dengan keseharian Anda.

!!! info "Referensi"
    Kuliah ini mengikuti alur penyampaian materi dari [CS221: Artificial Intelligence: Principles and Techniques](http://web.stanford.edu/class/cs221/) dari Stanford University. Karena kedekatan materi, beberapa materi juga diadaptasi dari [CS154: Artificial Intelligence](http://courses.cms.caltech.edu/cs154/) dari Caltech.

Kuliah ini akan menggunakan Python dan/atau Java sebagai bahasa pengantarnya. Jadi, bagi Anda yang masih belum familiar dengan Python, silakan cek [tutorial singkat untuk Python dan Numpy](http://cs231n.github.io/python-numpy-tutorial/). Sangat disarankan bagi Anda yang masih mengalami kesulitan dengan pendekatan matematis untuk menguatkan kemampuan pemrograman Anda agar dapat mengikuti kecepatan penyampaian materi di kelas.

!!! info "Referensi"
    Anda yang telah familiar dengan Java mungkin juga bisa membuka materi kuliah [Pemrograman Python](/python).

Anda dapat membuat *clone* dari repositori mata kuliah ini di [sini](https://github.com/aliakbars/uai-ai).

## Pengenalan Inteligensi Buatan

[Salindia minggu ke-1: Pengenalan Inteligensi Buatan](https://github.com/aliakbars/uai-ai/raw/master/01-intro.pdf)

[Catatan minggu ke-1](https://github.com/aliakbars/uai-ai/raw/master/notes-01.pdf)

"Apa itu Artificial Intelligence?" Meski banyak yang sudah mendengar namanya, tapi ternyata tidak banyak yang menyadari bahwa inteligensi buatan sudah menjadi bagian dari keseharian kita. Google yang Anda gunakan hampir setiap hari itu terdiri dari berbagai komponen cerdas yang dibangun oleh para insinyur di dalamnya. Ada beberapa pertanyaan filosofis tentang inteligensi buatan yang juga akan dicoba dijawab dalam pertemuan ini. Pertemuan ini akan menjelaskan lebih lengkap tentang alur penyampaian materi kuliah ini selama satu semester ke depan.

## Regresi dan Optimasi

[Salindia minggu ke-2: Regresi Linear](https://github.com/aliakbars/uai-ai/raw/master/02-regresi.pdf)

[Catatan minggu ke-2](https://github.com/aliakbars/uai-ai/raw/master/notes-02.pdf)

Inteligensi pada tingkatan paling rendah adalah model yang diberikan kemampuan refleks. Salah satu cara untuk membentuk model tersebut adalah dengan melihat tugas yang dihadapi sebagai masalah regresi. Materi ini membahas bagaimana kita bisa memprediksi suatu nilai numerik berdasarkan nilai-nilai lain yang diketahui, misalnya mencari nilai *likes* di Facebook berdasarkan jumlah *share* dan komentar suatu pos. Proses pencarian model yang optimal tersebut juga akan dibahas dalam pertemuan kali ini. *Time to brush up your calculus and linear algebra skills!*

!!! info "Referensi"
    Untuk materi aljabar linear, Anda dapat membaca buku *Deep Learning* (Goodfellow et al., 2016) [Chapter 2](http://www.deeplearningbook.org/contents/linear_algebra.html).

[Salindia minggu ke-3: Klasifikasi: Regresi Logistik](https://github.com/aliakbars/uai-ai/raw/master/03-klasifikasi.pdf)

[Catatan minggu ke-3](https://github.com/aliakbars/uai-ai/raw/master/notes-03.pdf)

Bagaimana kalau yang ingin kita prediksi nilainya berupa kategori? Misalnya, jika diberikan suatu teks, apakah teks tersebut spam atau bukan? Setelah berkutat dengan data numerik, kita akan mengeksplorasi penggunaan model linear lebih lanjut untuk melakukan klasifikasi. Berbeda dengan regresi linear, regresi logistik menggunakan metode optimasi yang berbeda, optimasi numerik. Oleh karena itu, kita akan belajar lebih lanjut tentang metode *gradient descent*.

## Melatih Model Linear

[Salindia minggu ke-4: Training vs Testing](https://github.com/aliakbars/uai-ai/raw/master/04-training.pdf)

Bagaimana cara mengukur bahwa model yang kita buat sebelumnya sudah baik? Apa pula yang dimaksud dengan *hyperparameter tuning*? Kita akan belajar cara untuk mengestimasi error general dengan membagi data menjadi data latih, validasi, dan uji. Anda juga akan dikenalkan dengan beberapa metrik yang dapat dipakai untuk mengevaluasi model yang dihasilkan.

<!-- ## Neural Networks

[Salindia minggu ke-4: Neural Networks](https://github.com/aliakbars/uai-ai/raw/master/04-nets.pdf)

[Catatan minggu ke-4](https://github.com/aliakbars/uai-ai/raw/master/notes-04.pdf)

*Deep learning* yang saat ini sedang populer di banyak tempat berakar pada algoritma *artificial neural networks*. Algoritma ini pun sebetulnya sangat berkaitan erat dengan regresi linear dan logistik. Dengan menggunakan pengembangan dari metode optimasi *gradient descent*, *neural networks* saat ini digunakan untuk berbagai permasalahan pengenalan pola hingga pembuatan model generatif.

Beberapa *framework* yang cukup banyak digunakan dalam bahasa Python untuk mengembangkan neural networks antara lain: [TensorFlow](https://www.tensorflow.org/), [PyTorch](http://pytorch.org/), dan [Caffe2](https://caffe2.ai/). Untuk level abstraksi yang lebih tinggi, mungkin Anda akan tertarik untuk menggunakan [Keras](https://keras.io/) sebagai awal. Keras juga punya versi JavaScript sehingga model yang telah Anda latih di Python dapat dimuat di web dengan [Keras.js](https://transcranial.github.io/keras-js/).

Untuk yang sifatnya lebih teoritis, Anda bisa melihat buku [Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/) (sangat direkomendasikan!) atau buku [Deep Learning](http://www.deeplearningbook.org/). Buku yang terakhir ini juga direkomendasikan bagi Anda yang masih perlu mengulas kembali materi tentang matematika yang dibutuhkan untuk pengembangan algoritma machine learning secara umum. Semua buku ini tersedia secara legal dan gratis di internet. *Do read it if you are interested in this field!* -->

## Tugas 1

[Notebook Tugas 1](https://colab.research.google.com/github/aliakbars/uai-ai/blob/master/scripts/tugas1b.ipynb)

Dalam tugas ini, Anda akan mengeksplorasi regresi linear dan logistik, serta menggunakan neural networks yang didasarkan pada kedua algoritma tersebut.

!!! warning "Tenggat"
    Selasa, 23 Oktober 2018, pukul 23.55 WIB

## Nearest Neighbours

[Salindia minggu ke-5: k-Nearest Neighbours](https://github.com/aliakbars/uai-ai/raw/master/05-knn.pdf)

[Catatan minggu ke-5](https://github.com/aliakbars/uai-ai/raw/master/notes-05.pdf)

Salah satu cara paling alamiah untuk mengambil keputusan bagi kita sebagai manusia adalah dengan bertanya kepada "tetangga". Orang-orang terdekat di sekeliling kita, bagaimana pun cara pengukuran kedekatannya, sering kita jadikan referensi sebelum menggunakan keputusan mayoritas mereka sebagai keputusan pribadi. Ide itu yang juga digunakan dalam algoritma Nearest Neighbours. Pada pertemuan kali ini, Anda akan belajar bagaimana metode ini dapat digunakan dalam kasus regresi maupun klasifikasi.

## Clustering: k-Means

[Salindia minggu ke-6: k-Means](https://github.com/aliakbars/uai-ai/raw/master/06-clustering.pdf)

[Catatan minggu ke-6](https://github.com/aliakbars/uai-ai/raw/master/notes-06.pdf)

Pada pertemuan kali ini, kita akan beralih ke algoritma *machine learning* yang masuk ke dalam kategori *unsupervised learning*. Berbeda dengan beberapa algoritma yang telah kita bahas di pertemuan-pertemuan sebelumnya, algoritma ini tidak membutuhkan label sehingga cara mengevaluasinya juga lebih bervariasi. Untuk kebutuhan mata kuliah ini, kita hanya akan membahas tentang salah satu algoritma untuk melakukan pengelompokan data (*clustering*), yaitu k-Means.

<!-- ## Tugas 2

[Notebook Tugas 2](https://nbviewer.jupyter.org/github/aliakbars/uai-ai/blob/master/scripts/tugas2.ipynb)

Dalam tugas ini, Anda akan mengeksplorasi penggunaan k-NN untuk klasifikasi dan regresi, serta melakukan *clustering* dan klasifikasi dengan memanfaatkan algoritma k-Means untuk gambar angka.

!!! warning "Tenggat"
    Minggu, 19 November 2017, pukul 23.55 WIB -->

## Carian

[Salindia minggu ke-8: Uninformed Search](https://github.com/aliakbars/uai-ai/raw/master/08-search.pdf)

Setingkat di atas refleks, agen cerdas juga perlu untuk memahami *state* dia berada sekarang dan menentukan sekumpulan aksi yang harus diambil agar mencapai tujuannya. Pertemuan ini membahas agen cerdas yang memanfaatkan informasi yang terbatas untuk mencari solusi optimal berupa urutan aksi.

[Salindia minggu ke-9: Informed Search](https://github.com/aliakbars/uai-ai/raw/master/09-search-2.pdf)

Agen cerdas yang dibahas di minggu sebelumnya adalah agen yang "buta". Ini berarti bahwa agen cerdas tersebut tidak mengetahui bahwa terkadang alternatif jalur yang diambil malah menjauhi solusi optimalnya. Materi minggu ini membahas bagaimana kita dapat memperbaiki agen cerdas tersebut dengan memanfaatkan *heuristik*.

<!-- ## Tugas 3

[Deskripsi Tugas 3](https://github.com/aliakbars/uai-ai/raw/master/tugas-3.pdf)

Dalam tugas ini, Anda diminta untuk mengimplementasikan beberapa algoritma carian untuk menyelesaikan kasus-kasus terkait. Tugas ini harus Anda kumpulkan dalam format PDF. Anda hanya perlu membuat kode pada bagian 1. Cantumkan kode tersebut ke dalam file PDF Anda. Dengan kata lain, **tidak ada file untuk source code yang perlu Anda cantumkan**. Anda dapat menggunakan bahasa Java atau Python untuk kode pada bagian 1 tersebut.

!!! warning "Tenggat"
    Sabtu, 16 Desember 2017, pukul 23.55 WIB -->

<!-- ## Proposal Tugas Akhir

[Template Proposal](https://github.com/aliakbars/uai-ai/tree/master/makalah)

Anda diminta untuk membuat sebuah makalah dan poster sebagai pengganti nilai ujian akhir semester (UAS). Untuk kebutuhan tersebut, Anda diminta untuk mengumpulkan proposal penelitian Anda terlebih dahulu. Sebagai gambaran, proposal penelitian Anda ini akan mengandung pendahuluan yang berisi latar belakang dan tujuan penelitian Anda, landasan teori berupa ulasan makalah terkait, dan pengajuan Anda untuk metode yang akan digunakan.

Untuk tugas ini, topik yang Anda pilih disarankan berkaitan dengan materi paruh semester kedua, yaitu **searching, dynamic programming, genetic algorithm, reinforcement learning, Q-learning, game theory,** atau **Bayesian networks**. Jika Anda kesulitan dengan topik tersebut, Anda diperbolehkan mengambil topik *machine learning*, dengan syarat bahwa tingkat kesulitannya akan di atas makalah dengan topik dari materi paruh semester kedua.

Beberapa topik yang menarik untuk diadaptasi antara lain:

- [Congklak with RL](http://ieeexplore.ieee.org/abstract/document/7863309/)
- [MarI/O](https://www.youtube.com/watch?v=qv6UVOQ0F44) & [NEAT](http://nn.cs.utexas.edu/downloads/papers/stanley.ec02.pdf)
- [Atari breakout with Deep Q-learning](https://www.youtube.com/watch?v=V1eYniJ0Rnk)
- [Bayesian Bandits](https://www.chrisstucchio.com/blog/2013/bayesian_bandit.html) & [Multi-armed bandit](https://en.wikipedia.org/wiki/Multi-armed_bandit)
- [AlphaGo](https://deepmind.com/research/alphago/)
- [Alpha-Beta tree search for Checkers](http://www.cs.columbia.edu/~devans/TIC/AB.html)

!!! info "Contoh Poster"
    Contoh poster yang Anda harus buat sebagai bagian dari tugas akhir dapat Anda lihat di [sini](http://cs231n.stanford.edu/reports/2017/posters/). Proposal yang Anda buat nanti akan berukuran kertas A1.

Keterangan lebih lanjut tentang tugas ini akan segera dimuat di situs ini. Silakan cek laman ini secara berkala.

!!! warning "Tenggat Proposal"
    Selasa, 5 Desember 2017, pukul 23.55 WIB -->

## Reinforcement Learning

[Salindia minggu ke-11: Markov Decision Processes](http://web.stanford.edu/class/cs221/2018/lectures/index.html#include=mdp1.js)

[Salindia minggu ke-12: Reinforcement Learning](http://web.stanford.edu/class/cs221/2018/lectures/index.html#include=mdp2.js)

Untuk menjelaskan *reinforcement learning*, silakan merujuk pada salindia dari Stanford University yang tercantum pada tautan di atas. Agen cerdas tipe ini belajar dalam *states* dan ketidakpastian. Ketika suatu aksi yang diambil tidak pasti berujung pada yang diharapkan, kita harus mempertimbangkan kembali aksi yang harus kita ambil agar dapat mengoptimasi solusi yang diharapkan. Untuk materi yang lebih lanjut, Anda juga dapat menyimak video kuliah dari David Silver di [sini](https://www.youtube.com/watch?v=2pWv7GOvuf0).

<!-- ## Tugas Akhir

[Template Makalah](https://www.ieee.org/conferences_events/conferences/publishing/templates.html)

Proposal yang telah Anda ajukan harus diselesaikan dalam bentuk makalah (bisa berbahasa Indonesia maupun Inggris) dengan batasan **minimal 4 halaman dan maksimal 6 halaman** (tidak termasuk daftar pustaka). Makalah tersebut dibuat dalam bentuk dua kolom sesuai standar IEEE. Di samping itu, Anda harus membuat **poster berukuran A1** yang merangkum makalah yang Anda buat. Hindari menulis salinan makalah Anda dalam poster. Anda harus membuat poster tersebut, dengan prioritas secara berurut, **menarik dan informatif**.

!!! info "Pembuatan Poster"
    Anda bisa mengikuti standar yang tertera di [sini](http://web.stanford.edu/class/cs221/project.html#p-poster).

!!! warning "Pengumpulan Makalah dan Poster"
    Makalah dan poster harus Anda buat dalam format PDF dan di-zip. Anda dapat mencantumkan potongan kode dalam file tersebut jika diperlukan. File tersebut dikumpulkan melalui e-learning paling lambat

    Jumat, 19 Januari 2018, pukul 23.55 WIB -->

## Game Playing

[Salindia minggu ke-13: Minimax, expectimax, evaluation functions, alpha-beta pruning](http://web.stanford.edu/class/cs221/2018/lectures/index.html#include=games1.js)

[Salindia minggu ke-14: TD learning, game theory](http://web.stanford.edu/class/cs221/2018/lectures/index.html#include=games2.js)

Di materi sebelumnya, kita sudah membahas bagaimana proses pencarian dalam pohon maupun graf termasuk ketika ada elemen keacakan (*stochasticity*). Bagaimana jika yang dilawan bukan hanya lingkungan saja, tetapi juga lawan yang selalu berusaha meminimalkan keuntungan yang dapat kita raih? Untuk itu, kita perlu memodifikasi kasus yang telah kita pelajari menjadi pohon permainan (*game trees*) sehingga kita dapat menghasilkan solusi yang optimal bagi agen yang kita buat. Materi dalam dua minggu ini juga masih diadaptasi dari CS221 Stanford University.

!!! tip "Video Lectures"
    Untuk membantu pemahaman Anda, Anda bisa melihat contoh lain untuk penjelasan **Alpha-Beta pruning** dari MIT OpenCourseWare di [sini](https://www.youtube.com/watch?v=STjW3eH0Cik).

    Video untuk belajar **Game Theory** bisa dilihat di [channel ini](https://www.youtube.com/user/gametheoryonline).

<!-- ## Tugas 4

[Deskripsi Tugas 4](https://github.com/aliakbars/uai-ai/raw/master/tugas-4.pdf)

Secara umum, tugas ini berhubungan dengan game dan pengambilan strategi terbaik dari game menggunakan Markov Decision Processes dan strategi lainnya. Dalam tugas ini, Anda juga diminta untuk bermain sebuah [game](http://ncase.me/trust) dan menjawab pertanyaan yang diberikan terkait dengan game tersebut. Tugas ini harus Anda kumpulkan dalam format PDF. Anda tidak perlu membuat kode sama sekali.

!!! warning "Tenggat"
    Minggu, 21 Januari 2018, pukul 23.55 WIB -->