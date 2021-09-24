# Jarkom-Modul-1-D12-2021
Laporan Resmi Praktikum Jaringan Komputer 2021 - D12
- Nur Hidayati (05111940000028)
- Pramudityo Prabowo (05111940000210)
- Muhammad Rizky Widodo (05111940000216)

## Soal No. 1
## Soal No. 2
## Soal No. 3
## Soal No. 4
## Soal No. 5
Login ke **portal.ichimarumaru.tech** kemudian ikuti perintahnya! Username dan password bisa didapat dari query insert pada table users dari file .pcap!

Pada soal ini, digunakan filter expression pada display filter ```mysql contains "password"```. Setelah semua paket tampil, selanjutnya pada bagian tengah, extend MYSQL Protocol kemudian extend Request Command Query. Pada bagian ini akan ditemukan statemen query insert pada table users yang memiliki atribut username dengan value **akakanomi** dan password dengn value **pemisah4lautan**.

<img src="img/soal-5-Wireshark.jpg" width=800></img><br>

Langkah selanjutnya yaitu masukkan username dan password yang telah didapat dan menjawab pertanyaan tentang urutan konfigurasi kabel T568B.

<img src="img/soal-5-hasil.jpg" width=800></img><br>

Kendala yang dialami yaitu mengalami beberapa kesalahan saat memasukkan filter expression pada display filter sehingga tidak menemukan username dan password.
## Soal No. 6
## Soal No. 7
## Soal No. 8
## Soal No. 9
Dari paket-paket yang menuju FTP terdapat indikasi penyimpanan beberapa file. Salah satunya adalah sebuah file berisi data rahasia dengan nama **secret.zip**. Simpan dan buka file tersebut!

Untuk menjawab soal ini, dapat digunakan filter expression pada display filter ```ftp-data.command contains "secret"```. Hasilnya sebagai berikut:

<img src="img/soal-9-Wireshark-1.jpg" width=800></img><br>

Selanjutnya pada salah satu paket dengan nama **secret.zip**, **klik kanan** kemudian **tcp stream** yang selanjutnya akan muncul tampilan berikut:

<img src="img/soal-9-Wireshark-2.jpg" width=800></img><br>

Lalu mengubah show data as menjadi **raw** dan menyimpan file tersebut sebagai zip file. Setelah file tersimpan file dapat dibuka dengan rar. Saat membuka file tersebut akan diminta password. 

<img src="img/soal-9-hasil.jpg" width=800></img><br>

Kendala yang dialami yaitu mengalami beberapa kesalahan saat memfilter paket.
## Soal No. 10
Selain itu terdapat **history.txt** yang kemungkinan berisi history bash server tersebut! Gunakan isi dari history.txt untuk menemukan password untuk membuka file rahasia yang ada di **secret.zip**!

Soal no 10 merupakan lanjutan dari soal no 9, langkah-langkahnya mirip hanya saja dibedakan pada filter file yang dicari. Untuk mencari file **history.txt** digunakan filter expression pada display filter ```ftp-data.command contains "history"```. Setelah paket muncul, pada bagian tengah, extend Line-based text data. Pada bagian ini akan ditemukan key dimana langkah selanjutnya yaitu mencari file **bukanapaapa.txt**. 

<img src="img/soal-10-Wireshark-1.jpg" width=800></img><br>

Untuk mencari file **bukanapaapa.txt** digunakan filter expression ```ftp-data.command contains "bukanapaapa"```. Setelah paket muncul, pada bagian tengah, extend Line-based text data. Pada bagian ini akan ditemukan passwordnya yaitu **d1b1langbukanapaapajugagapercaya.

<img src="img/soal-10-Wireshark-2.jpg" width=800></img><br>

Kemudian masukkan password tersebut untuk membuka file yang telah disimpan dan didapatkan hasil sebagai berikut:

<img src="img/soal-10-hasil.jpg" width=800></img><br>

Kendala yang dialami yaitu cukup kesulitan menemukan password untuk membuka file karena tidak meng-extend setiap bagiannya. Pada mulanya mengira bahwa passwordnya adalah bukanapaapa sehingga file tidak bisa dibuka.
## Soal No. 11
## Soal No. 12
## Soal No. 13
## Soal No. 14
## Soal No. 15
