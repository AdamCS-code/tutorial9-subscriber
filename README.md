Nama: Adam Caldipawell Sembiring
Kelas: ADPRO B
NPM: 2306227160

a. Apa itu AMQP?
Jawaban:
AMQP adalah singkatan dari Advanced Message Queuing Protocol. Ini adalah protokol lapisan aplikasi standar terbuka untuk middleware berorientasi pesan. Bayangkan ini sebagai sekumpulan aturan yang memungkinkan berbagai aplikasi perangkat lunak untuk bertukar pesan secara andal dan aman, bahkan jika ditulis dalam bahasa pemrograman yang berbeda atau berjalan di sistem operasi yang berbeda.

Karakteristik utama AMQP meliputi:

* **Berorientasi pesan:** Dirancang khusus untuk mengirim dan menerima pesan.
* **Asinkron:** Pengirim dan penerima tidak harus online pada waktu yang sama. Pesan dapat diantrikan dan dikirim nanti.
* **Andal:** AMQP menyediakan mekanisme untuk memastikan pengiriman pesan, bahkan jika terjadi masalah jaringan atau kegagalan aplikasi.
* **Standar terbuka:** Sebagai standar terbuka, vendor yang berbeda dapat mengimplementasikan broker dan klien AMQP yang dapat beroperasi bersama.

b. Apa arti dari `guest:guest@localhost:5672`? Apa arti `guest` yang pertama, `guest` yang kedua, dan untuk apa `localhost:5672`?
Jawaban:
String `guest:guest@localhost:5672` adalah **URI (Uniform Resource Identifier) koneksi** yang umum digunakan untuk menentukan cara terhubung ke broker AMQP.

* **`guest` (yang pertama):** Ini adalah **nama pengguna** yang digunakan untuk autentikasi dengan broker AMQP. Dalam banyak pengaturan default atau pengembangan, "guest" adalah nama pengguna default yang umum.

* **`guest` (yang kedua):** Ini adalah **kata sandi** yang terkait dengan nama pengguna yang digunakan untuk autentikasi. Sekali lagi, "guest" sering kali menjadi kata sandi default untuk pengguna "guest" dalam lingkungan pengembangan. 

* **`localhost:5672`:** Ini menentukan **alamat jaringan** dari broker AMQP:
    * **`localhost`:** Ini merujuk ke mesin lokal tempat kode berjalan. Ini berarti broker AMQP diharapkan berjalan di komputer yang sama.
    * **`5672`:** Ini adalah **nomor port** di mana broker AMQP mendengarkan koneksi masuk. Secara konvensi, 5672 adalah port standar untuk AMQP.

**Singkatnya, `guest:guest@localhost:5672` memberi tahu aplikasi Rust Anda untuk terhubung ke broker AMQP yang berjalan di mesin yang sama (`localhost`) pada port 5672, menggunakan nama pengguna "guest" dan kata sandi "guest" untuk autentikasi.**
