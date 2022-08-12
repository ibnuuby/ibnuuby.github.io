---
title: "Cara Mendapatkan Free SSL di Cloudflare"
author: Ibnu Ubaeydillah
layout: post
comments: true
permalink: /Cara-Mendapatkan-Free-SSL-di-Cloudflare/
categories: Genel
tags: [linux, all-post]
---

Halo semuanya, sebenarnya tulisan yang saya buat ini adalah masalah yang saya alami, yaitu salam membeli domain. Ya domain yang saya beli ternyata belum terdapat SSLnya. Tetapi saya bersyukur dengan terjadinya masalah yang saya alami ini. Saya mendapatkan ilmu baru yaitu [Cara Mendapatkan Free SSL di Cloudflare](#). Oke sebelum memulai pembahasan cara mendapatkan SSL secara gratis, terlebih dahulu kita harus pahami apa itu SSL?

[SSL](https://sis.binus.ac.id/2019/06/04/pengertian-dan-fungsi-secure-socket-layer-ssl) adalah cara untuk sebuah website untuk membangun koneksi yang aman [terenkripsi](#) antara webserver (website) dengan client (Browser) atau antara mail server dengan mail client. Sehingga koneksi antara client dan server dapat berjalan secara aman dari pihak lain yang tidak berkepentingan. Jadi setiap kali pengujung web mengunjungi situs yang menggunakan SSL maka akan terciptanya sebuah link yang <b>terenkripsi</b>
sehingga jauh lebih aman. lalu bagaimana cara membedakan website yang sudah menggunakan SSL atau belum.
<br>(ref//https://sis.binus.ac.id/2019/06/04/pengertian-dan-fungsi-secure-socket-layer-ssl/)

Untuk membedakannya bisa dilihat dari link website tersebut, website yang sudah menggunakan SSL maka akan membuanyai link website seperti ini [http://namadomain.com/](#) dan jika website tersebut belum menggunakan SSL linknya akan seperti ini [https://namadomain.com/](#). jadi yang membedakannya adalah huruf ['S'](#). 

Baik langsung saya mulai saja bagaimana cara mendapatkan free ssl di cloudflare, yang pertama kalian harus menyiapkan terlebih dahulu domain yang ingin kalian pakai, untuk domainnya yang belum menggunakan SSL ya. setelah kalian mempunyai domain yang ingin di terapkan SSL maka kalian harus membuat terlebih dahulu akun Cloudflare, untuk link pendaftarannya bisa [disini](https://dash.cloudflare.com/sign-up).

<img src="https://user-images.githubusercontent.com/28418984/181007412-a6eed80b-a750-488c-bd10-8b94067f0611.png">
Setelah berhasil daftar akun cloudflare, silakan pilih menu [add site](#) untuk menambahkan website kamu.
<img src="https://user-images.githubusercontent.com/28418984/181010238-5d2fc473-c7b8-4076-85ae-481480f78be9.png">
Setelah menambahkan situs, kamu akan diarahkan untuk memilih plan yang ada di Cloudflare.
Scroll ke bagian paling bawah, pilih yang [Free $0](#), kemudian klik [Continue](#).
<img src="https://sekolahblogger.com/wp-content/uploads/2021/10/free-plan-cloudflare.webp">
Kemudian sistem Cloudflare akan melakukan scanning terhadap domain Anda, tunggu sampai prosesnya selesai lalu klik [Continue](#)
<img src="https://sekolahblogger.com/wp-content/uploads/2021/10/menambahkan-dns-baru-pada-cloudflare.webp">
Selanjutnya, Anda akan diminta untuk mengganti nameserver domain Anda dengan name server milik Cloudflare.
<img src="https://sekolahblogger.com/wp-content/uploads/2021/10/mengganti-nameserver-cloudflare.webp">
Silahkan ikuti langkah-langkah yang diberikan Coudflare
- Login ke provider [domain Anda](#)
- [Hapus nameserver](#) yang Anda pakai sekarang
- [Ganti](#) dengan [nameserver Cloudflare](#)
- Klik [Done](#), check nameserver
Proses propagasi ini membutuhkan waktu antara 24-48 jam, tapi biasanya bisa lebih cepat.
Setelah itu, Anda akan diarahkan ke halaman konfigurasi domain yang baru Anda tambahkan tadi.
Ada 3 konfigurasi yang perlu Anda sesuaikan.
- [Improve security](#)
- [Optimize performance](#)
- [Summary](#)
<br>Pada bagian Improve security, pastikan toggle Automatic HTTPS Rewrites-nya Anda geser ke kanan sampai berwarna hijau, seperti gambar di bawah ini, kemudian klik [Save](#)
<img src="https://sekolahblogger.com/wp-content/uploads/2021/10/automatic-https-rewrites-on-cloudflare.webp">
Lakukan hal yang sama pada section Always Use HTTPS, pastikan tonggle nya berwarna hijau. Kemudian [klik Save](#).
<img src="https://sekolahblogger.com/wp-content/uploads/2021/10/always-use-https-on-cloudflare.webp">
Pada bagian Optimize Performance, ada dua konfigurasi yang harus Anda sesuaikan, Auto Minify dan Brotli.
Lakukan hal yang sama pada bagian ini seperti proses sebelumnya, pastikan Anda mengaktifkan semuanya [toggle berwarna hijau](#).
<img src="https://sekolahblogger.com/wp-content/uploads/2021/10/auto-manify-configuration-on-cloudflare.webp">
<img src="https://sekolahblogger.com/wp-content/uploads/2021/10/brotli-configuration.webp">
Pada bagian Summary, [klik Finish](#).
Dan selesai. Situs Anda sekarang sudah dipasangi SSL dan [sudah aman](#).
<img src="https://sekolahblogger.com/wp-content/uploads/2021/10/situs-sudah-terlindungi-oleh-cloudflare.webp">
Proses ini membutuhkan waktu antara 24-48 jam, Anda bisa mengeceknya secara berkala.



