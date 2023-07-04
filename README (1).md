
# Deteksi Marka Jalan

*Teori Tentang Marka Jalan*

Marka jalan merupakan elemen penting dalam pengaturan lalu lintas dan keselamatan jalan. Mereka adalah tanda atau garis yang terletak di permukaan jalan dan berfungsi sebagai panduan dan petunjuk bagi pengguna jalan. Dalam konteks pengolahan citra, marka jalan merujuk pada proses pengenalan dan analisis tanda-tanda atau garis-garis pada gambar atau video jalan.

Pengolahan citra marka jalan bertujuan untuk mengidentifikasi dan memahami informasi yang terkandung dalam tanda-tanda atau garis-garis marka jalan. Salah satu aplikasi utama dari pengolahan citra marka jalan adalah pemetaan jalan, di mana citra jalan dianalisis untuk mengidentifikasi dan memetakan letak marka jalan. Informasi ini dapat digunakan untuk membuat peta digital yang akurat dari jalan-jalan di suatu daerah.

Selain itu, pengolahan citra marka jalan juga dapat digunakan untuk pengukuran lebar jalan. Dengan mengidentifikasi garis marka jalan di gambar atau video, pengukuran lebar jalan dapat dilakukan dengan presisi tinggi. Informasi ini dapat digunakan untuk analisis lalu lintas, perencanaan jalan, dan pemeliharaan infrastruktur jalan.

Selain itu, pengolahan citra marka jalan dapat membantu dalam estimasi posisi kendaraan. Dengan menganalisis posisi relatif kendaraan terhadap marka jalan, sistem pengolahan citra dapat memberikan informasi tentang posisi kendaraan di jalan, kecepatan kendaraan, dan perubahan jalur. Informasi ini sangat penting dalam pengembangan kendaraan otonom atau sistem pengawasan lalu lintas yang cerdas.

Secara keseluruhan, pengolahan citra marka jalan merupakan bidang penelitian yang penting dalam pengembangan teknologi transportasi dan pengelolaan lalu lintas. Melalui analisis tanda-tanda atau garis-garis marka jalan, informasi yang berharga dapat diekstraksi untuk tujuan identifikasi dan pemetaan jalan, pengukuran lebar jalan, estimasi posisi kendaraan, dan masih banyak lagi. Dengan memahami dan menerapkan teknik pengolahan citra ini, kita dapat meningkatkan efisiensi, keamanan, dan keandalan sistem transportasi di masa depan.
Pengolahan citra untuk mendeteksi dan memahami marka jalan melibatkan serangkaian langkah, seperti segmentasi, deteksi garis, dan ekstraksi fitur. Berikut adalah penjelasan lebih rinci tentang langkah-langkah ini:

1. Segmentasi adalah tahap awal dalam pengolahan citra marka jalan yang bertujuan untuk memisahkan area gambar menjadi komponen yang berbeda, seperti jalan, marka jalan, kendaraan, dan latar belakang. Proses segmentasi ini penting untuk memfokuskan analisis pada area yang relevan, yaitu marka jalan.

Metode segmentasi yang umum digunakan dalam pengolahan citra marka jalan antara lain:

- Thresholding: Metode ini memisahkan piksel-piksel gambar berdasarkan ambang nilai tertentu. Piksel dengan nilai di atas ambang nilai tersebut dianggap sebagai marka jalan, sedangkan piksel dengan nilai di bawah ambang nilai dianggap sebagai latar belakang atau objek lain.

- Pemisahan Warna: Metode ini memanfaatkan perbedaan warna antara marka jalan dan latar belakang untuk memisahkan komponen tersebut. Misalnya, jika marka jalan memiliki warna putih dan latar belakangnya berwarna lain, maka dengan melakukan analisis warna, piksel dengan warna putih dapat diidentifikasi sebagai marka jalan.

- Metode Berbasis Kontur: Metode ini melibatkan deteksi kontur atau tepi pada gambar. Marka jalan umumnya memiliki garis-garis kontur yang berbeda dengan latar belakangnya. Dengan mengidentifikasi dan memisahkan kontur yang berkaitan dengan marka jalan, kita dapat memisahkan marka jalan dari latar belakang.

Setiap metode segmentasi memiliki kelebihan dan kelemahan tertentu, dan pilihan metode yang tepat tergantung pada karakteristik gambar atau video yang akan diproses. Penggunaan metode segmentasi yang tepat akan menghasilkan pemisahan yang akurat antara marka jalan, jalan, kendaraan, dan latar belakang.

Dengan melakukan segmentasi yang baik, kita dapat mengisolasi marka jalan dari latar belakang dan objek lain dalam citra. Hal ini memungkinkan langkah-langkah selanjutnya, seperti deteksi garis dan ekstraksi fitur, untuk dilakukan dengan fokus pada marka jalan yang relevan. Segmen marka jalan yang terpisah kemudian dapat dianalisis lebih lanjut untuk pemetaan, pengukuran, estimasi posisi kendaraan, dan berbagai aplikasi pengolahan citra marka jalan lainnya.

2. Deteksi garis merupakan langkah penting dalam pengolahan citra marka jalan setelah proses segmentasi. Tujuan dari deteksi garis adalah untuk menemukan garis-garis marka jalan yang terdapat dalam citra atau video. Terdapat beberapa metode yang umum digunakan dalam deteksi garis, seperti transformasi Hough dan deteksi tepi.

- Transformasi Hough: Metode transformasi Hough adalah salah satu metode yang sering digunakan dalam deteksi garis. Metode ini memungkinkan deteksi garis secara presisi tinggi bahkan ketika garis tersebut tidak terlalu jelas dalam citra. Transformasi Hough bekerja dengan mengubah titik-titik dalam ruang citra menjadi representasi parameter garis dalam ruang parameter. Dalam ruang parameter tersebut, garis-garis marka jalan akan memberikan pola yang terkonsentrasi, sehingga dapat terdeteksi dengan akurasi tinggi.

- Deteksi Tepi: Metode deteksi tepi juga sering digunakan dalam deteksi garis marka jalan. Deteksi tepi melibatkan penggunaan operator filter, seperti operator Sobel atau Canny, untuk menemukan perbedaan intensitas yang signifikan di antara piksel-piksel dalam gambar. Garis marka jalan umumnya memiliki perbedaan intensitas yang jelas dengan latar belakangnya, sehingga dapat terdeteksi sebagai tepi yang kuat dalam citra.

Kedua metode tersebut memiliki kelebihan dan kelemahan masing-masing. Transformasi Hough memiliki keunggulan dalam mendeteksi garis dengan berbagai orientasi dan posisi dalam citra, sementara deteksi tepi lebih sensitif terhadap perbedaan intensitas lokal. Pilihan metode yang tepat tergantung pada karakteristik citra atau video yang akan diproses serta tujuan deteksi garis yang diinginkan.

Dengan menggunakan metode deteksi garis yang tepat, kita dapat mengidentifikasi dan menemukan garis-garis marka jalan yang ada dalam citra atau video. Deteksi garis yang akurat memungkinkan kita untuk mengetahui letak, panjang, orientasi, dan arah marka jalan. Informasi ini sangat berharga dalam pemetaan jalan, pengukuran lebar jalan, estimasi posisi kendaraan, serta dalam pengembangan sistem pengawasan lalu lintas yang cerdas.

3. Ekstraksi fitur adalah langkah penting setelah garis-garis marka jalan terdeteksi dalam pengolahan citra marka jalan. Pada tahap ini, berbagai fitur yang menggambarkan karakteristik marka jalan diekstraksi dari gambar atau video untuk analisis lebih lanjut. Beberapa fitur yang umum diekstraksi meliputi panjang garis, posisi relatif terhadap jalan, sudut kemiringan, dan informasi warna marka jalan.

- Panjang Garis: Dengan mengukur panjang garis marka jalan yang terdeteksi, kita dapat memperkirakan lebar jalan. Informasi ini sangat penting dalam perencanaan lalu lintas dan perawatan infrastruktur jalan. Panjang garis juga dapat digunakan untuk menghitung rasio marka jalan terhadap panjang jalan secara keseluruhan.

- Posisi Relatif Terhadap Jalan: Dengan mengetahui posisi garis marka jalan terhadap jalan secara relatif, seperti jarak dari tepi jalan atau letaknya di antara jalur kendaraan, kita dapat memahami konfigurasi jalan yang spesifik. Informasi ini penting dalam pemetaan jalan, perencanaan lalu lintas, dan navigasi kendaraan.

- Sudut Kemiringan: Mengukur sudut kemiringan garis marka jalan dapat memberikan informasi tentang arah lalu lintas pada jalan. Misalnya, sudut kemiringan yang curam mungkin menandakan jalan berkelok-kelok atau tikungan tajam. Hal ini dapat digunakan dalam navigasi kendaraan otonom atau sistem peringatan pengemudi.

- Informasi Warna: Warna marka jalan juga dapat menjadi fitur yang penting dalam ekstraksi fitur. Dengan mengidentifikasi pola warna dan bentuk marka jalan, kita dapat mengklasifikasikan jenis marka jalan, seperti marka jalan putih, kuning, atau merah. Selain itu, informasi warna juga dapat digunakan untuk mengevaluasi kondisi marka jalan, seperti keausan atau kerusakan.

Fitur-fitur yang diekstraksi ini memberikan pemahaman lebih lanjut tentang marka jalan yang terdeteksi dan dapat digunakan dalam berbagai aplikasi. Misalnya, dengan menggunakan informasi panjang garis dan posisi relatif terhadap jalan, kita dapat memperoleh pemetaan yang lebih akurat. Informasi warna dan bentuk marka jalan dapat digunakan untuk pengenalan pola atau klasifikasi marka jalan. Selain itu, ekstraksi fitur juga dapat digunakan dalam evaluasi kondisi marka jalan dan pemeliharaan infrastruktur jalan secara keseluruhan.

4. Pemetaan dan analisis: Setelah ekstraksi fitur, informasi yang diperoleh dari marka jalan dapat digunakan untuk pemetaan jalan dan analisis lebih lanjut. Pemetaan jalan melibatkan identifikasi dan pemetaan letak marka jalan pada peta digital. Ini membantu dalam pemeliharaan dan perencanaan infrastruktur jalan. Analisis lebih lanjut dapat mencakup estimasi posisi kendaraan relatif terhadap marka jalan, pengenalan pola marka jalan untuk tindakan peringatan atau pengendalian, serta penilaian kondisi marka jalan seperti keausan atau kerusakan. 

Setelah dilakukan ekstraksi fitur dari marka jalan, informasi yang diperoleh dapat digunakan untuk pemetaan jalan dan analisis lebih lanjut. Berikut adalah pengembangan lebih detail tentang pemetaan dan analisis:

- Pemetaan Jalan: Dengan menggunakan informasi lokasi dan karakteristik marka jalan yang telah diekstraksi, dapat dilakukan pemetaan jalan. Pemetaan jalan melibatkan identifikasi dan penempatan letak marka jalan pada peta digital yang melambangkan jaringan jalan yang sebenarnya. Informasi ini membantu dalam pemeliharaan dan perencanaan infrastruktur jalan. Pemetaan yang akurat memungkinkan pemangku kepentingan, seperti pemerintah daerah atau lembaga lalu lintas, untuk memiliki pemahaman yang lebih baik tentang keadaan jalan dan memfasilitasi perbaikan atau perubahan yang diperlukan.

- Estimasi Posisi Kendaraan: Dengan memanfaatkan informasi marka jalan yang terdeteksi, dapat dilakukan estimasi posisi kendaraan relatif terhadap marka jalan. Dalam sistem navigasi kendaraan otonom atau bantuan pengemudi, informasi ini penting untuk menentukan posisi dan lintasan kendaraan. Dengan membandingkan posisi kendaraan dengan letak marka jalan yang telah dipetakan, sistem dapat memberikan peringatan atau instruksi kepada pengemudi atau mengarahkan kendaraan secara otomatis.

- Pengenalan Pola Marka Jalan: Informasi mengenai pola marka jalan yang diekstraksi dapat digunakan untuk pengenalan pola dan klasifikasi marka jalan. Misalnya, dengan menganalisis pola warna, bentuk, atau simbol yang terkandung dalam marka jalan, dapat diidentifikasi tanda-tanda khusus seperti zebra cross atau marka jalan prioritas. Informasi ini dapat digunakan untuk tindakan peringatan, pengendalian lalu lintas, atau pengumpulan data tentang perilaku pengendara.

- Penilaian Kondisi Marka Jalan: Ekstraksi fitur marka jalan juga dapat digunakan untuk penilaian kondisi marka jalan, seperti keausan atau kerusakan. Dengan melihat fitur-fitur seperti panjang garis atau warna marka jalan, dapat dilakukan analisis terhadap kondisi marka jalan secara keseluruhan. Informasi ini penting dalam penjadwalan perawatan jalan atau evaluasi keefektifan tindakan pemeliharaan yang telah dilakukan.

Pemetaan jalan dan analisis lebih lanjut ini memberikan pemahaman yang lebih dalam tentang kondisi, lokasi, dan fungsi marka jalan. Informasi ini dapat digunakan dalam berbagai aplikasi, mulai dari perencanaan lalu lintas, navigasi kendaraan, hingga pengawasan dan pemeliharaan infrastruktur jalan yang efisien dan aman.

Pengolahan citra marka jalan melalui serangkaian langkah-langkah yang telah dijelaskan sebelumnya menghasilkan informasi berharga tentang jalan, marka jalan, dan penggunaannya. Dengan menggabungkan langkah-langkah tersebut, berbagai aplikasi yang relevan dapat diimplementasikan. Berikut adalah pengembangan rinci dan detail tentang aplikasi-aplikasi tersebut:

- Pengembangan Kendaraan Otonom: Informasi yang diperoleh dari pengolahan citra marka jalan sangat penting dalam pengembangan kendaraan otonom. Dengan mendeteksi dan memahami marka jalan, kendaraan otonom dapat menavigasi jalan dengan lebih akurat dan aman. Penggunaan deteksi garis dan ekstraksi fitur marka jalan memungkinkan kendaraan untuk mengenali batas-batas jalan, mengikuti jalur yang tepat, dan beradaptasi dengan perubahan kondisi marka jalan. Informasi ini juga dapat digunakan untuk mengidentifikasi tanda lalu lintas, memperkirakan kecepatan maksimum yang diizinkan, dan mengambil keputusan yang tepat saat menghadapi situasi kompleks di jalan.

- Sistem Pengawasan Lalu Lintas: Pengolahan citra marka jalan dapat digunakan dalam sistem pengawasan lalu lintas untuk memantau dan mengelola lalu lintas. Dengan memonitor marka jalan, sistem dapat mendeteksi pelanggaran lalu lintas, seperti kendaraan yang keluar dari jalurnya atau menginjak marka jalan terlarang. Informasi ini dapat digunakan untuk memicu tindakan peringatan atau memberikan bukti bagi penegak hukum. Selain itu, analisis pola marka jalan dapat membantu dalam mengidentifikasi pola perilaku pengemudi, memprediksi kepadatan lalu lintas, atau mengoptimalkan pengaturan lampu lalu lintas.

- Perencanaan Lalu Lintas: Informasi tentang marka jalan yang diperoleh melalui pengolahan citra dapat digunakan dalam perencanaan lalu lintas. Pemetaan jalan yang akurat dan pemahaman tentang karakteristik marka jalan dapat membantu dalam perancangan rute, penempatan tanda-tanda lalu lintas, dan penentuan zona kecepatan. Analisis lebih lanjut mengenai kondisi marka jalan, seperti keausan atau kerusakan, juga penting dalam menentukan jadwal pemeliharaan atau perbaikan infrastruktur jalan. Dengan memanfaatkan data yang dihasilkan dari pengolahan citra marka jalan, perencanaan lalu lintas dapat menjadi lebih efisien, aman, dan sesuai dengan kebutuhan pengguna jalan.

- Pemeliharaan Infrastruktur Jalan: Pengolahan citra marka jalan juga berperan penting dalam pemeliharaan infrastruktur jalan. Dengan menganalisis kondisi marka jalan secara rutin, dapat diidentifikasi tanda-tanda keausan, kerusakan, atau hilangnya marka jalan. Informasi ini dapat digunakan untuk merencanakan tindakan perawatan.

*Langkah-langkah menyelesaikan project*

Koding tersebut adalah implementasi deteksi marka jalan pada gambar menggunakan beberapa teknik pengolahan citra. Berikut adalah pengertian dari kodingan tersebut:

1. Pertama, gambar dengan nama "Marka.jpeg" dibaca menggunakan `cv2.imread()` dan disimpan dalam variabel `image`.

2. Gambar tersebut kemudian dikonversi dari format warna BGR menjadi RGB menggunakan `cv2.cvtColor()`. Gambar asli yang sudah dikonversi disimpan dalam variabel `image_asli`.

3. Dilakukan pengaburan gambar dengan filter Gaussian menggunakan `cv2.GaussianBlur()` untuk mengurangi noise dan meningkatkan kualitas gambar yang akan diproses selanjutnya. Hasil pengaburan disimpan dalam variabel `blurred_frame`.

4. Konversi gambar yang sudah diaburkan ke ruang warna HSV menggunakan `cv2.cvtColor()`. Hal ini mempermudah dalam penanganan warna pada gambar.

5. Definisikan batas warna putih dalam format HSV menggunakan `lower_white` dan `upper_white` sebagai batas bawah dan atas. Selanjutnya, mask dibuat dengan memanfaatkan `cv2.inRange()` untuk mengisolasi marka jalan yang berwarna putih dalam gambar.

6. Menggunakan operator Canny (`cv2.Canny()`) pada mask untuk mendeteksi tepi pada gambar. Parameter 50 dan 100 adalah threshold yang digunakan untuk deteksi tepi.

7. Transformasi Hough Probabilistik (`cv2.HoughLinesP()`) digunakan untuk mendeteksi garis-garis pada gambar dengan memanfaatkan tepi yang telah dideteksi sebelumnya. Parameter seperti jarak resolusi, sudut resolusi, ambang batas, dan jarak maksimum antar-garis diatur sesuai kebutuhan.

8. Jika terdapat garis yang terdeteksi, gambar garis tersebut pada gambar asli menggunakan `cv2.line()`. Dalam koding tersebut, garis-garis tersebut digambar dengan warna hijau `(0, 255, 0)` dan ketebalan 75 piksel.

9. Gambar hasil deteksi marka jalan dikonversi kembali ke format warna RGB menggunakan `cv2.cvtColor()` dan disimpan dalam variabel `image_rgb`.

10. Terakhir, menggunakan `plt.subplots()` untuk membuat subplot dengan 2 kolom. Gambar asli ditampilkan pada subplot pertama dan diberi judul "Gambar Asli". Gambar hasil deteksi marka jalan ditampilkan pada subplot kedua dan diberi judul "Deteksi Marka Jalan". Akhirnya, `plt.show()` digunakan untuk menampilkan kedua gambar tersebut dalam satu jendela pop-up.

Dengan menjalankan koding tersebut, gambar asli dan gambar dengan marka jalan yang terdeteksi akan ditampilkan secara berdampingan.

*Jurnal Mengenai Deteksi Garis Marka Jalan*

chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://repository.its.ac.id/55764/7/02311440000047-Undergraduate_Thesis.pdf










