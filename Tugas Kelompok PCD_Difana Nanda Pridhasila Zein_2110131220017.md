<h1 align = "center"><b>TUGAS KEDELAPAN</b></h1>

----
KELOMPOK 2<br>
Nama Anggota:<br>
Ahmad Adieb Ibrahim (1710131210001)<br>
Difana Nanda Pridhasila Zein (2110131220017)<br>
Rapiyah Hawa Nur (1810131120017)<br>
Risalatul Husna (2110131120008)<br><br>

<p align = "justify"><b>SOAL :</b><br> Buatlah Kode Program Octave tentang Low Pass Filtering dan High Pass Filtering</p>

#
<h1 align = "center"><b>PENYELESAIAN</b></h1>

---
#
# __LOW PASS FILTERING__
<p align = "justify">

<p align="justify"><b>Low Pass Filtering (LPF)</b> : Proses filter yang melewatkan komponen citra dengan nilai intensitas yang rendah dan meredam komponen citra dengan nilai intensitas yang tinggi. Low Pass Filter disebut juga smoothing filter yang merupakan salah satu metode untuk menghilangkan noise acak, noise berkala, dan menampilkan pola latar belakang. 
</p>

<p align="justify">Low pass filtering digunakan untuk membuat citra menjadi lebih halus dan lebih blur. Efek pengaburan ini disebut dengan efek blurring.</p>

#
## *Ciri-ciri Kernel Low Pass Filtering*

- Jumlah semua elemen kernel bernilai satu. 

- Elemen kernel tidak ada yang bernilai negatif

- Tinggi dan lebar kernel ganjil, jika tidak bernilai ganjil maka piksel pusat tidak bisa ditemukan.

- Bobot dalam kernel bersifat simetris terhadap piksel pusat


#
## *Cara Menghitung Low Pass Filtering*
<p align="justify">Low pass filtering dilakukan dengan melakukan konvolusi antara citra dan kernel. Contoh kernel low pass filtering menggunakan matriks 3x3</p>

<p align="center"><img src="img/B1.PNG"></p>

<p align="center"><img src="img/B2.PNG"></p>

#
## *Pseudocode*

<p align = "center">Untuk Semua</p>
<p align="center"><img src="img/B4.PNG"></p>

<p align = "center">Pada Octave</p>
<p align="center"><img src="img/B3.PNG"></p>


#
## *Implementasi Low Pass Filtering dengan Octave*

#
### ___1) Kode Program Manual___
<br>
<p align="center"><img src="img/B19.PNG"></p>
<p align = "center">Kode Program</p>

<p align="center"><img src="img/B21.PNG"></p>
<p align = "center">Output Kode Program</p>

<p align="center"><img src="img/B20.PNG"></p>
<p align = "center">Citra Asli</p>

#
### ___1) Kode Program Yang Sudah ada pada Octave___
<br>
<p align="center"><img src="img/B5.PNG"></p>
<p align = "center">Kode Program</p>

<p align="center"><img src="img/B7.PNG"></p>
<p align = "center">Output Kode Program</p>

<p align="center"><img src="img/B8.PNG"></p>
<p align = "center">Output Kode Program</p>

<p align="center"><img src="img/B9.PNG"></p>
<p align = "center">Output Kode Program</p>

<p align="center"><img src="img/B6.PNG"></p>
<p align = "center">Citra Asli</p>




#
# __HIGH PASS FILTERING__
<p align = "justify">

<p align="justify"><b>High Pass Filter (HPF</b> adalah proses filter yang mengambil citra dengan gradiasi intensitas yang tinggi dan perbedaan intensitas yang rendah akan dikurangi atau dibuang. High Pass Filtering adalah salah satu dari metode penajaman (sharpening).</p> 

<p align="justify">Tujuan utama dari proses penajaman ini adalah untuk menyoroti detail-detail halus dalam gambar atau untuk meningkatkan detail yang telah dikaburkan baik dalam kesalahan atau efek alami dari proses akuisisi citra tertentu.</p>

#
## *Kegunaan High Pass Filtering*

- High-Pass Filter sering disebut juga sebagai filter penajaman tepi (edge sharpening) karena HPF digunakan dalam proses penajaman citra. 

- Operasi penajaman citra bertujuan untuk memperjelas tepi pada objek di dalam citra atau menghilangkan bagian citra yang lembut.

- Karena penajaman citra lebih berpengaruh pada tepi (edge) objek, maka penajaman citra sering disebut juga penajaman tepi (edge sharpening) atau peningkatan kualitas tepi (edge enhancement).


#
## *Ciri-ciri Kernel High Pass Filtering*
- Koefisien penapis boleh negatif, nol, ataupun bernillai positif.

- Total keseluruhan koefisiennya ialah bernilai 0 ataupun 1.

- Apabila jumlah koefisiennya berjumlah = 0, maka setiap elemen yang rendah frekuensinya nilainya akan menurun. 

- Namun, apabila total dari koefisien adalah = 1, maka elemen yang memiliki frekuensi rendah nilainya tetap sama dengan nilai semula


#
## *Implementasi High Pass Filtering dengan Octave*

#
### ___1) Kode Program Manual___
<br>
<p align="center"><img src="img/B22.jpeg"></p>
<p align = "center">Kode Program</p>

<p align="center"><img src="img/B23.jpeg"></p>
<p align = "center">Output Kode Program</p>

<h3><b><i>2) Kode Program Yang Sudah ada pada Octave</i></b></h3>
<br>
<p align="center"><img src="img/B10.PNG"></p>
<p align = "center">Kode Program</p>

<p align="center"><img src="img/B11.PNG"></p>
<p align = "center">Output Kode Program</p>

<p align="center"><img src="img/B12.PNG"></p>
<p align = "center">Output Kode Program</p>

<p align="center"><img src="img/b13.PNG"></p>
<p align = "center">Output Kode Program</p>

<p align="center"><img src="img/B14.PNG"></p>
<p align = "center">Output Kode Program</p>

<p align="center"><img src="img/B15.PNG"></p>
<p align = "center">Output Kode Program</p>

<p align="center"><img src="img/B16.PNG"></p>
<p align = "center">Output Kode Program</p>

# Implementasi High Boost Filtering

<p align="justify" >High-Boost Filtering merupakan salah satu bagian dari operasi yang dapat dilakukan untuk melakukan perbaikan citra.

High-Boost Filtering bertujuan untuk menekankan komponen frekuensi tinggi yang mewakili detail gambar tanpa menghilangkan komponen frekuensi rendah (seperti sharpening). Filter high boost dapat digunakan untuk mengubah komponen frekuensi tinggi.</p>

1. High Boost Filtering menggunakan fungsi

<p align="center"><img src="img/hbf.png"></p>

<p align="center"><img src="img/hbf1.png"></p>


# Implementasi Median Filtering

<p align="justify">Median filtering adalah teknik penyaringan digital nonlinear, yang sering digunakan untuk menghilangkan noise. Penyaringan median sangat banyak digunakan dalam pemrosesan gambar digital karena mempertahankan tepi sambil menghilangkan noise.

Penerapan dari median filtering dapat berupa untuk peningkatan kualitas citra gambar yang mengalami penurunan mutu citra, misalnya karena mengandung cacat atau derau (noise). Contohnya adalah bintik hitam atau putih yang muncul secara acak yang tidak diinginkan di dalam citra. bintik acak ini disebut dengan derau (noise) salt & pepper/</p>

1. Median Filtering menggunakan fungsi

<p align="center"><img src="img/medfunc.png"></p>

<p align="center"><img src="img/med1.png"></p>

2. Median Filtering secara manual

<p align="center"><img src="img/medman.png"></p>

<p align="center"><img src="img/medman1.png"></p>


# Implementasi Edge Detection

<p align="justify">Deteksi tepi (edge detection) pada suatu citra adalah suatu pendekatan untuk memeroleh tepi-tepi/garis batas dari objek di dalam citra tersebut. Tepi objek bermanfaat untuk segmentasi, registrasi, dan identifikasi antar objek pada citra.

Sutu titik (x, y) dapat dikatakan sebagai tepi jika terjadi perubahan nilai intensitas derajat keabuan (grayscale) yang tinggi dalam jarak yang dekat dengan tetangganya.</p>

1. Edge Detection menggunakan fungsi

<p align="center"><img src="img/ed.png"></p>

<p align="center"><img src="img/ed1.png"></p>

2. Edge Detection secara manual (Sobel)

<p align="center"><img src="img/egman.png"></p>

<p align="center"><img src="img/eg1.png"></p>



