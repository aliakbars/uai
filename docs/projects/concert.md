# Sistem Pengelolaan Panitia Konser

**Kesulitan**: mudah

**Keahlian terkait**: web dinamis, web service

**Pustaka terkait**:

* [Flask](http://flask.pocoo.org/)
* [Django](https://www.djangoproject.com/)

## Deskripsi

Bayangkan Anda sedang berada dalam sebuah konser yang berformat festival.
Umumnya, konser seperti itu akan memiliki sejumlah panitia. Di luar panitia
yang jumlahnya terkadang bisa mencapai ratusan tersebut, masih ada pula
*tenants* yang perlu keluar-masuk dari area konser.

Untuk memudahkan proses identifikasi orang yang keluar-masuk area konser,
maka diperlukan sebuah sistem yang dapat memeriksa status setiap orang
yang didaftarkan. Jadi, sistem ini akan menyimpan data dari masing-masing
orang yang berkepentingan, lalu mencatat juga status terakhir orang tersebut,
di dalam atau di luar area, serta waktu orang tersebut keluar atau masuk.
