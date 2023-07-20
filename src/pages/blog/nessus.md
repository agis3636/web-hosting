---
templateKey: blog-post
title: Sekilas Tentang Nessus, Apa itu Nessus ?
date: 2022-08-13T00:00:00.000Z
featuredpost: false
featuredimage: /img/nessus.png
description: Nessus adalah sebuah aplikasi dari Tenable Security
tags:
  - Nessus adalah
  - nessus
  - aplikasi Tenable Security
  - Sekilas Tentang Nessus
  - melihat vulnerability didalam network
---

Nessus adalah sebuah aplikasi dari Tenable Security untuk melihat vulnerability didalam network.
Aplikasi Nessus adalah client server based, merupakan system pengecekan vulnerability. Nessus bisa di download di www.nessus.org

Nessus akan melakukan scanning ke computer yang dituju untuk mengetahui port port mana yang terbuka dan vulnerability yang ada sekaligus melaporkan bila ada issue yang terkait dengan hal itu.

Proses pengecekannya dihubungkan dengan Nessus server, oleh karena itu Nessus selalu dilengkapi dengan pengetahuan vulnerability terkini.

![Nessus](/img/Nessus3.png)

Fitur fitur Nessus antara lain :

- Database security Nessus diupdate setiap hari ketika konek server Nessus.
- Nessus mampu mendeteksi tidak cuma port port yang terbuka di setiap computer yang terhubung kedalam jaringan, tetapi juga mengecek patch patch OS nya termasuk didalamnya pacth untuk Windows, Unix, Linux atau MacOS.
- Nessus bisa dibangun dalam skala kecil, satu atau dua computer dengan sedikit resource prossesor sampai dengan prosessor dengan quad core lebih. Semakin diberikan “power” ke Nessus maka semakin cepat pula task akan diselesaikan.
- Setiap security test di bentuk dalam modul plugin dan ditulis dalam NASL, artinya update nessus tidak akan melibatkan binaries yang tidak dipercaya dari Internet.
- Setiap NASL plugin dapat dibaca , di modifikasi agar report Nessus bisa dibaca dengan lebih mudah.
- NASL ( Nessus Attack Scripting Language) suatu Bahasa yang dikembankan khusus agar security test dapat dijalankan dengan mudah dan cepat.
- NASL plugin didalam suatu container yang bisa berdiri diatas virtual mesin sehingga membuat Nessus menjadi scanner yang benar benar secure.
- Nessus memiliki kemampuan untuk mengetest SSL seperti https, smptps, imaps dll, dan dapat pula di itegrasikan dengan certificate.




Ketika kita menjalankan Nessus maka ada 3 ( tiga) tahap yaitu :

1. Scanning
   
   Pada fase ini nessus akan melakukan pengecekan untuk mengetahui mana mana host yang hidup ( live), dengan cara mengirimkan ICMP Echo. Kemudian selanjutnya bisa host tersebut diketahui live akan diteruskan dengan port scanning.

2. Enumeration
   
   Pada tahap ini nessus akan melakukan pemeriksaan kepada host yang live dengan mencari banner grabbing yang bisa menunjukkan jenis, type dan versi OS yang digunakan oleh host. Tergantung dari sistemnya difase ini dimungkinkan untuk melakukan test penjebolan account dan password dengan metode brute force.

3. Deteksi Vulnerabilty
   
   Setelah fase 2 selesai maka nessus akan melanjutkan dengan mencari vulnerability yang sesuai yang terdapat pada host target misalanya input validasi, buffer overflows,konfigurasi yang tidak tepat dll.


Sampai dengan saat ini Nessus sudah memiliki versi 6.0. Untuk typenya ada 3 tipe yang ditawarkan yaitu `tipe cloud`, `tipe on premises` dan `tipe on your laptop`, semuanya memiliki ke untungan masing masing, tinggal disesuaikan kebutuhannya.
Tentunya harga pun menyesuaikan dengan besarnya jumlah IP yang akan di scan dengan Nessus.

Ada satu lagi tipe yang bisa digunakan meskipun dengan jumlah maksimum IP adalah 16, yaitu Nessus Home dan tanpa batasan waktu , tipe ini bisa digunakan untuk mengetahui bagaimana Nessus ini bekerja. Silahlan download Nessus Home di link berikut ini : http://www.tenable.com/products/nessus/select-your-operating-system?gclid=CNakkMy20cwCFQqBvQodiyYOHQ.



    Demikian dapat saya sampaian untuk kesempatan kali ini semoga bermanfaat.