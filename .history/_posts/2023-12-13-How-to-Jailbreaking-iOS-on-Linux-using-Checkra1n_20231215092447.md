---
title: "How to Jailbreaking iOS on Linux using Checkra1n"
author: Ibnu Ubaeydillah
layout: post
comments: true
permalink: /How-to-Jailbreaking-iOS-on-Linux-using-Checkra1n/
tags: [all-post]
---

``Jailbrake IOS`` adalah sebuah proses menghilangkan batasan yang diberlakukan oleh Apple pada perangkat genggam dengan sistem operasi iOS, yakni iPhone, iPod Touch, iPad dan Apple TV generasi ke-2. Menjebol kungkungan akan membuat sang pengguna bisa mendapatkan akses penuh (atau akses akar) terhadap sistem operasi, yang darinya pengguna iOS itu bisa mengunduh perangkat lunak, baik yang bajakan ataupun yang orisinal namun tidak tersedia di Apple App Store. 
(source//https://id.wikipedia.org/wiki/Jailbreaking_di_iOS). 
<br>

<center>
<img src="{{ site.url }}{{ site.baseurl }}/assets/images/iphone-jailbreak.jpeg">
</center>

Beberapa tahun yang lalu, proses jailbreak dianggap kompleks, tetapi saat ini, dengan hadirnya berbagai alat bantu, seperti Checkra1n, proses tersebut menjadi lebih mudah dan dapat dilakukan oleh pengguna awam.

Checkra1n disebut sebagai semi-tethered jailbreak, yang memungkinkan pengguna untuk melakukan jailbreak pada perangkat iOS mereka. Dalam jenis jailbreak ini, pengguna perlu menjalankan kembali proses jailbreak setiap kali perangkat dimatikan atau restart. Meskipun demikian, proses ini dijelaskan sebagai mudah dan sederhana, dapat dilakukan oleh pengguna awam.

Teks tersebut juga menyoroti bahwa Checkra1n dapat digunakan di sistem operasi Linux, memberikan panduan cara melakukan jailbreak menggunakan alat tersebut. Kelebihan yang disorot melibatkan kemudahan dan praktisitas dalam melakukan jailbreak tanpa memerlukan perangkat tambahan atau proses yang rumit.

Selain itu, penekanan pada manfaat jailbreak termasuk kemampuan pengguna untuk mengoptimalkan sistem operasi dan melakukan modifikasi pada perangkat iOS sesuai kebutuhan mereka. Dengan demikian, tutorial tersebut memberikan informasi tentang cara menggunakan Checkra1n di Linux untuk memudahkan pengguna iPhone dalam melakukan jailbreak dan mempersonalisasi perangkat mereka.

<h1>Install Checkra1n</h1>

``` 
wget -O - https://assets.checkra.in/debian/archive.key | gpg --dearmor | sudo tee /usr/share/keyrings/checkra1n.gpg >/dev/null
echo 'deb [signed-by=/usr/share/keyrings/checkra1n.gpg] https://assets.checkra.in/debian /' | sudo tee /etc/apt/sources.list.d/checkra1n.list
sudo apt-get update
sudo apt-get install checkra1n
```
bila tidak bisa install checkra1n menggunakan perintah ``sudo apt-get install checkra1n``, kalian bisa menginstall secara manual dengan cara berikut ini:

```
Buka link ini https://checkra.in/releases/#all-downloads
Pilih Download for linux
```

Setelah file checkra1n berhasil di download, selanjutnya kalian, jalankan perintah ``chmod +x ./checkra1n``, setelah itu jalankan perintah ``./checkra1n``. maka chekra1n akan otomatis dijalankan.  

<center>
<img src="{{ site.url }}{{ site.baseurl }}/assets/images/checkra1n-1.png">
</center>

Selanjutnya pilih ``Start`` dan Enter. owh iya jangan lupa kalian harus menghubungkan iphone dengan menggunakan kabel USB terlebih dahulu ya sebelum menjalakan ``checkra1n`` ini.

Selanjutnya checkra1n akan membuat iPhone kita masuk ke recovery mode.

<center>
<img src="{{ site.url }}{{ site.baseurl }}/assets/images/checkra1n-2.png">
</center>

Selanjutnya kita akan diinstruksikan untuk masuk ke DFU mode. Tinggal pilih Start, Enter, lalu ikuti saja instruksi dari checkra1n.

<center>
<img src="{{ site.url }}{{ site.baseurl }}/assets/images/DFU-Mode.png">
</center>

Sampai proses ini kalian tinggal tunggu saja prosesnya sampai selesai.
<center>
<img src="{{ site.url }}{{ site.baseurl }}/assets/images/jalikbreaking.png">
</center>


Setelah semua selesai, cabut kabel USB. Lalu di iOS kalian akan muncul aplikasi checkra1n. Tinggal buka aplikasi tersebut lalu install Cydia. mungkin sampai sekian tulisan ini, tulisan ini akan terus di update bilamana disuatu hari nanti ada update terbaru.
``Terima kasih`` 