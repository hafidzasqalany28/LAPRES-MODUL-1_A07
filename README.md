# LAPRES-MODUL-1_A07

 ## Soal "CAPTURE FILTER WIRESHARK"

1) Filter sehingga wireshark hanya mengambil paket yang mengandung port 21.
 # Jawaban
    
2) Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80 (ajk.if.its.ac.id).
 # Jawaban
    
3) Filter sehingga wireshark hanya menampilkan paket yang menuju port 443 (google.com).
 # Jawaban
    
4) Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian.
 # Jawaban
    
5) Filter sehingga wireshark hanya mengambil paket yang tujuannya ke monta.if.its.ac.id.
 # Jawaban
   
 ## Soal "DISPLAY FILTER WIRESHARK"
1)  Tampilkan semua paket yang hostnya mengandung "www.ne.its.ac.id"
 ### Jawaban
 
   ![Screenshot (68)](https://user-images.githubusercontent.com/45744801/64916036-5d80ba00-d79f-11e9-972a-60869061c4f2.png) Menggunakan syntax http.host == "www.ne.its.ac.id" untuk Menampilkan semua paket dengan protokol HTTP yang host nya mengandung   "www.ne.its.ac.id"

 
2)  Tampilkan paket yang hanya berasal dari IP 10.151.36 81 dan menuju web "mb.its.ac.id"
 ### Jawaban
 
   ![Screenshot (75)](https://user-images.githubusercontent.com/45744801/64917377-13f19880-d7ba-11e9-8af7-21d40822d6e6.png)
   #### Menggunakan syntax ip.src == 10.151.36.81 && http.host == "mb.its.ac.id".
   
   ip.src == 10.151.36.81 untuk memfilter IP yang hanya berasal dari 10.151.36.81(ip source).
     
   http.host == "mb.its.ac.id" untuk memfilter paket dengan protokol HTTP yang host nya mengandung "mb.its.ac.id".
 

 
3)  Simpan gambar ckedokteran.png
 ### Jawaban
 ![Screenshot (76)](https://user-images.githubusercontent.com/45744801/64917691-fd990c00-d7bc-11e9-98ba-7100c97e09ff.png)
 buka menu file ->Export Object-> HTTP Object List lalu masukkan nama file yang akan dicari di text filter. disini kita mencari      ckedokteran.png
 
 setelah itu tinggal save as/save untuk menyimpan gambar.
 
 note : disini memang filenya yang tidak ada.
 
4)  Cari charset dari halaman "ajk.if.its.ac.id"
 ### Jawaban
 ![Screenshot (77)](https://user-images.githubusercontent.com/45744801/64917692-feca3900-d7bc-11e9-9793-df83c79e63b5.png)
 menggunakan syntax http.host == "ajk.if.its.ac.id" untuk Menampilkan semua paket dengan protokol HTTP yang host nya mengandung "ajk.if.its.ac.id". pilih salah satu file dari hasil filteran tadi lalu klik kanan untuk memilih menu Follow -> TCP Stream. setelah itu tulis charset di menu text filter.
 
 note : host "ajk.if.its.ac.id" memang tidak ada.

5)  Cari username dan password ketika login di "freeshare.lp.if.its.ac.id"
 ### Jawaban
 ![Screenshot (73)](https://user-images.githubusercontent.com/45744801/64917700-2e794100-d7bd-11e9-9be2-83e9d555de7a.png)
 Menggunakan Syntax http.request.method == POST && http.host == "freeshare.lp.if.its.ac.id" setelah itu cari menu HTML Form URL Encoded di packet details panel/detail paket data. disitu kita bisa melihat bahwa user untuk login = "umum" dan password = "enter-umum". 
 
6)  Sebutkan web server yang digunakan pada "www.ne.its.ac.id"
 ### Jawaban
 ![Screenshot (78)](https://user-images.githubusercontent.com/45744801/64917738-bcedc280-d7bd-11e9-8295-470060e281b8.png)
 Menggunakan syntax http.host == "www.ne.its.ac.id" untuk Menampilkan semua paket dengan protokol HTTP yang host nya mengandung "www.ne.its.ac.id"
 
 pilih salah satu file dari hasil filteran tadi lalu klik kanan untuk memilih menu Follow -> TCP Stream. kemudian tulis server di menu text filter maka akan ketahuan web server yang dipakai adalah Apache/2.4.10 (Debian).
 ![Screenshot (79)](https://user-images.githubusercontent.com/45744801/64917741-bf501c80-d7bd-11e9-8df2-828dc52e5265.png)
 
7)  Sebutkan versi PHP dan yang digunakan pada "riset.ajk.if.its.ac.id"
 ### Jawaban
 ![Screenshot (80)](https://user-images.githubusercontent.com/45744801/64917750-e60e5300-d7bd-11e9-8147-aa93e98f9327.png)
 Menggunakan syntax http.host == "riset.ajk.if.its.ac.id" untuk Menampilkan semua paket dengan protokol HTTP yang host nya mengandung "riset.ajk.if.its.ac.id".
 
 pilih salah satu file dari hasil filteran tadi lalu klik kanan untuk memilih menu Follow -> TCP Stream. kemudian tulis PHP di menu text filter maka akan ketahuan PHP yang dipakai adalah 5.5.9-1ubuntu4.26.
 ![Screenshot (81)](https://user-images.githubusercontent.com/45744801/64917751-e73f8000-d7bd-11e9-87c7-51bb4434e820.png)
 
8)  Filter pada wireshark kalian sehingga menampilkan hasil ping
 ### Jawaban
 ![Screenshot (82)](https://user-images.githubusercontent.com/45744801/64917754-fb837d00-d7bd-11e9-82e5-4a0e44db4fc3.png)
 Menggunakan syntax "icmp" untuk menampilkan hasil ping.
 
9)  Dapatkan semua metode GET yang mengakses "monta.if.its.ac.id"
 ### Jawaban
 ![Screenshot (83)](https://user-images.githubusercontent.com/45744801/64917771-41404580-d7be-11e9-954a-78206217d406.png)
 menggunakan syntax http.request.method == GET  && http.host == "monta.if.its.ac.id"
 
 http.request.method == GET untuk memfilter semua paket dengan protokol htpp yang menggunakan metode GET
 http.host == "monta.if.its.ac.id" untuk  memfilter semua paket dengan protokol htpp yang host nya mengandung "monta.if.its.ac.id"
 
10) Tunjukkan username dan password yang dimasukkan ketika login FTP
 ### Jawaban
 ![Screenshot (84)](https://user-images.githubusercontent.com/45744801/64917839-36d27b80-d7bf-11e9-8a59-ee5e57781163.png)
Menggunakan syntax ftp.request.command == USER || ftp.request.command == PASS

disitu kita bisa melihat bahwa user dan password untuk login sama yaitu praktikum.

11) Tunjukkan di wireshark, paket mana yang dikirimkan FTP client ketika upload file "qwpeaspojdasjfpasjfpaosuhuy.jpg"
 ### Jawaban
 ![Screenshot (85)](https://user-images.githubusercontent.com/45744801/64918390-c11edd80-d7c7-11e9-96c3-8dd84f851400.png)
 Menggunakan syntax ftp.request.command == STOR && ftp.request.arg == "qwpeaspojdasjfpasjfpaosuhuy.jpg"
 

12) Tunjukkan di wireshark, paket mana yang dikirimkan FTP client ketika menghapus file "qwpeaspojdasjfpasjfpaos.jpg"
 ### Jawaban
 ![Screenshot (86)](https://user-images.githubusercontent.com/45744801/64918401-e9a6d780-d7c7-11e9-9f13-a4479d4dc8f5.png)
 Menggunakan syntax ftp.request.command == DELE && ftp.request.arg == "qwpeaspojdasjfpasjfpaos.jpg" untuk memfilter semua paket ftp yang menggunakan method DELE(rename) file "qwpeaspojdasjfpasjfpaos.jpg"
 
 note : memang tidak ada file "qwpeaspojdasjfpasjfpaos.jpg" sehingga ftp DELE(hapus) file pun tidak ada.
 
13) Tunjukkan di wireshark, paket mana yang dikirimkan FTP client ketika mengganti nama file "sutlin.png"
 ### Jawaban
 ![Screenshot (87)](https://user-images.githubusercontent.com/45744801/64918465-b9ac0400-d7c8-11e9-9bc6-273b65d1dee7.png)
 Menggunakan syntax ftp.request.command == RNFR  && ftp.request.arg == "sutlin.png" untuk memfilter semua paket ftp yang menggunakan method RNFR(rename) file "sutlin.png"
 
 
14) Tunjukkan di wireshark, paket mana yang dikirimkan FTP client ketika download file "sutlun.png"
 ### Jawaban
 ![Screenshot (88)](https://user-images.githubusercontent.com/45744801/64918466-badd3100-d7c8-11e9-99e0-0c04094f423f.png)
 Menggunakan syntax ftp.request.command == RETR && ftp.request.arg == "sutlun.png" untuk memfilter semua paket ftp yang menggunakan method RETR(download) file "sutlun.png"
 
15) Cari file .zip di wireshark lalu download dan extract file tersebut 
    clue: "50 4B 03 04"
 ### Jawaban
 ![Screenshot (89)](https://user-images.githubusercontent.com/45744801/64918467-bc0e5e00-d7c8-11e9-83ea-c5d0343b7d90.png)
 tekan ctrl + F di wireshark. kemudian masukkan clue yang tertera di soal dan jangan lupa ganti mode file menjadi Hex Value
 
 setelah itu pilih salah satu file dari hasil filteran tadi lalu klik kanan untuk memilih menu Follow -> TCP Stream. kemudian save as file dalam bentuk RAW agar bisa tersimpan dalam bentuk .zip dan juga bisa di extract.
 ![Screenshot (90)](https://user-images.githubusercontent.com/45744801/64918468-bca6f480-d7c8-11e9-9537-78cc9fa6ebb6.png)
 
 hasil extract dari .zip berisi file hantu.png
 ![Screenshot (91)](https://user-images.githubusercontent.com/45744801/64918470-bdd82180-d7c8-11e9-8c06-968eb367b091.png)
 
