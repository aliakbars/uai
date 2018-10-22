description: Aplikasi deep learning dalam berbagai tugas computer vision, natural language processing, dan recommendation system. Diadaptasi dari materi fast.ai dan Stanford CS230: Deep Learning.

# Soft Computing

## Pendahuluan

Kuliah ini akan meminta Anda untuk belajar menggunakan *deep learning* dalam berbagai kasus. Kemampuan pemrograman dalam bahasa Python menjadi syarat bagi Anda untuk dapat mengikuti kuliah ini. Sebagai referensi, Anda direkomendasikan untuk belajar dari buku [Deep Learning](http://www.deeplearningbook.org/) yang ditulis oleh Ian Goodfellow dkk. Buku dari Michael Nielsen tentang [Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/) juga bisa menjadi sumber yang baik.

!!! info "Referensi"
    Kuliah ini banyak mengadaptasi materi dari [fast.ai](http://course.fast.ai/) dan [CS230: Deep Learning](http://cs230.stanford.edu/) dari Stanford University.

Anda dapat membuat *clone* dari repositori mata kuliah ini di [sini](https://github.com/aliakbars/uai-soft-computing).

## Pengenalan Deep Learning

[Salindia minggu ke-1: Pendahuluan](https://github.com/aliakbars/uai-soft-computing/raw/master/01-intro.pdf)

Administrasi kuliah dan beberapa contoh penerapan *deep learning*.

## Model Linear

[Salindia minggu ke-2: Model Linear](https://github.com/aliakbars/uai-soft-computing/raw/master/02-linear.pdf)

Sebelum masuk ke materi *deep learning*, Anda akan dikenalkan pada *building blocks*-nya, yaitu regresi linear dan logistik. Bagaimana Anda dapat melakukan prediksi dengan data yang ada? Anda akan dikenalkan dengan model matematis yang dijadikan dasar dalam metode *deep learning*.

!!! info "Referensi"
    Untuk yang sifatnya lebih praktikal, Anda dapat melihat pendahuluannya di [sini](https://mlbook.explained.ai/intro.html#sec:2.2.9).

    Contoh pencarian solusi tertutup untuk nilai w dapat dilihat di [sini](http://www.cs.cmu.edu/~guestrin/Class/10701-S06/Handouts/recitations/recitation-linear-regression-01-26-2006.pdf).

## Neural Networks

[Salindia minggu ke-3: Neural Networks](https://github.com/aliakbars/uai-soft-computing/raw/master/03-nn.pdf)

Apa hubungannya model linear dengan neural networks? Mengapa pula disebut sebagai *neural networks*?

!!! info "Referensi"
    Sebagai pendahuluan, Anda dapat membaca materi [CS231n](http://cs231n.github.io/neural-networks-1/).

[Salindia minggu ke-4: Generalisation](https://github.com/aliakbars/uai-soft-computing/raw/master/04-generalisation.pdf)

[Lab 1: Multilayer Perceptron](https://colab.research.google.com/github/aliakbars/uai-soft-computing/blob/master/scripts/lab1.ipynb)

Bagaimana cara untuk membuat model neural networks yang *robust*? Apa saja yang dapat dilakukan untuk menghindari *overfitting*?

[Salindia minggu ke-5: Optimisation](https://github.com/aliakbars/uai-soft-computing/raw/master/05-optimisation.pdf)

Materi minggu ini berfokus pada metode yang dapat dilakukan untuk menghasilkan model *deep learning* yang bekerja dengan baik. Anda akan dikenalkan dengan regularisasi L2 dan *batch normalisation*, beberapa fungsi aktivasi baru, serta optimasi model dengan *hyperparameter tuning*.

## Tugas 1

[Notebook Tugas 1](https://colab.research.google.com/github/aliakbars/uai-soft-computing/blob/master/scripts/tugas1.ipynb)

Dalam tugas ini, Anda akan mencoba membuat regresi logistik dengan TensorFlow/Keras dan membandingkan kinerja model *wide* vs *deep learning*.

!!! warning "Tenggat"
    Senin, 29 Oktober 2018, pukul 23.55 WIB