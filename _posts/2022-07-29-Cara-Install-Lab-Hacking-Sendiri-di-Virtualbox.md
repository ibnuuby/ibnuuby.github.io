---
title: "Cara Install Lab Hacking Sendiri di Virtualbox"
author: Ibnu Ubaeydillah
layout: post
comments: true
permalink: /Cara-Install-Lab-Hacking-Sendiri-di-Virtualbox/
categories: Genel
tags: [tulisan, all-post]
---
Hello semuanya pada kesempatan kali ini saya akan menulis tentang ``Bagaimana cara menginstall lab hacking sendiri di virtualbox``. Banyak dari temen-temen disini masih mengalami kesulitan ketika melakukan praktek ``Penetration Pentesting``. Ya, untuk memudahkan hal tersebut saya membuat tulisan ini untuk temen-temen yang sedang belajar pada dunia ``cyber security``. Pada lab hacking ini, temen-temen nggak perlu khawatir akan merusak sistem. karena ini bersifatnya virtual di install ke komputer local server temen-temen. jadi temen-temen bebas bisa melakukan teknik apapun. Baik langsung mulai aja ``Bagaimana cara menginstall lab hacking sendiri di virtualbox``. 
<br>Ada beberapa bahan yang dibutuhkan pada tutorial kali ini, yaitu :
- VirtualBox, temen-temen bisa download virtualbox [disini](https://www.virtualbox.org/wiki/Downloads)
- Mesin Lab Hacking [DoubleTrouble 1](https://www.vulnhub.com/entry/doubletrouble-1,743/), mesin ini saya dowmnload dari [Vulnhub](https://download.vulnhub.com/doubletrouble/doubletrouble.ova)
<br>Setelah semua temen-temen download kalian bisa langsung mengikuti langkah-langkah dibawah ini
1. Download [Virtual](https://www.virtualbox.org/wiki/Downloads) dahulu, untuk linux bisa download [disini](https://www.virtualbox.org/wiki/Linux_Downloads) dan untuk windows bisa download [disini](https://download.virtualbox.org/virtualbox/6.1.36/VirtualBox-6.1.36-152435-Win.exe).
2. Disini saya akan mempraktekan bagaimana menginstall virtualbox di linux, karena saya menggunakan os linux, yang pertama temen-temen harus menambahkan repository virtualbox kedalam ``/etc/apt/sources.list``.
```
deb [arch=amd64 signed-by=/usr/share/keyrings/oracle-virtualbox-2016.gpg] https://download.virtualbox.org/virtualbox/debian <mydist> contrib
```
Kemudian inputkan perintah dibawah ini kedalam terminal temen-temen.
```
sudo gpg --dearmor oracle_vbox_2016.asc --yes --output /usr/share/keyrings/oracle-virtualbox-2016.gpg
```
atau bisa juga menggunakan perintah dibawah ini, ini hanya opsional ya. jadi temen-temen bebas memakai perintah apa.
```
wget -O- https://www.virtualbox.org/download/oracle_vbox_2016.asc | sudo gpg --dearmor --yes --output /usr/share/keyrings/oracle-virtualbox-2016.gpg
```
3. Lakukan ``sudo apt-get update`` dan tunggu sampai selesai
4. Inputkan perintah ``sudo apt-get install virtualbox-6.1`` dan misalkan disuruh milih, pilih yes/y
5. Tunggu proses installasi virtualbox sampai selesai
6. Setelah berhasil menginstall ``virtualbox`` langkah selanjutnya adalah temen-temen harus download mesin lab hacking yang akan digunakan. temen-temen bisa download [disini](https://download.vulnhub.com/doubletrouble/doubletrouble.ova)
7. Setelah selesai download mesin lab hacking, kita bisa langsung masuk ke proses konfigurasi.
8. Yang pertama silakan temen-temen buka ``virtualbox`` yang tadi di install.
9. Kemudian pilih menu ``File`` dan pilih menu ``Import Appliance``
<br>
<img src="https://user-images.githubusercontent.com/28418984/181749206-dbb154cf-ff1d-4f88-a6d1-11c195e1cff7.png">
10. Pilih ``File`` dan cari file ``OVA`` atau mesin lab yang kalian download tadi.
<img src="https://user-images.githubusercontent.com/28418984/181749609-20e51080-e9ad-4d88-b5c5-d5c05f0e9400.png">
11. Lalu tekan aja tombol ``Enter`` dan nanti akan muncul ``Appliance Settings`` kalian ``Enter`` lagi aja. Tunggu proses ``importing appliance`` sampai dengan selesai. 
12. Setelah selesai akan muncul ``virtual machine`` disebelah kiri
13. Kemudian temen-temen masuk ke ``Settings``
<img src="https://user-images.githubusercontent.com/28418984/181750630-29f607d3-c21d-47b9-91f1-44afaf3b2c78.png">
14. Pilih settingan ``Network``, untuk setinggan bisa dilihat digambar dibawah ini. owh iya disini saya menggunakan ``wlan0`` untuk alamat host yang akan digunakan untuk mesinnya ya.
<img src="https://user-images.githubusercontent.com/28418984/181750748-008e1710-de5b-44cd-b825-3ffeabe83f9b.png">
15. Lalu pilih menu ``OK`` untuk menyimpan hasil settingan.
16. Kemudian ``virtual machine`` yang tadi berhasil di install dan pilih menu ``Start``, makan akan secara otomatis mesin akan dijalankan dengan sendirinya.
<img src="https://user-images.githubusercontent.com/28418984/181751848-85c09ea4-a77e-485e-b1bf-3da76b7e2f3e.png">
17. Langkah selanjutnya adalah mengecek alamat ``ip wlan0`` kita berapa. caranya yaitu dengan mengetikan perintah ``ifconfig wlan0`` diterminal temen-temen.
18. Dan langkah yang terakhir adalah menggunakan aplikasi netdiscover gunakanya untuk mengetahui alamat host yang digunakan oleh ``mesin lab hacking`` temen-temen. untuk mengetahuinya menggunakan perintah ``sudo netdiscover -r alamat wlan0/24`` maka akan secara otomatis menampilakn host apa saja yang sedang berjalan. untuk lebih jelasnya bisa dilihat pada gambar dibawah ini ya.
<img src="https://user-images.githubusercontent.com/28418984/181753052-60be2da8-f568-4a3c-8865-a8da38857b7a.png">
19. Nah alamat IP/Host yang digunakan bisa dilihat pada tabel ``IP`` pada ``Mac Vendor/Hostname`` PCS Systemtechnik GmbH. setelah temen-temen dapet alamat IP/Host mesin lab hacking temen-temen. Silakan bisa ketikan ke browser temen dan jalankan. maka secara otomatis akan membuat ``Lab hacking`` temen-temen sendiri.
20. Selesai, Happy Hacking
<img src="https://user-images.githubusercontent.com/28418984/181753727-ed7a3428-ea43-46bf-aef0-f6b4e17757c8.png">