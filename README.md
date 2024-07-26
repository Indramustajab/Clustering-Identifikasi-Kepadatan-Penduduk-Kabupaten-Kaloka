># Clustering Identifikasi Kepadatan Penduduk Kabupaten Kaloka
> >Identifikasi pola-pola kepadatan penduduk yang ada di Kabupaten Kolaka

## Table of Contents

- [Permasalahan](#permasalahan)
- [Perbandingan alasan penggunaan K means](#perbadingan)
- [Grafik Dataset](#grafikDataset)
- [Conclusion](#conclusion)

## Permasalahan
Tujuan identifikasi untuk memperoleh pemahaman yang lebih dalam tentang sebaran populasi di Kabupaten Kolaka, yang akan memberikan dasar bagi pengambilan keputusan yang lebih baik terkait dengan pengembangan wilayah dan kebijakan publik. Variabel data yang akan digunakan mencakup informasi populasi, termasuk jumlah penduduk di setiap wilayah administratif, serta atribut lain yang penting seperti luas wilayah atau perkembangan ekonomi. Metode analisis akan menggunakan teknik clustering untuk mengelompokkan wilayah-wilayah dengan pola kepadatan penduduk yang serupa menjadi cluster-cluster yang berbeda. Teknik clustering seperti K-means, DBSCAN, atau Hierarchical Clustering mungkin akan digunakan. Data yang Dibutuhkan adalah data geografis yang mencakup informasi tentang lokasi dan jumlah penduduk di setiap bagian administratif Kabupaten Kolaka, serta atribut-atribut lain yang relevan. Nantinya hasil yang diharapkan yaitu pemetaan cluster kepadatan penduduk, yang akan membantu dalam memahami lebih baik distribusi populasi di Kabupaten Kolaka. Pemetaan ini akan berguna untuk mengenali daerah-daerah dengan kepadatan penduduk yang berbeda, serta peluang dan tantangan dalam pembangunan wilayah.

>## Perbandingan alasan penggunaan K means
>Perbandingan antara penggunaan K-means dengan metode lain dalam pemetaan penduduk:

>>K-Means vs Hierarchical Clustering
>>-	K-Means: Memerlukan jumlah cluster (K) yang ditentukan sebelumnya, cocok untuk data dengan cluster yang jelas dan berukuran seragam.
>>-	Hierarchical Clustering: Tidak memerlukan jumlah cluster yang ditentukan sebelumnya, menghasilkan dendrogram untuk memahami hubungan hierarkis di antara cluster, cocok untuk data dengan struktur cluster yang tidak jelas.

>>K-Means vs DBSCAN (Density-Based Spatial Clustering of Applications with Noise)
>>-	K-Means: Menghasilkan cluster yang berbentuk bulat dengan jelas, sensitif terhadap inisialisasi centroid, cocok untuk data dengan cluster yang terpisah secara jelas.
>>-	DBSCAN: Mengidentifikasi cluster berdasarkan kepadatan data, tidak memerlukan jumlah cluster yang ditentukan sebelumnya, dapat menangani cluster dengan bentuk dan ukuran yang beragam, cocok untuk data dengan cluster yang tidak teratur atau berbentuk non-bulat.

## Grafik Dataset
- Distributions
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/Grafik%20%20(1).png" width="400" height="200" /></td>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/Grafik%20%20(2).png" width="400" height="200" /></td>
  </tr>
</table>
Disini dapat dilihat dari 5 data yang disimulasikan memiliki grafik seperti gambar diatas. Dari jumlah penduduk memiliki keterikatan dengan nilai frekuensi begitu juga dengan luas wilayah yang saling berkaitan dengan nilai frekuensi juga.
<br></br>

- Categorical distributions
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/Grafik%20%20(3).png" width="400" height="200" /></td>
  </tr>
</table>
Berikut ini merupakan dari 5 daerah yang dibuat dalam bentuk diagram bar dengan acuan banyaknya penduduk dalam suatu wilayah dengan menggunakan frekuensi.
<br></br>

-  2-D distribusi
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/Grafik%20%20(4).png" width="400" height="200" /></td>
    
  </tr>
</table>
Berikut ini merupakan penempatan pointing dari setiap nilai luasan wilayah dari setiap nama daerah yang tertera
<br></br>

-   Values
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/Grafik%20%20(5).png" width="400" height="200" /></td>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/Grafik%20%20(6).png" width="400" height="200" /></td>
  </tr>
</table>
Dari gambar berikut ini dari 2 data set terlihat jika grafik diagram yang tergambarkan bahwa daerah yang memiliki sedikit penduduk masih sangat banyak dan luasan wilayah yang cukup kecil.
<br></br>

- Faceted distribution
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/Grafik%20%20(7).png" width="400" height="200" /></td>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/Grafik%20%20(8).png" width="400" height="200" /></td>
  </tr>
</table>

Penempatan grafik dari setiap wilayah dalam penggambaran garis yang berasal dari data tersebut dengan menempatkan nilai jumlah penduduk dari tiap-tiap daerah.
<br></br>

- Distribusi dari perhitungan rata-rata
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(30).png" width="400" height="200" /></td>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(31).png" width="400" height="200" /></td>
  </tr>
</table>
Berikut ini merupakan gambaran dari semua data yang ada dan menggunakan nilai rata-rata, minimal, penjumlahan, dan nilai maksimal. Dari gambar tabel tersebut merupakan hasil dari nilai jumlah penduduk menggunakan mean.
<br></br>

- 2-d distributions
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(29).png" width="400" height="200" /></td>
  </tr>
</table>

Berikut ini merupakan hasil dari pointing dalam bentuk 2D yang merupakan hasil dari luasan wilayah dalam bentuk nilai floating yang beracuan pada jumlah penduduk.
<br></br>

-   Values
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(28).png" width="400" height="200" /></td>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(27).png" width="400" height="200" /></td>
  </tr>
</table>

Grafik values tersebut terkait distribusi antara kedua variabel seperti sebaran data, pola konsentrasi data di sekitar nilai-nilai tertentu, serta apakah distribusi data tersebut normal atau tidak. 

Untuk Variabel “Jumlah”
-	Count: Jumlah total pengamatan yang tersedia untuk variabel “Jumlah”. Dalam kasus ini, terdapat 135 pengamatan.
-	Mean: Rata-rata dari variabel “Jumlah”. Nilainya adalah 1766.748148.
-	Std: Standar deviasi dari variabel “Jumlah”. Ini menunjukkan seberapa jauh nilai-nilai “Jumlah” tersebar dari rata-ratanya. Nilainya adalah 1624.108507.
-	Min: Nilai minimum dari variabel “Jumlah”. Nilai terendah adalah 261.
-	25%: Kuartil pertama dari variabel “Jumlah”. Ini menunjukkan nilai di mana 25% dari data berada di bawahnya. Nilainya adalah 870.5.
-	50%: Median dari variabel “Jumlah”. Nilai median (atau kuartil kedua) adalah 1263.
-	75%: Kuartil ketiga dari variabel “Jumlah”. Ini menunjukkan nilai di mana 75% dari data berada di bawahnya. Nilainya adalah 1973.
-	max: Nilai maksimum dari variabel “Jumlah”. Nilai tertinggi adalah 9078.

Untuk Variabel “Luas Wilayah”
-	Count: Jumlah total pengamatan yang tersedia untuk variabel "Luas Wilayah". Dalam kasus ini, juga terdapat 135 pengamatan.
-	Mean: Rata-rata dari variabel “Luas Wilayah”. Nilainya adalah 22.517778.
-	Std: Standar deviasi dari variabel “Luas Wilayah”. Nilainya adalah 26.768374.
-	Min: Nilai minimum dari variabel “Luas Wilayah”. Nilai terendah adalah 0.3.
-	25%: Kuartil pertama dari variabel “Luas Wilayah”. Nilainya adalah 4.34.
-	50%: Median dari variabel “Luas Wilayah”. Nilai median adalah 12.42.
-	75%: Kuartil ketiga dari variabel “Luas Wilayah”. Nilainya adalah 30.815.
-	Max: Nilai maksimum dari variabel “Luas Wilayah”. Nilai tertinggi adalah 134.38
<br></br>

- Print out pointing awal
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(26).png" width="400" height="200" /></td>
  </tr>
</table>
Berikut merupakan hasil analisa dari semua data dalam bentuk gambaran 2D menggunakan pointing yang disesuaikan dengan nilai dari data sebelumnya.
<br></br>

-  Clustering distribusi
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(25).png" width="400" height="200" /></td>
         <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(9).png" width="400" height="200" /></td>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(24).png" width="400" height="200" /></td>
 
  </tr>
</table>
Gambar berikut hasil dari penerapan data setelah dilakukan normalisasi data dan diubah dalam bentuk diagram batang sehingga dapat dilihat secara lebih jelas dari setiap daerah.
<br></br>

-  2D distribusi
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(23).png" width="400" height="200" /></td>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(22).png" width="400" height="200" /></td>
  </tr>
</table>
Sedangkan gambar berikut ini merupakan hasil pemetaan pointing dalam bentuk 2D. Dapat dilihat terdapat 2 simulasi gambar dengan pemetaan secara luas, sedangkan pada gambar bagian kanan merupakan hasil dari pointing linear.
<br></br>

-   Values
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(21).png" width="400" height="200" /></td>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(20).png" width="400" height="200" /></td>
     <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(19).png" width="400" height="200" /></td>
  </tr>
</table>
Gambar pertama merupakan hasil grafik dari continue, jumlah penduduk disetiap daerah dengan menggunakan acuan jumlah banyaknya daerah yang masuk.
Gambar kedua merupakan hasil grafik dari continue, luas wilayah yang memiliki acuan dengan banyak daerah yang sama dengan nilai dari setiap stepnya.
Gambar ketiga merupakan grafik dari clustering dari kedua data tersebut dengan memperhitungkan daerah mana saja yang termasuk dalam pusat pointing yang sudah di buat.
<br></br>

-   Print out K-Means
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(18).png" width="700" height="400" /></td>

  </tr>
</table>
Dari semua proses yang sudah dilakukan baik dari normalisasi data, pemetaan awal, dan lain-lain. Maka hasil output dari setiap proses tersebut ada dalam gambar diatas. Jika dilihat dari hasil akhir gambar tersebut, terdapat 3 titik utama sebagai titik acuan jarak terdekat dari tiap-tiap daerah yang ada. Sehingga dapat disimpulkan bahwa tiap-tiap daerah pasti memiliki suatu pusat yang memiliki jarak terdekat. Maka dari hasil tersebut dapat digunakan sebagai bahan pemerataan penduduk di setiap daerah yang ada sehingga di setiap daerah tidak ada penduduk yang memiliki warga yang begitu banyak atau mengurangi kepadatan penduduk.
<br></br>

-   Elbow Method
<table>
  <tr>
    <td><img src="https://github.com/Indramustajab/Clustering-Identifikasi-Kepadatan-Penduduk-Kabupaten-Kaloka/blob/main/Img%20Grafik/grafik%20%20(17).png" width="600" height="300" /></td>

  </tr>
</table>
Pada grafik Elbow Method tersebut, akan dicari titik di mana penurunan nilai CS mulai melambat secara signifikan, membentuk sudut yang mirip dengan siku pada siku. Titik ini menandakan jumlah klaster yang optimal untuk data tersebut. Pada jumlah klaster akan dipilih sesuai dengan titik siku yang tertera tersebut. Pada grafik, dapat dilihat jika grafik tersebut setelah jumlah klaster 3, penurunan nilai CS tidak lagi signifikan, maka akan dipilih 3 sebagai jumlah klaster yang optimal untuk model. Setelah menentukan jumlah klaster optimal, dapat dilanjutkan dengan menggunakan jumlah klaster tersebut untuk melakukan klasterisasi pada dataset.
<br></br>

## Conclusion
Hasil dari seluruh proses yang telah dilakukan, termasuk normalisasi data dan pemetaan awal, beserta langkah-langkah lainnya, tercermin dalam gambar yang ditampilkan di atas. Melalui analisis visual dari gambar akhir tersebut, dapat terlihat bahwa ada tiga titik pusat utama yang mewakili centroid dari setiap klaster yang dibentuk. Titik-titik ini berperan sebagai referensi jarak terdekat dari setiap daerah yang telah dikelompokkan ke dalam klaster. Dengan demikian, dapat diambil kesimpulan bahwa setiap daerah memiliki pusat klaster yang menjadi titik fokus terdekat bagi penduduk di daerah tersebut. Fenomena ini menunjukkan bahwa data populasi di berbagai daerah telah berhasil dikelompokkan ke dalam klaster dengan karakteristik yang serupa. Hasil klasterisasi ini dapat digunakan sebagai landasan untuk merencanakan pemerataan populasi di setiap daerah, dengan tujuan untuk mengurangi ketidakseimbangan jumlah penduduk yang mungkin terjadi atau kepadatan populasi yang berlebihan di suatu wilayah. Dengan demikian, pelaksanaan rencana pemerataan populasi berdasarkan hasil klasterisasi ini berpotensi membantu dalam menjaga distribusi penduduk yang lebih merata dan seimbang di seluruh wilayah.


