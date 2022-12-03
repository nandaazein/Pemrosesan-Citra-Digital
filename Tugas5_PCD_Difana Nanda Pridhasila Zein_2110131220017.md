<p><h1><center><b>BIT PLANE SLICING</b></center></h1></p>

<p align="justify">Untuk menguraikan bit plane slicing pada sebuah citra menggunakan pemrograman octave kita bisa menuliskan atau menggunakan fungsi bitget.
 
<p align="center"><img src="img/cdbit.png"></p>

<p align="justify">Langkah menguraikan bit plane slicing</p>

- Untuk membaca citra yang digunakan kita bisa menggunakan imread

- Mengubah citra menjadi grayscale menggunakan fungsi rgb2gray

- Menampilkan citra yang sudah dirubah menggunakan imshow

- Membuat sebuah matriks sebanyak ukuran citra yang digunakan

- Mengatur posisi pada matriks menggunakan subplot

- Membuat variabel baru yang menyimpan nilai baris dan kolom agar menjadi nol

- Membuat 3 perulangan, perulangan pertama atau i dibuat untuk mengulang dari 1 sampai 8. Perulangan kedua akan mengulang sebanyak jumlah baris dan perulangan yang ketiga akan mengulang sebanyak kolom yang ada pada citra.

- Diluar perulangan gunakan fungsi sublot untuk mengatur posisi matriks dan buat counter agar keterangan yang ada selalu bertambah 1.

<p align="center"><img src="img/bit.png"></p>

<p><h1><center><b>STEGANOGRAFI</b></center></h1></p>

<p align="justify">Steganografi adalah sebuah metode dalam pemrosesan citra digital untuk menyembunyikan suatu data rahasia ke dalam sebuah citra.</p>

Data yang disembunyikan dapat berupa:

- Gambar

- Teks

- Suara

- Dll

<p align="center">Code untuk menyisipkan pesan dalam sebuah citra</p>

<p align="center"><img src="img/cdstg.png"></p>

<p align="center"><img src="img/cdstg1.png"></p>

<p align="center">Citra asli</p>

<p align="center"><img src="img/lenna.jfif"></p>

<p align="center">Citra yang sudah disisipkan pesan</p>

<p align="center"><img src="img/hasil_baru.png"></p>

<p align="justify">Jika dilihat secara langsung, tidak ada perbedaan yang cukup mencolok antara citra yang belum disisipi pesan dan citra yang sudah disisipi pesan.</p>

<p align="justify">Untuk melihat pesan rahasia yang sudah disisipkan dalam sebuah citra kita bisa menggunakan</p>

<center><img src="img/rahasia.png"></center>

<center><img src="img/rahasia2.png"></center>

<p><h1><center><b>EKSPERIMEN TUKAR GAMBAR</b></center></h1></p>

<p align="center">Citra Iif Alifah</p>

<p align="center"><img src="img/iif.jpg"></p>

<p align="center">Citra Sopia Refaldi</p>

<p align="center"><img src="img/faldi.jpeg"></p>

<p align="center">Code untuk menggabungkan beberapa citra</p>

<p align="center"><img src="img/cdgabung.png"></p>

<p align="center">Bit Plane Slicing dari 2 citra yang digabungkan</p>

<p align="center"><img src="img/hasil.png"></p>


