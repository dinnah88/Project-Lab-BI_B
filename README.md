# **DASBOR AKU ANAK SEHAT**

## **Backgrounds**
  Bayi dengan gizi buruk mendapat perhatian dari pemerintah sebab menyangkut kualitas penerus bangsa. Maka itu pemerintah mencanangkan program untuk menangani masalah gizi perseorangan dan meningkatkan status gizi masyarakat. Program ini tentu memerlukan pendanaan dan pemetaan prioritas area yang harus dengan segera ditangani. Maka dibutuhkan sebuah visualisasi data agar para pihak dapat menentukan area yang diutamakan.
Prevalensi kasus gizi buruk pada bayi khususnya di Jawa Barat menjadi pilihan kelompok kami untuk dieksplorasi lebih lanjut sehingga para pihak atau user dari pemerintahan bisa mendapat gambaran kabupaten dan kota mana saja yang harus diprioritaskan dalam penanganan kasus gizi buruk ini.



## **Objectives**
  Selain melihat pemetaan angka gizi buruk berdasarkan kota-kabupaten di Jawa Barat, user juga dapat melihat perbandingan angka gizi buruk pada bayi dengan angka kehamilan ibu, serta indeks kesehatan di tiap kota-kabupaten di Jawa Barat. Melihat perbandingan ketiga data tersebut bertujuan agar user dapat membuat program yang tepat sasaran seperti menggalakkan kembali program keluarga berencana sebagai usaha meningkatkan kualitas gizi di tiap unit keluarga.
	Visualisasi data yang dibuat ditujukan untuk personas seperti pembuat kebijakan di Kementerian Kesehatan yang akan berkoordinasi langsung dengan Dinas Kesehatan Kota dan Kabupaten, juga para peneliti kesehatan baik dari pemerintah maupun pihak NGO agar dapat membantu mendorong pembuatan kebijakan tata laksana dan tata kelola program penekanan angka gizi buruk pada bayi. Visualisasi akan disajikan dalam bentuk dasbor satu halaman dengan peta angka gizi buruk selama tahun 2016 hingga 2018, 10 kota-kabupaten dengan angka gizi buruk pada bayi tertinggi, perbandingan angka gizi buruk dengan kehamilan ibu di tahun yang sama, serta korelasi antara ketiga angka tersebut.



## **Methods**
- Eksplorasi serta wrangling 3 dataset dari situs Open Jabar yaitu Angka Gizi Buruk pada Bayi, Angka Kehamilan Ibu, serta Indeks Kesehatan dengan menggunakan excel sebab kami memilih Tableau Public sebagai platform visualisasi data yang menerima format excel;
- Menentukan metrics yang membantu user memetakan kasus angka gizi buruk serta keterikatan dengan data lainnya, serta fitur yang dapat memfilter tiap grafik untuk kemudahan penggunaan;
- Menentukan user flow serta membuat prototype grafik-grafik serta penempatan fitur yang diperlukan;
- Membuat dasbor dengan Tableau dan menghubungkan data Open Jabar dengan data geographical (shp) dari GADM 36 Indonesia.



## **Wrangling Data**
Karena kami menggunakan Tableau sebagai platform visualisasi data, kami menyatukan tiga dataset menggunakan excel dan berikut hasil akhirnya:

[](https://drive.google.com/uc?id=1ebAwVMz_NVWjRHBmbIbYMRVUlsRTit4v)


## **Exploratory Data Analysis (EDA)**
Untuk menampilkan data Angka Gizi Buruk tiap daerah, kami menggunakan geographical data shp dari GADM36 IDN. Data tersebut kami connect langsung di Tableau, sehingga grafik berupa peta dapat langsung ditampilkan. Selain itu, kami menampilkan angka statistik rerata dari tiap Kota-Kabupaten dan menjadikan peta sebagai filternya. Bar chart yang membandingkan Angka Gizi Buruk dengan Angka Kehamilan Ibu juga mengikuti perubahan sesuai Kota-Kabupaten yang dipilih. Perbandingan tersebut juga kami sajikan dalam bentuk scatter plot dan menampilkan garis linear regresi untuk melihat korelasi antar variabel data tersebut.

Kami juga menampilkan bar chart top 10 Kota-Kabupaten dengan Angka Gizi Buruk tertinggi untuk memudahkan user memetakan area mana saja yang harus diprioritaskan. 

## **Dashboard**
Saat dasbor dibuka, user dapat memilih periode tahun keseluruhan, 2016, 2017, hingga 2018 untuk melihat persebaran angka gizi buruk pada bayi di kota-kabupaten Jawa Barat. Intensitas warna pada peta menunjukkan tinggi atau rendah angka tersebut. Semakin gelap, semakin tinggi angka gizi buruk pada bayi di daerah tersebut.
	Pada grafik di bawah peta, kami menghadirkan 10 kota-kabupaten tertinggi dengan angka gizi buruk pada bayi. Grafik ini memberikan gambaran kota yang harus diprioritaskan pembuat kebijakan.
	Di kanan atas, tersedia statistik Angka Gizi Buruk, Angka Kehamilan Ibu, serta Indeks Kesehatan di Jawa Barat secara keseluruhan, juga dapat dilihat statistik setiap kota kabupaten dengan cara mengklik setiap kota-kabupaten di peta. User dapat melihat perbandingan angka gizi buruk dengan kehamilan ibu (dibagi 100) secara keseluruhan maupun setiap tahun yang dipilih. Dan di bawahnya, user dapat melihat korelasi antara angka gizi buruk, dengan kehamilan ibu maupun indeks kesehatan. Kami menyajikan garis linear model dan menampilkan kalkulasi garis model tersebut agar peneliti kesehatan dapat mendapat insight seberapa korelatif semua data tersebut.

[](https://drive.google.com/file/d/1LqQtLv3v9A_sXrWAK2O679mp8xszKsAh/view?usp=sharing)
[Dashboard AKU ANAK SEHAT](https://public.tableau.com/app/profile/bow6761/viz/pered/AKUANAKSEHAT)


## **Analysis**
Pada dasbor Aku Anak Sehat, terlihat persebaran angka gizi buruk pada bayi di Jawa Barat berdasarkan intensitas warna dari yang paling gelap (tinggi) ke yang paling cerah (rendah). Kabupaten Bogor menjadi daerah dengan angka gizi buruk tertinggi. Dilihat dari statistik serta grafik pendukungnya, pada tahun 2017 terjadi peningkatan signifikan pada angka gizi buruk bayi dibanding tahun 2016 maupun 2018. Peningkatan sebanyak 3,120 dalam waktu satu tahun tersebut perlu ditelaah lebih lanjut baik secara kualitatif maupun kuantitatif oleh petugas di lapangan agar faktor penentu terjadinya peningkatan tersebut dapat ditemukan dan diatasi secara tepat. Pada grafik model linear di bawahnya, kami memunculkan kalkulasi serta statistik dari korelasi antara rerata Angka Gizi Buruk dengan Angka Kehamilan Ibu (grafik di kanan bawah). Meski R-squared menunjukkan hasil 0.43 yang berarti tidak berkorelasi kuat, kami ingin menunjukkan bahwa faktor penentu terjadinya angka gizi buruk tentu lebih luas dan kompleks, melibatkan kepercayaan masyarakat tentang pengasuhan anak, pendidikan kedua orang tua, dan faktor lainnya.
[](https://drive.google.com/file/d/1C3lRtPyd2jyvUHjQ-z17ITO8GYhcOYj4/view)


## **Conclusion**
Hasil analisis dari dashboard berupa pemetaan prioritas daerah mana yang memerlukan tindakan cepat untuk mengatasi masalah gizi buruk. Ranking teratas berarti daerah dengan kabupaten/kota dengan kasus gizi buruk yang perlu diatasi terlebih dahulu. Selain menentukan prioritas pada daerah berdasarkan ranking, kita bisa melihat dengan jelas angka gizi buruk, kehamilan, dan indeks Kesehatan. Lalu membandingkan angka gizi buruk dengan jumlah kehamilan pertahun. Terakhir melihat korelasi antara angka gizi buruk dengan jumlah ibu hamil dan indeks Kesehatan. Dari beberapa hal tadi bisa diambil keputusan apakah memang gizi buruk memiliki korelasi dengan jumah kehamilan dan indeks kesehatan sehingga nantinya diharapkan bisa memberikan rekomendasi kebijakan dan atau program yang tepat sasaran seperti sosialisasi dan pelayanan KB.


## **Pendukung**

Sumber data:
   - [Gizi Buruk pada Bayi](https://opendata.jabarprov.go.id/id/dataset/jumlah-bayi-bergizi-buruk-berdasarkan-kabupatenkota-di-jawa-barat)
   - [Angka Kehamilan Ibu](https://opendata.jabarprov.go.id/id/dataset/jumlah-ibu-hamil-berdasarkan-kabupatenkota-di-jawa-barat)
   - [Indeks Kesehatan](https://opendata.jabarprov.go.id/id/dataset/indeks-kesehatan-berdasarkan-kabupatenkota-di-jawa-barat)
Prototype: [Figma](https://www.figma.com/file/rmsBXPltBVxcz7l9zXFdqT/PLBI-1-Kelompok-B?node-id=0%3A1)


## **Reference**
- [Berita Gizi Buruk](https://www.suara.com/health/2017/07/21/175333/miris-kasus-gizi-buruk-cuma-berjarak-4-km-dari-istana-batutulis)
- [PRD](https://docs.google.com/document/d/1OGMNvPq3yGQUeCsBurKHuxb64OxJBpL3zH0BxIrOpes/edit?usp=sharing)
- [Dashboard Ref](https://github.com/zak-af/Project-Lab-BI)
