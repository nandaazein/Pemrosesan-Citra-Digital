<p align="center"><img src="img/rum.png"></p>

### **Lightness Method**
<p align="center"><img src="img/light.png"></p>
<p align="justify">Metode yang sangat sederhana adalah dengan mengambil nilai rata-rata yaitu menjumlahkan nilai tertinggi dan terendah.</p>

<p align="justify">Kita dapat dengan mudah melihat bahwa metode ini menghadirkan kelemahan yang sangat serius karena satu komponen RGB tidak digunakan. Ini jelas merupakan masalah karena jumlah cahaya yang dilihat mata kita bergantung pada ketiga warna dasar.</p>

### **Average Method**
<p align="center"><img src="img/ave.png"></p>
<p align="justify">Cara lain adalah dengan mengambil nilai rata-rata dari ketiga komponen (merah, hijau, dan biru).</p>

<p align="justify">Meskipun sekarang kita memperhitungkan semua komponen, metode rata-rata juga bermasalah karena memberikan bobot yang sama untuk setiap komponen. Berdasarkan penelitian tentang penglihatan manusia, kita tahu bahwa mata kita bereaksi terhadap setiap warna dengan cara yang berbeda. Secara khusus, mata kita lebih sensitif terhadap hijau, lalu merah, dan akhirnya biru. Oleh karena itu, bobot dalam persamaan di atas harus berubah.</p>

### **Luminosity Method**
<p align="center"><img src="img/lum.png"></p>

<p align="justify">Metode terbaik adalah metode luminositas yang berhasil memecahkan masalah metode sebelumnya. Berdasarkan pengamatan di atas, kita harus mengambil rata-rata tertimbang dari komponen. Kontribusi warna biru pada nilai akhir harus berkurang, dan kontribusi warna hijau harus meningkat.</p>

<p align="justify">Metode lightness cenderung mengurangi kontras. Metode luminositas bekerja paling baik secara keseluruhan dan merupakan metode default yang digunakan jika Anda meminta untuk mengubah gambar dari RGB ke skala abu-abu.</p>


<center><h1><b>HALFTONING</b></h1></center>

<p align="center"><img src="img/half1.png"></p>

<p align="justify"><b>Digital halftoning</b> adalah suatu proses untuk mengkonversi citra yang kontinu ke dalam suatu array berupa titik-titik. Jika dilihat oleh sistem visual manusia, pola tersebut akan  menciptakan  suatu  ilusi  sehingga  citra  tersebut  tampak  bukan  seperti  citra  hitam putih, namun seperti citra abu-abu yang kontinu.</p>

<p align="justify">Halftone adalah jenis efek visual statis yang diterapkan pada gambar digital dan cetak. Ini bekerja dengan prinsip yang sangat sederhana, di mana setiap piksel dalam area gambar dianggap sebagai titik dengan ukuran berbeda, beberapa di antaranya memakan lebih banyak ruang daripada satu piksel. Ketika gambar diubah menjadi halftone, tekstur gambar muncul seolah-olah telah ditempelkan di atas kumpulan titik tak terbatas tetapi tidak kontinu. Titik-titik tersebut sebenarnya tidak terbatas tetapi setara dengan resolusi total gambar. Gambar yang dihasilkan dikenal sebagai gambar halftone. Halftoning bertujuan  untuk  memberikan  kesan  warna  citra biner tampak  seperti citra abu-abu meskipun hanya menggunakan piksel warna hitam dan putih saja</p>

<p align="center"><b>gambar halftone</b></p>
<p align="center"><img src="img/half.png"></p>


<center><h1><b>PATTERNING</b></h1></center>

<p align="justify">Patterning adalah cara paling sederhana untuk menghasilkan gambar halftoning digital. Ini menghasilkan gambar yang memiliki resolusi spasial lebih tinggi daripada gambar sumber. Jumlah sel halftone citra keluaran sama dengan jumlah piksel citra sumber. Namun, setiap sel halftone dibagi lagi menjadi kotak 4x4. Setiap nilai piksel input diwakili oleh jumlah kotak terisi yang berbeda dalam sel halftone.

<p align="center"><b>Matriks pola rekursif</b></p>
<p align="center"><img src="img/pat1.png"></p>

<p align="center"><b>Operasi Pola</b></p>
<p align="center"><img src="img/pat2.png"></p>

<p align="justify">Pattern menghasilkan gambar halftoning digital dari gambar input menggunakan teknik pola. Pola program membaca gambar input, mengkuantisasi nilai piksel, dan memetakan setiap piksel ke pola yang sesuai. Gambar yang dihasilkan 16 kali lebih besar dari aslinya.</p>


<center><h1><b>DITHERING</b></h1></center>

Dithering juga merupakan salah satu cara untuk menghasilkan gambar halftoning. Tidak seperti pola, dithering membuat gambar keluaran dengan jumlah titik yang sama dengan jumlah piksel pada gambar sumber. Dithering dapat dianggap sebagai thresholding gambar sumber dengan matriks gentar. Matriks diletakkan berulang kali di atas gambar sumber. Dimanapun nilai piksel gambar lebih besar dari nilai dalam matriks, titik pada gambar output diisi.s</p>

<p align="center"><img src="img/dit1.png"></p>
<p align="center"><img src="img/dit2.png"></p>

<br>

## **Cara menentukan pola yang ada pada Patterning dan Dithering**

- **Patterning**
<p align="justify">Untuk menentukan banyaknya pola pada patterning kita bisa mengetahui secara langsung dengan menghitung banyaknya font biner atau pattern pengganti terlebih dahulu kemudian ditambahkan dengan 1.</p>

Contoh : menggunakan 4 x 4 font biner, maka banyaknya pola didapat adalah 17 pola.

<p align="justify">Pola yang ada pada patterning tidak boleh sama, pola yang sudah ada tidak boleh digunakan lagi (diputar dianggap sama).</p>

<p align="center"><img src="img/pat1.png"></p>

- **Dithering**

## **Cara menentukan matriks treshold pada dithering**

<p align="justify">Thresholding merupakan salah satu metode segmentasi citra di mana prosesnya didasarkan pada perbedaan derajat keabuan citra. Dalam proses ini dibutuhkan suatu nilai batas yang disebut nilai threshold. Nilai intensitas citra yang lebih dari atau sama dengan nilai threshold akan diubah menjadi hitam (0) sedangkan nilai intensitas citra yang kurang dari nilai threshold akan diubah menjadi putih (1).</p>

<p align="justify">Umumnya nilai Treshold(T) dihitung dengan menggunakan persamaan :</p>

<center><b>T = fmaks + fmin / 2</b></center>

<p align="justify">Dimana fmaks adalah nilai intensitas maksimum pada citra dan fmin adalah nilai intensitas minimun pada citra.</p>

<center><b>f(x,y) = 255, jika f(x,y) ??? T</b></center>
<center><b>f(x,y) = 0, jika f(x,y) < T </b></center>

Sebagai contoh misalnya diketahui citra grayscale 4x4 pixel

<table>
<tr>
<td>200</td>
<td>230</td>
<td>150</td>
<td>75</td>
</tr>
<tr>
<td>240</td>
<td>50</td>
<td>170</td>
<td>92</td>
</tr>
<tr>
<td>210</td>
<td>100</td>
<td>120</td>
<td>80</td>
</tr>
<tr>
<td>100</td>
<td>90</td>
<td>200</td>
<td>230</td>
</tr>
</table>


Dengan menggunakan persamaan ini, nilai treshold T didapatkan sebagai berikut :

<center><b> T = 240 + 50 / 2 = 145</b></center>

<p align="justify">Bila nilai T = 145 diterapkan untuk citra pada Gambar di atas maka diperoleh citra seperti : </p>

<table>
<tr>
<td>Hitam</td>
<td>Hitam</td>
<td>Hitam</td>
<td>Putih</td>
</tr>
<tr>
<td>Hitam</td>
<td>Putih</td>
<td>Hitam</td>
<td>Putih</td>
</tr>
<tr>
<td>Hitam</td>
<td>Putih</td>
<td>Putih</td>
<td>Putih</td>
</tr>
<tr>
<td>Putih</td>
<td>Putih</td>
<td>Hitam</td>
<td>Hitam</td>
</tr>
</table>


## **Mengapa hasil dithering dengan matriks 2x2 tidak sebagus yang lebih besar yaitu 16x16**

<p align="jutify"> Perbedaan antara keluaran yang dihasilkan antara citra  menggunakan  4x4  matriks dithering dan  16x16 matriks dithering terletak pada sensitifitas nilai piksel aslinya. Citra yang dihasilkan dari penggunaaan matriks 4x4 memiliki pola halftone yang kurang dibandingkan dengan citra yang diproses menggunakan matriks dithering 16x16. Karena itu hasil dari citra dengan 4x4 matriks dithering memiliki  banyak  daerah  dengan  pola  yang  sama, sehingga hasil yang ditampilkan menjadi kurang baik dibandingkan dithering dengan matriks 16x16.</p>






