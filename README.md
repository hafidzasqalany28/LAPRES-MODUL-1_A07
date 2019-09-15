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
 # Jawaban
 
4)  Cari charset dari halaman "ajk.if.its.ac.id"
 # Jawaban
 
5)  Cari username dan password ketika login di "freeshare.lp.if.its ac.id"
 # Jawaban
 
6)  Sebutkan web server yang digunakan pada "www.ne.its.ac.id"
 # Jawaban
 
7)  Sebutkan versi PHP dan yang digunakan pada "riset.ajk.if.its.ac.id"
 # Jawaban
 
8)  Filter pada wireshark kalian sehingga menampilkan hasil ping
 # Jawaban
 
9)  Dapatkan semua metode GET yang mengakses "monta.if.its.ac.id"
 # Jawaban
 
10) Tunjukkan username dan password yang dimasukkan ketika login FTP
 # Jawaban
 
11) Tunjukkan di wireshark, paket mana yang dikirimkan FTP client ketika upload file "qwpeaspojdasjfpasjfpaosuhuy.jpg"
 # Jawaban
 
12) Tunjukkan di wireshark, paket mana yang dikirimkan FTP client ketika menghapus file "qwpeaspojdasjfpasjfpaos.jpg"
 # Jawaban
 
13) Tunjukkan di wireshark, paket mana yang dikirimkan FTP client ketika mengganti nama file "sutlin.png"
 # Jawaban
 
14) Tunjukkan di wireshark, paket mana yang dikirimkan FTP client ketika download file "sutlun.png"
 # Jawaban
 
15) Cari file .zip di wireshark lalu download dan extract file tersebut 
    clue: "50 4B 03 04"
 # Jawaban
