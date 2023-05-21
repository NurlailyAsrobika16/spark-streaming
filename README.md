# Tugas Praktikum
<ol>
  <li>Jelaskan perbedaan Spark Streaming dengan metode stateless dan stateful stream processing?</li>
  <li>Jelaskan masing-masing maksud kode berikut sesuai nomor kodenya pada laporan praktikum Anda!</li>
</ol>

<img src="Tugas.png" width="700">

<ol>
  <li>
    <p>
      <strong>- sys.argv:</strong> Ini adalah daftar dalam modul sys di Python yang memberikan akses ke argumen baris perintah yang dilewatkan ke sebuah skrip. Ini memungkinkan Anda untuk mengakses argumen yang dilewatkan ke skrip Python saat dieksekusi dari baris perintah.
    </p>
    <p>
      <strong>- sys.stderr:</strong> Ini adalah objek mirip file dalam modul sys di Python yang mewakili aliran kesalahan standar. Digunakan untuk mencetak pesan kesalahan dan informasi traceback.
    </p>
    <p>
      <strong>- StreamingContext:</strong> Ini adalah kelas dalam modul Streaming Apache Spark yang digunakan untuk membuat DStream, yang merupakan Discretized Stream. DStream mewakili aliran data kontinu dalam Spark.
    </p>
    <p>
      <strong>- sc:</strong> Ini adalah objek dalam Apache Spark yang mewakili SparkContext. SparkContext adalah titik masuk untuk semua fungsionalitas Spark. Digunakan untuk membuat RDD (Resilient Distributed Datasets) dan melakukan operasi pada mereka.
    </p>
    <p>
      <strong>- socketTextStream:</strong> Ini adalah fungsi dalam Apache Spark Streaming yang membuat DStream dengan mendengarkan soket untuk data. Membaca data teks yang diterima melalui soket sebagai aliran baris masukan.
    </p>
    <p>
      <strong>- reduceByKey:</strong> Ini adalah operasi transformasi dalam Apache Spark yang digunakan pada pasangan RDD untuk menggabungkan nilai-nilai setiap kunci menggunakan fungsi reduce yang ditentukan. Mengelompokkan nilai-nilai setiap kunci dan menerapkan fungsi reduce pada nilai-nilai yang dikelompokkan.
    </p>
    <p>
      <strong>- lambda line:</strong> Ini adalah fungsi lambda dalam Python yang mengambil parameter bernama 'line' dan mewakili fungsi anonim. Dapat digunakan untuk mendefinisikan fungsi kecil satu baris tanpa nama.
    </p>
    <p>
      <strong>- awaitTermination:</strong> Ini adalah metode dalam StreamingContext Apache Spark yang memblokir thread saat ini sampai konteks streaming dihentikan secara eksplisit atau terjadi pengecualian.
    </p>
  </li>
  <li>
    <p>
      <strong>- nc:</strong> Ini merujuk pada perintah "nc" atau "netcat" di Linux. Ini adalah utilitas yang digunakan untuk membaca dari dan menulis ke koneksi jaringan. Dalam konteks data streaming, "nc" sering digunakan untuk mengatur soket jaringan yang berfungsi sebagai sumber data.
    </p>
    <p>
      <strong>- lk:</strong> Istilah "lk" tidak memiliki arti standar atau diakui secara luas dalam konteks pemrograman atau pemrosesan data. Tanpa konteks tambahan, sulit untuk menentukan arti spesifiknya.
    </p>
  </li>
  <li>
    <p>
      <strong>- spark-submit:</strong> Ini adalah alat baris perintah yang disediakan oleh Apache Spark yang digunakan untuk mengirimkan aplikasi Spark ke sebuah kluster. Ini mengambil file JAR atau file Python aplikasi sebagai input dan meluncurkan aplikasi di kluster.
    </p>
    <p>
      <strong>- master:</strong> Ini adalah parameter yang digunakan dengan spark-submit untuk menentukan alamat manajer kluster. Ini menentukan di mana aplikasi Spark harus dijalankan.
    </p>
    <p>
      <strong>- local[*]:</strong> Ini adalah nilai khusus untuk parameter "master" dalam Apache Spark yang menunjukkan aplikasi harus dijalankan secara lokal pada semua core yang tersedia. Sering digunakan untuk pengembangan dan pengujian lokal.
    </p>
  </li>
  <li>
    <p>
      <strong>- ssc.checkpoint:</strong> Ini adalah metode dalam StreamingContext Apache Spark yang mengatur direktori di mana sistem streaming akan menulis file checkpoint. Checkpointing digunakan untuk toleransi kesalahan dan pemulihan dalam aplikasi streaming.
    </p>
    <p>
      <strong>- parallelize:</strong> Ini adalah metode dalam SparkContext Apache Spark yang digunakan untuk membuat RDD dari koleksi data dalam program pengemudi. Mendistribusikan data ke beberapa partisi untuk memungkinkan pemrosesan paralel.
    </p>
    <p>
      <strong>- updateStateByKey:</strong> Ini adalah operasi transformasi dalam Apache Spark Streaming yang memungkinkan Anda untuk mempertahankan informasi status sembarang di beberapa batch data. Digunakan untuk memperbarui status suatu kunci berdasarkan data masukan baru dan fungsi pembaruan yang ditentukan oleh pengguna.
    </p>
    <p>
      <strong>- flatMap:</strong> Ini adalah operasi transformasi dalam Apache Spark yang digunakan untuk mengubah setiap elemen RDD menjadi nol atau lebih elemen keluaran. Mengambil fungsi sebagai argumen dan menerapkannya pada setiap elemen masukan untuk menghasilkan elemen keluaran.
    </p>
  </li>
  <li>
    <p>
      <strong>- rdd.take(5):</strong> Ini adalah metode dalam RDD Apache Spark yang mengembalikan lima elemen pertama dari RDD.
    </p>
  </li>
</ol>

## Praktik Dasar Spark Streaming

### Metode 1: Mode Stateless Stream Processing

**Interval waktu per 1 detik**

<img src="01_stateless/1.png" width="700">
<br>
<img src="01_stateless/2.png" width="700">

**Interval waktu per 5 detik**

<img src="01_stateless/3.png" width="300">
<br>
<img src="01_stateless/4.png" width="700">

### Metode 2: Mode Stateful Stream Processing

**Interval waktu per 1 detik**

<img src="02_stateful/4.png" width="700">
<br>
<img src="02_stateful/5.png" width="700">
<br>
<img src="02_stateful/6.png" width="700">

**Interval waktu per 5 detik**

<img src="02_stateful/7.png" width="300">
<br>
<img src="02_stateful/8.png" width="700">

## Melakukan Transformasi di Spark Streaming

**Interval waktu per 1 detik**

<img src="03_transformasi_word_sentiment/1.png" width="700">
<br>
<img src="03_transformasi_word_sentiment/2.png" width="700">

**Interval waktu per 5 detikk**

<img src="03_transformasi_word_sentiment/3.png" width="300">
<br>
<img src="03_transformasi_word_sentiment/4.png" width="700">
