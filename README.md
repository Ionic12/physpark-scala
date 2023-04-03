# physpark-scala
<p align="justify">Pyspark dan Scala keduanya digunakan untuk mengembangkan aplikasi big data pada framework Apache Spark dengan menyediakan antarmuka untuk akses fitur-fitur Spark. Pyspark adalah Python API, sementara Scala adalah bahasa pemrograman fungsional yang mendukung paradigma pemrograman berorientasi objek dan fungsional.

  <h1> Broadcast.py</h1>
  <p align="justify">menggunakan broadcast() pada SparkContext untuk mengirim list dari 1 hingga 99 ke setiap worker pada cluster. Nilai tersebut dapat diakses menggunakan .value.</p>
  <img src="BroadCast.py.png">
  
  <h1> UnderstandingRDDs.py</h1>
  <p align="justify">penggunaan PySpark pada mode standalone atau lokal, termasuk cara memulai command line dengan master tertentu dan memeriksa default parallelism. Selain itu, kode juga menunjukkan cara membuat RDD dengan jumlah partisi yang berbeda, mengakses isi setiap partisi, dan mengubah jumlah partisi dengan repartition() dan coalesce(). Terakhir, kode memeriksa grafik lineage RDD dengan toDebugString(). Kode ini dapat digunakan sebagai panduan dasar untuk penggunaan PySpark pada cluster atau mode lokal.</p>
  <img src="UnderstandingRDDs.png">

  <h1> WordCount.py</h1>
  <p align="justify">membaca file teks dari direktori tertentu menggunakan textFile() dari SparkContext dan melakukan penghitungan kata sederhana pada file tersebut. Kode menggunakan flatMap() untuk memisahkan setiap baris menjadi kata-kata, map() untuk menghitung jumlah kemunculan setiap kata, dan reduceByKey() untuk menggabungkan nilai-nilai yang sama menjadi satu nilai akhir. Output akhir dicetak menggunakan loop for. </p>
  <img src="WordCount.png">
  
  <h1> SystemCommandsOutput.scala</h1>
  <p align="justify">mengeksekusi perintah shell hadoop fs -ls menggunakan operator !! dan menampilkan outputnya menggunakan println().</p>
  <img src="SystemCommandsOutput1.png">
  <img src="SystemCommandsOutput2.png">

  <h1> SystemCommandsReturnCode.scala</h1>
  <p align="justify">import package sys.process untuk mengeksekusi perintah shell pada sistem operasi. Kode selanjutnya menjalankan perintah shell "ls /tmp" menggunakan operator ! dan menyimpan hasilnya dalam variabel res. Terakhir, kode mencetak hasil eksekusi perintah shell ke konsol dengan menggunakan println.</p>
  <img src="SystemCommandsReturnCode.png">
  
  <h1> LogAnalytics.py</h1>
  <p align="justify">Baris pertama mengimport modul sys dan add dari modul operator, serta mengimport SparkContext dari PySpark. selanjutnya memeriksa jumlah input yang diberikan dari baris perintah dan menampilkan pesan kesalahan jika jumlah input tidak sama dengan 2. selanjutnya menginisialisasi konteks Spark dengan nama aplikasi "Log Analytics". selanjutnya membaca file teks yang diberikan sebagai argumen dari baris perintah dan membaginya menjadi empat partisi. selanjutnya memfilter baris yang mengandung kata "ERROR" dan menyimpannya dalam variabel error_log. selanjutnya menyimpan error_log dalam cache untuk mengoptimalkan akses data. selanjutnya mencetak jumlah catatan error yang terdapat dalam file log. selanjutnya belas mencetak jumlah halaman produk yang dikunjungi dengan kesalahan dengan menggunakan filter untuk mencari baris yang mengandung kata "product". Jadi, program PySpark ini akan membaca file teks, mencari catatan error dan jumlah halaman produk yang dikunjungi dengan kesalahan, dan mencetak hasilnya ke konsol.
</p>
  <img src="AccessLog.png">
  <img src="Code.png">
  <img src="Result.png">
  
<h1> Accumulator.py</h1>
  <p align="justify">Program ini membuat objek accumulator dengan nilai awal 0 dan membuat RDD baru dengan elemen yang berasal dari rentang 1 hingga 99. Selanjutnya, program menggunakan foreach untuk menjalankan fungsi lambda pada setiap elemen dari RDD, yang menambahkan nilai elemen ke dalam accumulator. Terakhir, program mencetak nilai akhir dari accumulator ke konsol.</p>
<img src="Accumulator.py.png">

<h1> PairRDD.py</h1>
  <p align="justify">Program ini pertama-tama membuat sebuah list yang berisi tiga angka dan kemudian menjadikannya RDD dengan menggunakan sc.parallelize() dan menyimpannya ke dalam variabel myRDD. Selanjutnya, program memetakan setiap elemen RDD menjadi tuple dengan menggunakan fungsi map() dan menyimpan hasilnya dalam variabel myPairRDD. Kemudian, program menggunakan fungsi keys() untuk mengakses semua kunci dalam Pair RDD myPairRDD dan menyimpan hasilnya dalam variabel keys. Program juga menggunakan fungsi values() untuk mengakses semua nilai dalam Pair RDD myPairRDD dan menyimpan hasilnya dalam variabel values. Terakhir, program mencetak hasil kunci dan nilai ke konsol.</p>
<img src="PairRDD.py.png">



