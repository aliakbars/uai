# Image Classification Service

**Kesulitan**: sedang

**Keahlian terkait**: web service, machine learning

**Pustaka terkait**:

* [Flask](http://flask.pocoo.org/)
* [Flask-RESTful](https://flask-restful.readthedocs.io/en/0.3.5/)
* [Keras](https://keras.io/)
* [TensorFlow](https://www.tensorflow.org/)

## Deskripsi

Metode untuk melakukan deteksi objek maupun klasifikasi citra sudah sangat banyak
dan mumpuni. Dengan pustaka seperti Keras, tugas tersebut dapat dilakukan dengan
mudah. Bahkan, [salah satu juara Go-Hackathon](https://go-hackathon.hackerearth.com/sprints/go-hackathon/dashboard/QuantumSigmoid/idea/)
yang diadakan Go-Jek beberapa waktu yang lalu membangunnya sendiri dengan menggunakan TensorFlow.

Yang perlu Anda buat dalam proyek ini persis seperti yang mereka kerjakan dalam
waktu kurang lebih 24 jam. Dengan data gambar yang bisa Anda cari melalui internet,
Anda dapat mengklasifikasikan gambar makanan, kucing, hingga digit angka dengan
mudah. Kode untuk klasifikasi yang lebih canggih pun disediakan dalam repositori
Github milik Keras. Anda hanya perlu membungkusnya dalam bentuk *web service*
sehingga pengguna awam dapat mengunggah gambar dan langsung mendapatkan hasil
klasifikasinya. Lebih bagus lagi kalau Anda bisa membuatnya secara *real-time*.
