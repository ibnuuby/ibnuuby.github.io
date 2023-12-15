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
<img src="https://github-production-user-asset-6210df.s3.amazonaws.com/28418984/290683914-e3effa61-7038-4266-ab2b-c1dc026e8ae1.jpeg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20231214%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231214T233755Z&X-Amz-Expires=300&X-Amz-Signature=fcbb178a64227080435f7c9edcbc377704b694f5eae2dd3694f643a943f9b1c4&X-Amz-SignedHeaders=host&actor_id=28418984&key_id=0&repo_id=517898668">
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
<img src="https://github-production-user-asset-6210df.s3.amazonaws.com/28418984/290685997-c5fc7739-6fc0-45a2-aa6c-d087ffba3df4.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20231214%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231214T235148Z&X-Amz-Expires=300&X-Amz-Signature=d06dfe60e40489ec0149ce7cb3fb6a44ee7fe541638b9022d233f9828959ad36&X-Amz-SignedHeaders=host&actor_id=28418984&key_id=0&repo_id=517898668">

Setelah file checkra1n berhasil di download, selanjutnya kalian, jalankan perintah ``chmod +x ./checkra1n``, setelah itu jalankan perintah ``./checkra1n``. maka chekra1n akan otomatis dijalankan.  

<center>
<img src="https://github-production-user-asset-6210df.s3.amazonaws.com/28418984/290686851-2d0275a0-d9d8-445c-b53d-606fc3aff323.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20231214%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231214T235812Z&X-Amz-Expires=300&X-Amz-Signature=d99e567c764d4d137d240b3284b11407616a0505664324ac756f13531d8a887b&X-Amz-SignedHeaders=host&actor_id=28418984&key_id=0&repo_id=517898668">
</center>

Selanjutnya pilih ``Start`` dan Enter. owh iya jangan lupa kalian harus menghubungkan iphone dengan menggunakan kabel USB terlebih dahulu ya sebelum menjalakan ``checkra1n`` ini.

Selanjutnya checkra1n akan membuat iPhone kita masuk ke recovery mode.

<center>
<img src="https://github-production-user-asset-6210df.s3.amazonaws.com/28418984/290687526-44d1940a-511b-4ec0-9581-7b0e506de187.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20231215%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231215T000216Z&X-Amz-Expires=300&X-Amz-Signature=bbf95eeaf6780cf1a61d3e462a25e2e8107ec0115c390eefaf81f2ef73ec592b&X-Amz-SignedHeaders=host&actor_id=28418984&key_id=0&repo_id=517898668">
</center>

Selanjutnya kita akan diinstruksikan untuk masuk ke DFU mode. Tinggal pilih Start, Enter, lalu ikuti saja instruksi dari checkra1n.

<center>
<img src="https://github-production-user-asset-6210df.s3.amazonaws.com/28418984/290687623-591954a2-be82-4f22-810d-38294e453d88.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20231215%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231215T000342Z&X-Amz-Expires=300&X-Amz-Signature=6e21ad50b7324a5b67337c4f601d7a58483ae728a7f566eac34cbd8812a1bfa0&X-Amz-SignedHeaders=host&actor_id=28418984&key_id=0&repo_id=517898668">
</center>

