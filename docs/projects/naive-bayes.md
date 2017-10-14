# Modul Naive Bayes Tambahan

**Kesulitan**: sukar

**Keahlian terkait**: aljabar linear, probabilitas & statistik, machine learning

**Pustaka terkait**:

* [NumPy](http://www.numpy.org/)
* [SciPy](https://www.scipy.org/)
* [scikit-learn](http://scikit-learn.org/stable/)

## Deskripsi

Berdasarkan dokumentasi scikit-learn untuk Naive Bayes, dapat dilihat bahwa
terdapat tiga jenis distribusi yang umum digunakan, yaitu Bernoulli, Multinomial,
dan Gaussian. Ketiga jenis distribusi tersebut disesuaikan dengan tipe data yang
ditangani, e.g. Bernoulli untuk boolean, Multinomial untuk data pencacahan, dan
Gaussian untuk numerik. Namun, scikit-learn baru bisa mengerjakan satu untuk semua.
Dengan kata lain, jika dalam satu *dataframe* ternyata ada beberapa tipe data,
semua akan dianggap sebagai satu tipe.

Hal ini berbeda dengan [Weka](http://www.cs.waikato.ac.nz/ml/weka/) yang memungkinkan
penggunanya untuk mendefinisikan sekaligus mengubah tipe data dari tiap-tiap atribut.
Tugas Anda adalah membuat modul tambahan yang dapat mengakomodasi perbedaan tipe data
dari suatu *dataframe* tersebut. Akan lebih bagus lagi jika Anda bisa memberikan
pilihan distribusi tambahan, misalnya Poisson atau Kernel Density Estimation (KDE).
