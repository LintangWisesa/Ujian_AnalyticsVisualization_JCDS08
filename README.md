# Soal Ujian Data Science - Data Analytics & Visualization

![Lintang_Purwadhika](https://static.wixstatic.com/media/2e6af2_f69a4271c3534ae1869a7ed63e278b2b~mv2.png/v1/fill/w_246,h_39,al_c,usm_0.66_1.00_0.01/2e6af2_f69a4271c3534ae1869a7ed63e278b2b~mv2.png)

## **Soal 1 - Distributor Die Cast 🚗**

![hotwheels](https://drimjuguetes.vteximg.com.br/arquivos/banner-landing-hotwheels.jpg)

Anda adalah distributor ternama di bidang jual-beli _die cast_ (miniatur moda transportasi) yang menjual beragam produk dari vendor-vendor berkualitas,
dengan 7 kantor cabang tersebar di beberapa negara dunia. Disediakan database
yang menyimpan berbagai data terkait usaha Anda, mulai dari daftar customer, karyawan, produk hingga transaksi yang dilakukan. 

Unduh database __.sql__ di repo ini ([_**/database/retrowheels.sql**_](/database)) dan import ke local MySQL server Anda. Tata cara import database juga tercantum di folder: ([_**/database**_](/database)). Kemudian selesaikan soal-soal berikut. Anda __dilarang keras__ mengubah struktur & format tabel serta database yang telah disediakan.

1. Rumuskan _single query_ untuk menampilkan jumlah __total customer__ yang Anda layani, beserta jumlah __total kota & negara asal__ customer-customer Anda. Contoh output yang diharapkan:

    ```bash
    +-----------+--------+-----------+
    | Customers | Cities | Countries |
    +-----------+--------+-----------+
    |       122 |     95 |        27 |
    +-----------+--------+-----------+
    ```

    Anda memiliki __122 customer__ dari __95 kota__ yang tersebar di __27 negara__!

2. Rumuskan _single query_ untuk menampilkan _resources_ yang Anda miliki, mulai dari jumlah __karyawan__, jumlah __kantor & lokasi negaranya__, jumlah __barang yang dijual__, total __stok barang__ & jumlah __vendor__ yang menjadi partner Anda. Contoh output yang diharapkan:

    ```bash
    +-----------+---------+---------+----------+---------------+---------+
    | Employees | Offices | Country | Products | StockProducts | Vendors |
    +-----------+---------+---------+----------+---------------+---------+
    |        23 |       7 |       5 |      110 |        555131 |      13 |
    +-----------+---------+---------+----------+---------------+---------+
    ```

    Anda memiliki __23 karyawan__ di __7 kantor__ yang berada di __5 negara__, dengan __110 model die cast__ (total stok mencapai __555131 item__) yang didistribusikan dari __13 vendor partner__.

3. Dari soal sebelumnya tercatat Anda memiliki __110 model die cast__ dengan total stok __555131 item__. Jika dikategorikan, produk yang Anda jual terbagi menjadi __7 product line__ _die cast_, yakni model mobil klasik, mobil _vintage_, sepeda motor, pesawat terbang, kapal laut, kereta api serta truk & bus. Rumuskan _single query_ yang dapat menampilkan __harga produk terendah & tertinggi__ untuk masing-masing kategori. Contoh output yang diharapkan:

    ```bash
    +------------------+----------+----------+
    | productLine      | minPrice | maxPrice |
    +------------------+----------+----------+
    | Classic Cars     |    15.91 |   103.42 |
    | Motorcycles      |    24.14 |    91.02 |
    | Planes           |    29.34 |    77.27 |
    | Ships            |    33.30 |    82.34 |
    | Trains           |    26.72 |    67.56 |
    | Trucks and Buses |    24.92 |    84.76 |
    | Vintage Cars     |    20.61 |    86.70 |
    +------------------+----------+----------+
    ```

4. Rumuskan _single query_ yang dapat menampilkan daftar 10 customer paling _royal_ (paling banyak mendatangkan uang bagi kita), yang total nominal transaksinya paling tinggi. Data yang ditampilkan adalah nama customer, kota & negara asal, beserta total uang yang dihabiskan di produk kita. Contoh output yang diharapkan:

    ```bash
    +------------------------------+---------------+-------------+-----------+
    | customerName                 | city          | country     | total     |
    +------------------------------+---------------+-------------+-----------+
    | Euro+ Shopping Channel       | Madrid        | Spain       | 715738.98 |
    | Mini Gifts Distributors Ltd. | San Rafael    | USA         | 584188.24 |
    | Australian Collectors, Co.   | Melbourne     | Australia   | 180585.07 |
    | Muscle Machine Inc           | NYC           | USA         | 177913.95 |
    | Dragon Souveniers, Ltd.      | Singapore     | Singapore   | 156251.03 |
    | Down Under Souveniers, Inc   | Auckland      | New Zealand | 154622.08 |
    | AV Stores, Co.               | Manchester    | UK          | 148410.09 |
    | Anna's Decorations, Ltd      | North Sydney  | Australia   | 137034.22 |
    | Corporate Gift Ideas Co.     | San Francisco | USA         | 132340.78 |
    | Saveley & Henriot, Co.       | Lyon          | France      | 130305.35 |
    +------------------------------+---------------+-------------+-----------+
    ```

5. Pada __2003-06-05__, terdapat pembayaran masuk sebesar __US$ 14571.44__. Tampilkan data seputar transaksi tersebut, mencakup __nama customer__ yang melakukan pembayaran, __nama produk__ yang dibeli, __jumlah tiap produk__ yang dibeli dan __harga satuannya__. Pastikan
total harga yang dibeli sesuai dengan data pembayaran masuk. Output yang diharapkan:

    ```bash
    +-------------------+--------------------------------+-----------------+-----------+
    | customername      | productname                    | quantityOrdered | priceEach |
    +-------------------+--------------------------------+-----------------+-----------+
    | Atelier graphique | 1965 Aston Martin DB5          |              26 |    120.71 |
    | Atelier graphique | 1999 Indy 500 Monte Carlo SS   |              46 |    114.84 |
    | Atelier graphique | 1948 Porsche Type 356 Roadster |              34 |    117.26 |
    | Atelier graphique | 1966 Shelby Cobra 427 S/C      |              50 |     43.27 |
    +-------------------+--------------------------------+-----------------+-----------+
    ```

    Jika Anda cek jumlah total dari ```quantityOrdered``` dikali ```priceEach``` dari tabel di atas, hasilnya __14571.44__. Dan transaksi pembayaran tersebut terjadi tepat pada tanggal __2003-06-05__.

✅ _Kirim & lampirkan jawaban soal ini dalam bentuk text (__.txt__) via email ke lintang@purwadhika.com_ dengan subject email "_NamaLengkap_DieCast_".

<hr>

## **Soal 2 - World Happiness 😄**

Disediakan dataset laporan tingkat kebahagiaan di berbagai negara di dunia, unduh di sini: [World Happiness](https://www.kaggle.com/unsdsn/world-happiness#2019.csv). Gunakan hanya dataset _2019.csv_, lalu buatlah sebuah file _notebook_ (__.ipynb__) dan selesaikanlah beberapa soal berikut:

1. Untuk setiap numerik _feature/column_ (kecuali column ```Overall Rank```), hitunglah:
    - Mean, Median dan Modus
    - Range, Q1, Q3 dan IQR
    - Standard Deviasi & Variance
    - Z-score tiap data point

2. Untuk setiap numerik _feature/column_ (kecuali column ```Overall Rank```), carilah _data outlier_-nya berdasarkan:
    - IQR method
    - Z-score method

3. Tampilkan sebaran masing-masing numerik _feature/column_ (kecuali column ```Overall Rank```) dalam bentuk _boxplot_ dan _histogram_!

4. Di antara semua numerik _feature/column_ (kecuali column ```Overall Rank```), _feature/column_ mana saja yang sangat mempengaruhi _happiness score_ suatu negara? Buktikan dengan menghitung nilai:
    - Covariance
    - Pearson Correlation
    - Spearman Correlation
    - Kendall Correlation

5. Visualisasikan dalam bentuk _bar chart_ data berikut:
    - 10 Negara dengan _GDP per capita_ tertinggi.
    - 10 Negara dengan _Healthy life expectancy_ tertinggi.
    - 10 Negara dengan _Perceptions of corruption_ tertinggi.

✅ _Push & commit jawaban Anda ke sebuah repo github dengan nama __Soal2_WorldHappiness__. Kirim & lampirkan url repo github Anda via email ke lintang@purwadhika.com_ dengan subject email "_NamaLengkap_WorldHappiness_".

<hr>

## **Soal 3 - Indonesia Covid-19 Maps 🌏**

Jumlah kasus infeksi virus corona Covid-19 masih terus mengalami peningkatan. Hingga Minggu (29/3/2020) sore, jumlah kasus infeksi Covid-19 yang telah dilaporkan di seluruh dunia adalah sebanyak __669.312 kasus__ dengan __145.609 pasien sembuh__ dan __31.700 meninggal dunia__. Wabah ini telah dilaporkan di lebih dari 170 negara di dunia, termasuk Indonesia.

Disediakan:
- Data sebaran Covid-19 tiap provinsi di Indonesia: [klik sini](https://en.wikipedia.org/wiki/2020_coronavirus_pandemic_in_Indonesia), untuk mengaksesnya silakan gunakan teknik _web scraping_.
- Data lokasi latitude & longitude tiap provinsi di Indonesia: [klik sini](https://raw.githubusercontent.com/LintangWisesa/Indonesia-Covid19-Maps/master/data/gps_indonesia.json), untuk mengaksesnya silakan lakukan GET request ke ```https://raw.githubusercontent.com/LintangWisesa/Indonesia-Covid19-Maps/master/data/gps_indonesia.json```.

Dengan data tersebut, buatlah sebuah peta sebaran Covid-19 per provinsi di Indonesia, dengan minimum requirements sebagai berikut:
- Tampilkan _marker_ di setiap provinsi.
- Saat _marker_ diklik akan menampilkan _popup message_ total kasus, pasien sembuh & kematian akibat Covid-19 di provinsi tersebut.
- Jawaban yang diminta berupa 1 file _notebook_ (__.ipynb__) berisi proses ekstraksi & data cleaning, beserta 1 file _html_ peta sebaran Covid-19 per provinsi (__.html__). 
- Contoh output dapat Anda simak di [bit.ly/cov19id](http://bit.ly/cov19id). Tampilan tidak harus sama, utamakan fitur.

✅ _Push & commit jawaban Anda ke sebuah repo github dengan nama __Soal3_Covid19__. Kirim & lampirkan url repo github Anda via email ke lintang@purwadhika.com_ dengan subject email "_NamaLengkap_Covid19_".

<hr>

🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸🔸

# Remedial Ujian Python Data Analytics & Visualization

### **Soal - 🍔 Nutrisi McD 🍟**

Disediakan dataset daftar nutrisi tiap menu di McDonald, unduh di sini: [Nutrition Facts for McDonald's Menu](https://www.kaggle.com/mcdonalds/nutrition-facts). Buatlah sebuah file _notebook_ (__.ipynb__) dan selesaikanlah beberapa soal berikut:

1. Untuk _feature/column_ ```Serving Size```, ```Calories```, & ```Total Fat``` hitunglah:
    - Mean, Median dan Modus
    - Range, Q1, Q3 dan IQR
    - Standard Deviasi & Variance
    - Z-score tiap data point

2. Untuk _feature/column_ ```Serving Size```, ```Calories```, & ```Total Fat``` carilah _data outlier_-nya berdasarkan:
    - IQR method
    - Z-score method

3. Untuk menu dengan kategori ```Coffee & Tea```, ```Breakfast```, ```Chicken & Fish```, ```Beef & Pork``` & ```Snacks & Sides```, tampilkan sebaran data dalam bentuk _boxplot_ dan _histogram_ untuk _feature/column_ ```Serving Size```, ```Calories```, & ```Total Fat```.

4. Untuk menu dengan kategori ```Coffee & Tea```, ```Breakfast```, ```Chicken & Fish```, ```Beef & Pork``` & ```Snacks & Sides```, visualisasikan dalam bentuk _bar chart_ data berikut:
    - 5 Menu dengan ```Serving Size``` tertinggi tiap kategori.
    - 5 Menu dengan ```Calories``` tertinggi tiap kategori.
    - 5 Menu dengan ```Total Fat``` tertinggi tiap kategori.

_**Catatan:**_ 

✅ Commit & push source code jawaban soal ini ke __Github__ Anda, buatlah repo dengan nama __Nutrisi_McD__, kemudian lampirkan __url link repo Github__ Anda via email ke _lintang@purwadhika.com!_

<hr>

### *__#HappyCoding__* :relaxed:

#### Lintang Wisesa :love_letter: _lintangwisesa@ymail.com_

[Facebook](https://www.facebook.com/lintangbagus) | 
[Twitter](https://twitter.com/Lintang_Wisesa) |
[Google+](https://plus.google.com/u/0/+LintangWisesa1) |
[Youtube](https://www.youtube.com/user/lintangbagus) | 
:octocat: [GitHub](https://github.com/LintangWisesa) |
[Hackster](https://www.hackster.io/lintangwisesa)