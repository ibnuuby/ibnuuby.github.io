---
title: "Subdomain Enumeration"
author: Ibnu Ubaeydillah
layout: post
comments: true
permalink: /Subdomain-Enumeration/
categories: Genel
tags: [linux, all-post]
---

Ya subdomain, sebenarnya apa itu subdomain?
subdomain merupakan bagian dari sebuah nama domain induk. Subdomain umumnya mengacu ke suatu alamat fisik di sebuah situs contohnya: wikipedia.org merupakan sebuah domain induk. Sedangkan id.wikipedia.org merupakan sebuah subdomain.
Pada tulisan kali ini saya akan memberikan tutorial cara mengenumerasi subdomain. baik kita langsung mulai aja.
Hal pertama yang dibutuhkan adalah [Subfinder](#) dan [Httpx-Toolkit](#), jadi bagi kalian yang belum menginstall software tersebut kalian bisa install terlebih dahulu.
<br>Bagi kalian yang ``belum install subfinder``, kalian bisa mengikuti langkah-langkah dibawah ini.
1. Langkah yang pertama, kalian ``go install -v github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest``
2. Setelah berhasil kalian download, silakan masuk ke direktory ``/go/bin/`` disana kalian akan menemukan file ``subfinder``
3. Sekarang pindahkan file ``subfinder ke dalam folder /bin/subfinder/`` dengan mengetikan perintah ``sudo mv subfinder /bin/subfinder`` di terminal laptop kalian. 
4. Tujuannya untuk apa memindahkan file subfinder ke dalam direktory ``/bin/subfinder/`` yaitu agar dapat menjalankan perintah ``subfinder dimanapun`` berbeda sebelum dipindahkan ke ``/bin/subfinder``, kita perlu melakukan pemanggilan direktory dimana ``subfinder itu berada`` tentu itu akan sangat merepotkan.
5. Untuk mengetestnya apakah sudah berhasil melakukan penginstallan subfinder bisa dengan cara menginputkan perintah ``subfinder -version`` kedalam terminal kalian.
<br>Berikut adalah gambar ketika berhasil melakukan penginstallan subfinder
<br><img src="https://user-images.githubusercontent.com/28418984/181219663-d2fdd242-f21c-4f2e-af9b-2dc22d943244.png">
<br>Baik kita lanjut, sekarang kita akan menginstall ``Httpx-Toolkit``
1. Langkah pertama kalian inputkan perintah ``go install -v github.com/projectdiscovery/httpx/cmd/httpx@latest`` kedalam terminal kalian
2. Setelah berhasil download seperti biasa masuk ke dalam folder ``/go/bin/`` dan disana kalian akan menemukan file ``http-toolkit/httpx``. silakan pindahkan file tersebut ke dalam folder ``/bin/httpx-toolkit/`` dengan inputkan perintah `` sudo mv httpx-toolkit /bin/httpx-toolkit``.
3. Kalian bisa langsung mengecek di terminal laptop kalian apakah ``httpx-toolkit`` sudah terinstall atau belum dengan menginputkan perintah ``httpx-toolkit -v``. maka akan muncul seperti gambar di bawah ini.
<img src="https://user-images.githubusercontent.com/28418984/181224945-e0eedbb4-a7a9-4476-85a3-74a9b4debf34.png">
<br>Setelah semua bahan yang dibutuhkan telah terinstall semua.
Berikut adalah alur diagram bagaimana saya mencari sebuah subdomain.
<img src="https://user-images.githubusercontent.com/28418984/181231539-a86c3630-9aa1-46cb-8f1a-5aa22b809beb.jpg">
pada alur diagram gambar di atas saya membagi ke beberapa subdomain dengan ``status code`` yang berbeda-beda tujuannya untuk mempermudah saat proses pentest dan juga kita bisa memanfaatkan subdomain tersebut contohnya. untuk ``subdomain`` yang ``berstatus code 403`` bisa dijadikan sebagai vulnerability menjadi ``subdomain take over`` jikan memang subdomain itu terdapat vuln. tentu saja akan berbeda-beda cara ``mentake over subdomain``. untuk mengetahui bagaimana cara mengtakeover ``subdomain`` kalian bisa baca disini [Can I Take Over XYZ](https://github.com/EdOverflow/can-i-take-over-xyz).
<br>Sebelum saya berikan beberapa perintah untuk mencari subdomain berdasarkan ``status codenya`` saya akan memberikan beberapa sedikit penjelasan.

```
subfinder -d target.com
```
perintah di atas di gunakan untuk mencari sebuah domain, `-d` yang berarti ``domain`` dan ``target.com`` bisa kalian ganti sesuai dengan target yang kalian inginkan.

```
httpx-toolkit -status-code -title
```
Perintah di atas digunakan untuk menampilkan ``status-code`` pada sebuah domain/sistem. 
Misalkan kalian ingin mengetahui teknologi apa yang digunakan pada domain/sistem tersebut, kalian bisa menambahkan perintah ``-tech-detect``
```
httpx-toolkit -status-code -title -tech-detect
```
Bila kalian ingin mengetahui ``server header`` apa yang digunakan bisa menambahkan inputan ``-server``
```
http-toolkit -status-code -title -tech-detect -server
```
Bila kalian ingin mengetahui ``Host cname`` yang digunakan bisa menambahkan inputan ``-cname``
```
http-toolkit -status-code -title -tech-detect -server -cname
```
Bila kalian ingin mengetahui ``CDN`` yang digunakan bisa menambahkan inputan ``-cdn``
```
http-toolkit -status-code -title -tech-detect -server -cname -cdn
```
Berikut adalah beberapa perintah yang ada di ``HTTPX-toolkit`` bila kalian ingin mengeskplore lebih dalam lagi dalam penggunaa perintah di ``HTTPX-toolkit``:
``` 
   -sc, -status-code     Menampilkan Status Code
   -td, -tech-detect     Menampilkan Teknologi yang digunakan
   -cl, -content-length  Menampilkan Content-Length
   -server, -web-server  Menampilkan Server header
   -ct, -content-type    Menampilkan Content-Type header
   -lc, -line-count      Menampilkan Response body line count
   -wc, -word-count      Menampilkan Response body word count
   -rt, -response-time   Menampilkan the response time
   -title                Menampilkanpage title
   -location             Menampilkan Location header
   -method               Menampilkan Request method
   -websocket            Menampilkan server using websocket
   -ip                   Menampilkan Host IP
   -cname                Menampilkan Host cname
   -cdn                  Menampilkan if CDN in use
   -probe                Menampilkan probe status
```
Dari tadi, selalu cara menampilkan. mungkin ada yang bertanya bagaimana cara memfilternya sesuai dengan keinginan kita?
ya, bisa menambkan perintah ``-match-code string status code``, contohnya pada perintah dibawah ini saya ingin menfilter ``subdomain yang berstatus code 200``
```
http-toolkit -status-code -title -tech-detect -server -cname -cdn -match-code 200
```
Setelah semua sudah mengerti bagaimana cara menampilkan teknologi yang digunakan, cdn apa, webservernya apa. yang terakhir adalah bagaimana cara menyimpan subdomain tersebut berdasarkan ``status codenya``. kalian bisa menggunakan perintah dibawah ini:
```
http-toolkit -status-code -title -tech-detect -server -cname -cdn -fc 200 -o subsdomain_200.txt
```
jadi hanya menambahkan perintah yaitu ``-fc`` digunakan untuk memfilter ``status-code`` yang ingin disimpan dan perintah ``-o`` untuk menghasilkan output apa. disini saya menghasilkan ``output file txt`` sebagai contohnya.

Sejak tadi saya selalu menggunakan ``subfinder`` untuk mencari ``subdomain`` ya di sini saya akan memberikan sedikit trik yang biasa saya gunakan untuk mencari sebuah subdomain.
Perintah dibawah ini biasa saya gunakan untuk mencari subdomain, saya memanfaatkan web [crt.sh](https://crt.sh/) untuk mencari sebuah subdomain jadi di sini saya tidak hanya berfokus menggunakan ``subfinder`` saja, tapi menggunakan cara yang sedikit berbeda. berikut perintah yang biasa saya gunakan.
```
curl -s "https://crt.sh/?q=%25.HOST&output=json" | jq -r '.[].name_value' | sed 's/\*\.//g' | sort -u | httpx-toolkit -title -tech-detect -status-code
``` 
Pada tulisan ``HOST`` silakan bisa kalian ganti, dengan target yang kalian inginkan.
mungkin sampai sekian tulisan ini, tulisan ini akan terus di update bilamana disuatu hari nanti ada update terbaru.
<br>Terima kasih
<br>(ref//:https://id.wikipedia.org/wiki/Subdomain)
