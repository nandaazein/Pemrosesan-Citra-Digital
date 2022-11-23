#### **Kelompok 2**

- Difana Nanda Pridhasila Zein

- Risalatul Husna

- Rapiyah Hawa Nur 

- Ahmad Adieb Ibrahim 


# **LOW PASS FILTERING**

<p align="justify"><b>Low Pass Filtering (LPF)</b> : Proses filter yang melewatkan komponen citra dengan nilai intensitas yang rendah dan meredam komponen citra dengan nilai intensitas yang tinggi. Low Pass Filter disebut juga smoothing filter yang merupakan salah satu metode untuk menghilangkan noise acak, noise berkala, dan menampilkan pola latar belakang. 
</p>

<p align="justify">Low pass filtering digunakan untuk membuat citra menjadi lebih halus dan lebih blur. Efek pengaburan ini disebut dengan efek blurring.</p>

### **Ciri-ciri Kernel Low Pass Filtering**

- Jumlah semua elemen kernel bernilai satu. 

- Elemen kernel tidak ada yang bernilai negatif

- Tinggi dan lebar kernel ganjil, jika tidak bernilai ganjil maka piksel pusat tidak bisa ditemukan.

- Bobot dalam kernel bersifat simetris terhadap piksel pusat

### **Manual Low Pass Filtering**

### **Octave Low Pass Filtering**

<center><img src="img/lowman1.png"></center>
<center><img src="img/lowman2.png"></center>



# **HIGH PASS FILTERING**

<p align="justify"><b>High Pass Filter (HPF</b> adalah proses filter yang mengambil citra dengan gradiasi intensitas yang tinggi dan perbedaan intensitas yang rendah akan dikurangi atau dibuang. High Pass Filtering adalah salah satu dari metode penajaman (sharpening).</p> 

<p align="justify">Tujuan utama dari proses penajaman ini adalah untuk menyoroti detail-detail halus dalam gambar atau untuk meningkatkan detail yang telah dikaburkan baik dalam kesalahan atau efek alami dari proses akuisisi citra tertentu.</p>

### **Kegunaan High Pass Filtering**

- High-Pass Filter sering disebut juga sebagai filter penajaman tepi (edge sharpening) karena HPF digunakan dalam proses penajaman citra. 

- Operasi penajaman citra bertujuan untuk memperjelas tepi pada objek di dalam citra atau menghilangkan bagian citra yang lembut.

- Karena penajaman citra lebih berpengaruh pada tepi (edge) objek, maka penajaman citra sering disebut juga penajaman tepi (edge sharpening) atau peningkatan kualitas tepi (edge enhancement).


### **Ciri-ciri Kernel High Pass Filtering**
- Koefisien penapis boleh negatif, nol, ataupun bernillai positif.

- Total keseluruhan koefisiennya ialah bernilai 0 ataupun 1.

- Apabila jumlah koefisiennya berjumlah = 0, maka setiap elemen yang rendah frekuensinya nilainya akan menurun. 

- Namun, apabila total dari koefisien adalah = 1, maka elemen yang memiliki frekuensi rendah nilainya tetap sama dengan nilai semula

### **Manual High Pass Filtering**

### **Octave High Pass Filtering**

<center><img src="img/highman1.png"></center>
<center><img src="img/highman2.png"></center>
