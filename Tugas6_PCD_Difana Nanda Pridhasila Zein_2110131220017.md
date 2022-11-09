<center><h1>Metode Spasial dan Frekuensi Domain</h1></center>

<p align="justify">Berdasarkan ranah (domain) operasinya, metode-metode untuk memperbaiki kualitas citra dapat dikelompokkan menjadi dua kategori : </p>

- Image enhancement dalam ranah spasial
<p align="justify">Metode-metode image enhancement dalam ranah spasial dilakukan dengan memanipulasi secara langsung pixel-pixel di dalam citra.</p>
<p align="center"><img src="img/spasial.png"></p>

- Image enhancement dalam ranah frekuensi

<p align="center"><img src="img/frek.png"></p>
<p align="justify">Metode-metode image enhancement dalam ranah frekuensi dilakukan dengan mengubah citra terlebih dahulu dari ranah spasial ke ranah frekuensi, baru kemudian memanipulasi nilai-nilai frekuens tersebut.</p>

<p align="jutsify">Masing-masing ranah operasi digunakan untuk tujuan yang spesifik, karena <b>tidak semua perbaikan citra dapat dilakukan dalam ranah spasial</b> begitu juga sebaliknya.</p>

# **Domain Spasial**

<p align="justify">Peningkatan mutu citra pada domain spasial terbagi menjadi dua yaitu : </p>

- Point Processing

- Mask Processing

### **1. Point Processing**

<p align="justify">Cara paling mudah untuk melakukan peningkatan mutu pada domain spasial adalah dengan melakukan pemrosesan yang hanya melibatkan satu pixel saja.</p>

- Image Negative
<p align="justify">Mengubah nilai grey-level pixel citra input dengan : </p>

<p align="center">Hasilnya seperti klise foto :</p>
<p align="center"><img src="img/im.png"></p>

- Contrast Stretching
<p align="justify">Mengubah kontras dari suatu image dengan cara mengubah grey-level pixel pada citra menurut fungsi s = T(r) tertentu.</p>

<p align="center">Hasil contrast stretching</p>
<p align="center"><img src="img/cs.png"></p>

- Histogram Equalization
<p align="justify">Histogram : diagram yang menunjukkan jumlah kemunculan grey-level (0-255) pada suatu citra. Histogram equalization mengubah bentuk histrogram agar pemetaan grey-level pada citra juga berubah.</p>

<p align="center">Hasil histogram equalization</p>
<p align="center"><img src="img/he.png"></p>

- Image Substraction
<p align="justify">Dilakukan jika kita ingin mengambil bagian tertntu saja dalam suatu citra.</p>

<p align="center">Hasil image substraction</p>
<p align="center"><img src="img/is.png"></p>

- Image Averaging
<p align="justify">Dilakukan jika kita memiliki beberapa citra yang bergambar sama, namun semua citra mempunyai noise (gangguan). Noise satu citra berbeda dengan noise citra lainnya tidak berkorelasi, cara memperbaikinya adalah dengan melakukan operasi rata-rata terhadap semua citra tersebut.</p>


# **Mask Processing**

<p align="justify">Jika pada point processing kita hanya melakukan operasi terhadap masing-masing pixel, maka pada mask processing kita melakukan operasi terhadap suatu jendela ketatanggan pada citra.</p>
<p align="center">Kemudia kita menerapkan (mengkonvulasikan) suatu maks terhadap jendela tersebut, mask juga sering disebut <b>filter.</p>

<p align="center"><img src="img/mp.png"></p>

<p align="justify">Contoh : jendela ketetanggan 3x3, nilai pixel pada posisi x dipengaruhi oleh nilai tetangganya. Perbedaan dengan point processing, pada point processing nilai suatu pixel tidak dipengaruhi oleh nilai tetangganya sedangkan pada mask processing nilai pixel dipengaruhi oleh tetangganya.</p>

### **Jenis-jenis filter spasial**

- Smoothing filters : lowspass filter dan median filter.

- Sharpening filter.