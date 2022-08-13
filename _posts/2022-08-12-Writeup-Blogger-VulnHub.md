---
title: "Writeup Machine Blogger 1 VulnHub"
author: Ibnu Ubaeydillah
layout: post
comments: true
permalink: /Writeup-Machine-Blogger-VulnHub/
tags: [writeup, all-post]
---
Halo temen-temen ini adalah writeup kedua saya, writeup kali ini akan membahas mesin ``Blogger``, mesin tersebut saya ambil dari [Vulnhub](https://www.vulnhub.com/entry/blogger-1,675/). Pada mesin kali ini memiliki vulnerability pada fitur ``post comment`` yang dimana fitur tersebut dapat digunakan untuk mengupload exploit shell kita. Ok baik, kita langsung mulai aja ketulisan selanjutnya. 

<h2>Scan Open Port</h2>
```
nmap -T4 -sC -sV -p- --min-rate=1000 blogger.thm -oN blogger.nmap
```
<img src="https://user-images.githubusercontent.com/28418984/184466224-7e2e39ab-8748-4147-9ffa-6571c28acd07.png">
<h2>Enumerate webserver</h2>
```
dirsearch -u http://blogger.thm/assets/fonts/
```
<br>
<center>
<img src="https://user-images.githubusercontent.com/28418984/184466857-92b4d469-1eeb-464d-b719-ffd2b58f60b1.png">
</center>
<br>kemudian saya cek view source apakah ada informasi yang menarik dan ternyata ada, sistem ini menggunakan ``Wordpress`` ternyata.
```
view-source:http://blogger.thm/assets/fonts/blog/
```
<br>
<center>
<img src="https://user-images.githubusercontent.com/28418984/184466896-45986e80-2128-429c-a1fb-367bdf0810db.png">
</center>
<h2>Enumerate wordpress</h2>
Dikarenakan target menggunakan ``Wordpress`` disini, saya mencoba mengscannya menggunakan ``WPScan``, untuk menemukan informasi apa saja yang di milikinya.
```
wpscan --api-token=$WPSCAN_KEY --url http://blogger.thm/assets/fonts/blog --plugins-detection mixed -e
```
<br>
<center>
<img src="https://user-images.githubusercontent.com/28418984/184467260-b3cd7b66-553a-4835-8608-f16381a8255d.png">
</center>
<br>informasi yang telah saya temukan adalah ``WordPress version 4.9.20`` dan ``Direct Access`` ke ``http://blogger.thm/assets/fonts/blog/wp-content/uploads/`` disini dapat dinyatakan tempat penyimpanan pada sistem disimpan disini dan juga dapat dilakukan ``Direct Access``. Oleh karena itu saya mencoba melakukan proses enumerate lagi terhadap ``Webserver``, ternyata disini ada fitur ``post comment``. 
<img src="https://user-images.githubusercontent.com/28418984/184467364-f6ab4d38-f201-40ef-99c4-6fea91ee1b4c.png">
kemudian saya melakukan ``view source`` pada halaman ``view-source:http://blogger.thm/assets/fonts/blog/?p=29`` dan menemukan sebuah script java script ``<script type='text/javascript' src='http://blogger.thm/assets/fonts/blog/wp-content/plugins/wpdiscuz/assets/js/wpdiscuz-combo.min.js?ver=7.0.4'></script>`` yang di artikan sistem ini menggunakan ``Wpdisquz version 7.0.4`` untuk membuat fitur ``post comment``. 

<h2>Uploading Shell</h2>
Saya mencoba mengupload exploit kedalam fitur ``post comment`` untuk exploitnya sendiri saya ambil dari [https://github.com/pentestmonkey/php-reverse-shell](https://github.com/pentestmonkey/php-reverse-shell), jadi pastikan temen-temen download terlebih dahulu exploit ini. Setelah ``php-reverse-shell`` kalian download, silakan kalian edit file tersebut.
``Note :``
<br>
dikarenakan hanya file gambar saja yang bisa di upload pada fitur ``post comment`` oleh karena itu kita akan memanipulasi sehingga target mengira bahwa file exploit yang kita kirimkan adalah file gambar biasa. Caranya yaitu dengan menambahkan tulisan ``GIF89a;`` pada line 1 dan temen-temen juga tidak lupa untuk mengganti ``IP`` dan ``PORT`` nya ya, sesuai dengan ``IP`` dan ``PORT`` temen-temen miliki.
<center>
<img src="https://user-images.githubusercontent.com/28418984/184468581-2019b8b4-478b-43c7-9f9b-08a449a13714.png">
</center>
<center>
<img src="https://user-images.githubusercontent.com/28418984/184467967-8fce6417-e5a0-497a-a7c0-2c73fa507961.png">
</center>
<br>
setelah itu upload ``php-reverse-shell`` pada fitur ``post comment``. dan cek pada url ``http://blogger.thm/assets/fonts/blog/wp-content/uploads/2022/08/`` disitu sudah akan muncul file ``php-reverse-shell`` yang telah di upload tadi. silakan kalian nyalakan terlebih dahulu netcatnya ``nc -lvnp 4444`` dan open file ``php-reverse-shell`` tersebut, maka akan secara otomatis netcat akan meresponnya dan masuk kedalam shell sistem.
<center>
<img src="https://user-images.githubusercontent.com/28418984/184468558-27675477-dc28-4325-9fa3-9c53b35e631b.png">
</center>
lalu masukan perintah ``python3 -c 'import pty; pty.spawn("/bin/bash")'`` untuk mengganti menjadi ``bash`` dan masukan perintah ``export TERM=xterm`` kemudian ``CTRL+z`` > ``stty raw -echo && fg`` > untuk mengupgrade shell. Di sini saya mengecek pada direktori ``/home`` terdapat ``3 user``.
<center>
<img src="https://user-images.githubusercontent.com/28418984/184469002-a2d5677b-42ab-40fd-8535-c9b8c8949962.png">
</center>
<h2>Getting user’s flag</h2>
pada direktori ``/home/james/`` saya menemukan sebuah file ``user.txt`` namun ketikan saya masukan perintah ``cat user.txt`` file tersebut tidak meliki hak akses dan hanya dapat dibuka oleh user ``james``.
<center>
<img src="https://user-images.githubusercontent.com/28418984/184469104-eda0928b-bee3-4f1d-88c8-a76f813d0530.png">
</center>
kemudian kita cek ke direktori ``/tmp`` apakah ada file yang dapat digunakan sebagai informasi, ternyata di folder ``/tmp`` ada sebuah file ``backup.tar.gz``, namun ketika saya pindahkan dan saya extrack ke local. ternyata itu hanya jebakan (rabit hole) saja. isi dari file tersebut berupa ``encrypt base64``.
<center>
<img src="https://user-images.githubusercontent.com/28418984/184469891-c5e4c5ce-db4f-4e59-a13c-3a0af73cadfc.png">
</center>
<h2>Monitoring Process</h2>
Lalu saya mencoba melihat latar belakang pada sistem menggunakan ``PSPY``, untuk temen-temen yang ingin download ``PSPY`` bisa di [https://github.com/DominicBreuker/pspy](https://github.com/DominicBreuker/pspy) sesuaikan dengan versi bit komputer target ya. Ketika saya melakukan analisa pada latar belakang sistem, saya menemukan hal yang janggal, yang dimana ada sebuah proses yang menjalankan file ``backup.sh`` > ``/bin/sh /usr/local/bin/backup.sh ``.
<center>
<img src="https://user-images.githubusercontent.com/28418984/184470474-bdfb3790-a3ac-422c-9145-6a7f5df3ace7.png">
</center>
<br>
Ternyata file ``backup.sh`` memiliki fungsi untuk memanggail user ``james``. tetapi user ``www-data@ubuntu-xenial`` tidak dapat membaca dan menulis ke direktori tersebut.
<center>
<img src="https://user-images.githubusercontent.com/28418984/184470633-faa808b4-2496-4d25-a0bb-6428793b9268.png">
</center>
<br>sekarang saya akan menebak ``kata sandi`` user yang dimiliki oleh sistem ini, ternyata ada salah satu user yang memiliki ``username`` dan ``password`` yang sama, yaitu ``vagrant``.
<center>
<img src="https://user-images.githubusercontent.com/28418984/184480062-b909b02f-c76a-411d-8dac-d680c32f4a30.png">
</center>
<br>ketika saya memasukan perintah ``sudo -l`` saya menemukan bahwa user ``vagrant`` tidak memerlukan kata sandi untuk mengeksekusi apa pun pada siapa pun. oleh karena itu saya memasukan perintah ``sudo su james`` dan ternyata benar bisa masuk.
<center>
<img src="https://user-images.githubusercontent.com/28418984/184480227-7b988fde-168b-4a85-8faa-ec5a447da661.png">
</center>
<br>dikarena user ``vagrant`` bisa mengakses dimanapun saya akhirnya mencoba untuk masuk sebagai user ``root``
<h2>Get User Root</h2>
ternyata bisa masuk dan saya sedikit coba mengenumerate ke direktori ``/root`` disana ternyata ada ``FLAG`` > ``root.txt``.
<center>
<img src="https://user-images.githubusercontent.com/28418984/184480396-86081a67-7e94-4473-b3ff-05f4cda8aa7e.png">
</center>
Sekian dari tulisan writeup kedua kali ini, semoga tulisan ini dapat dipahami oleh temen-temen. misalkan ada kalimat yang bingung mau di tanyakan, bisa menghubungi twitter saya [@xcore13x](https://twitter.com/xcore13x). Terima kasih.

