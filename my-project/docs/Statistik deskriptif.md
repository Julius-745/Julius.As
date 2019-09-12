# Statistik deskriptif

#### 

## Pengertian

> Statistika deskriptif adalah metode pengumpulan dan penyajian data menjadi suatu gugus data sehingga menghasilkan informasi yang berguna.

​	Statistika deskriptif hanya memberikan data yang dia punyai dan sama sekali tidak menarik kesimpulan apapun tentang gugus induknya yang lebih besar. Contoh statistika deskriptif adalah data yang kumpulan data yang di peroleh akan tersaji dengan ringkas dan rapi serta dapat memberikan informasi inti dari kumpulan data yang ada seperti data table, diagram, grafik, dan besaran-besaran lainya di majalah atau koran yang memuat data seperti: ukuran pemusatan data, ukuran penyebaran data, serta kecenderungan suatu gugus data.



## Tipe Statistik Deskriptif

#### Mean(rata-rata)

​	Mean adalah *nilai rata-rata* dari beberapa buah data. Nilai mean dapat ditentukan dengan membagi jumlah data dengan banyaknya data.

​	Mean (rata-rata) merupakan suatu ukuran pemusatan data. Mean suatu data juga merupakan statistik karena mampu menggambarkan bahwa data tersebut berada pada kisaran mean data tersebut. Mean tidak dapat digunakan sebagai ukuran pemusatan untuk jenis data nominal dan ordinal.

​	Berdasarkan definisi dari mean adalah jumlah seluruh data dibagi dengan banyaknya data. Dengan kata lain jika kita memiliki N data sebagai berikut maka mean data tersebut dapat kita tuliskan sebagai berikut :

![](F:\Tugas\Penambangan Data\Penambangan_Data\1.JPG)

Dimana: x = data ke n x bar = x rata-rata = nilai rata-rata sampel n = banyaknya data

#### Median

​	Median menentukan letak tengah data setelah data disusun menurut urutan nilainya. Bisa juga *nilai tengah dari data-data yang terurut. Simbol untuk median adalah Me. Dengan median Me, maka 50% dari banyak data nilainya paling tinggi sama dengan Me, dan 50% dari banyak data nilainya paling rendah sama dengan Me. Dalam mencari median, dibedakan untuk banyak data ganjil dan banyak data genap. Untuk banyak data ganjil, setelah data disusun menurut nilainya, maka median Me adalah data yang terletak tepat di tengah. Median bisa dihitung menggunakan rumus sebagai berikut:

![](F:\Tugas\Penambangan Data\Penambangan_Data\2.JPG)

#### Modus

​	Modus adalah nilai yang sering muncul. Jika kita tertarik pada data frekuensi, jumlah dari suatu nilai dari kumpulan data, maka kita menggunakan modus. Modus sangat baik bila digunakan untuk data yang memiliki sekala kategorik yaitu nominal atau ordinal. Modus bisa dihitung menggunakan rumus sebagai berikut:

![](F:\Tugas\Penambangan Data\Penambangan_Data\3.JPG)

Dimana :

​	Mo = Modus L = Tepi bawah kelas yang memiliki frekuensi tertinggi (kelas modus) i = Interval kelas b1 = Frekuensi kelas modus dikurangi frekuensi kelas interval terdekat sebelumnya b2 = frekuensi kelas modus dikurangi frekuensi kelas interval terdekat sesudahnya

## Standart Deviasi

​	Standar Deviasi dan Varians Salah satu teknik statistik yg digunakan untuk menjelaskan homogenitas kelompok. Varians merupakan jumlah kuadrat semua deviasi nilai-nilai individual terhadap rata-rata kelompok. Sedangkan akar dari varians disebut dengan standar deviasi atau simpangan baku.

​	Standar Deviasi dan Varians Simpangan baku merupakan variasi sebaran data. Semakin kecil nilai sebarannya berarti variasi nilai data makin sama Jika sebarannya bernilai 0, maka nilai semua datanya adalah sama. Semakin besar nilai sebarannya berarti data semakin bervariasi. Standar Deviasi bisa didapat menggunakan rumus sebagai berikut:

![](F:\Tugas\Penambangan Data\Penambangan_Data\4.JPG)

Dimana :

x = data ke n x bar = x rata-rata = nilai rata-rata sampel n = banyaknya data

## Varians

​	Varians merupakan rata-rata dari selisih kuadrat tersebut merupakan suatu ukuran penyimpangan dari observasi. Simbol varians pada ukuran populasi sigma kuarat dan pada ukuran sample S2. Akar dari varians dinamakan standar deviasi atau simpangan baku. Varians bisa didapat menggunakan rumus sebagai berikut:

![](F:\Tugas\Penambangan Data\Penambangan_Data\5.JPG)

## Skewness

​	Skewness (*kemencengan*) adalah derajat ketidaksimetrisan suatu distribusi. Jika kurva frekuensi suatu distribusi memiliki ekor yang lebih memanjang ke kanan (dilihat dari meannya) maka dikatakan menceng kanan (positif) dan jika sebaliknya maka menceng kiri (negatif). Secara perhitungan, skewness adalah momen ketiga terhadap mean. Distribusi normal (dan distribusi simetris lainnya, misalnya distribusi t atau Cauchy) memiliki skewness 0 (nol). Skewness bisa dihitung menggunakan rumus sebagai berikut:

![](F:\Tugas\Penambangan Data\Penambangan_Data\6.JPG)

## Quartile

​	Quartile adalah nilai-nilai yang membagi segugus pengamatan menjadi empat bagian sama besar. Nilai-nilai itu, yang dilambangkan dengan Q1, Q2, dan Q3, mempunyai sifat bahwa 25% data jatuh dibawah Q1, 50% data jatuh dibawah Q2, dan 75% data jatuh dibawah Q3. Quartile bisa dihitung menggunakan rumus sebagai berikut:

![](F:\Tugas\Penambangan Data\Penambangan_Data\7.JPG)



## Penerapan statistik deskriptif menggunakan python

### Alat dan Bahan

​	Pada penerapan ini saya menggunakan 500 data random yang disimpan dalam bentuk .xlsx dan untuk mempermudah dalam penerapan tersebut, perlu disiapkan library python yang dapat didownload secara gratis.

dalam kasus ini library python yang digunakan adalah sebagai berikut:

1. pandas, digunakan untuk data manajemen dan data analysis.
2. scipy, berisi kumpulan algoritme dan fungsi matematika.

### Pertama

pada langkah ini kita memasukkan library yang telah disiapkan sebelumya

```python
import pandas as pd
from scipy import stats
```

### Kedua

Dan Selanjutnya memuat data excel yang telah di siapkkan

```python
df = pd.read_csv('sample_data.csv', sep=';')
```



### Ketiga

​	kemudian membuat data penyimpanan (*dictionary*) yang menampung nilai yang akan ditampilkan. selanjutnya mengambil data dari beberapa kolom pada csv dengan cara diiterasi serta menghitungnya dengan berbagai metode yang telah disiapkan oleh pandas itu sendiri. kemudian hasil tersebut di disimpan pada penyimpanan tadi

```python
data = {"Stats" : ['Min','Max','Mean','Standard Deviasi','Variasi','Skewnes',
                   'Quartile 1','Quartile 2', 'Quartile 3', 'Median','Modus']}
```

```python
for i in df.columns:
    data[i] = [df[i].min(), df[i].max(), df[i].mean(),
                round(df[i].std(), 2),round(df[i].var(), 2),
                round(df[i].skew(), 2), df[i].quantile(0.25),
                df[i].quantile(0.5), df[i].quantile(0.75),
                df[i].median(), stats.mode(df[i]).mode[0]]
```

### Keempat

Terakhir adalah menvisualisasikan hasil tersebut dalam bentuk dataframe

```python
tes = pd.DataFrame(data, columns = ['Stats'] + [x for x in df.columns])
tes
```

![](F:\Tugas\Penambangan Data\Penambangan_Data\9.JPG)





## Mencari Outliner

​	Outlier merupakan suatu nilai dari pada sekumpulan data yang lain atau berbeda dibandingkan biasanya serta tidak menggambarkan karakteristik data tersebut. Sebuah outlier mungkin karena variabilitas dalam pengukuran atau mungkin menunjukkan kesalahan eksperimental. Standarisasi Data deteksi data dengan standarisasi pada prinsipnya mengubah niali data menjadi bentuk Z, dengan menggunakan formula dari Z score, yaitu:

![](F:\Tugas\Penambangan Data\Penambangan_Data\8.JPG)

pada data xlsx tersebut saya lakukan modifikasi dengan memberikan data sampah yang pada berbagai kolom. dan dalam pencarian outlier ini saya menggunakan formula dari z score yang diterapkan pada python, yaitu sebagai berikut:

```python
def dekteksi_outlier(df_in):
    outliers = []
    threshold = 3
    for col_name in df_in:
        mean = df_in[col_name].mean()
        std = df_in[col_name].std()
        i=1
        for y in df_in[col_name]:
            z_score = (y - mean) / std
            if abs(z_score) > threshold:
                outliers.append([col_name,y,i])
            i+=1
    return outliers

for i in dekteksi_outlier(df):
    print('Data sampah',i[1],'dikolom',i[0],'pada baris',i[2])
```

Dari Fungsi diatas menghasilkan outliner dari data xlsx tersebut

![](F:\Tugas\Penambangan Data\Penambangan_Data\10.JPG)

