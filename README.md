# Stroke Predicition

## Domain Proyek

Stroke adalah sebuah penyakit yang telah menjadi momok bagi masyarakat luas. Meskipun stroke sudah lama dikenal oleh masyarakat tetapi kita masih susah dalam mengetahui kapan dan di mana kita akan mendapati penyakit stroke. Menurut [Organisasi Kesehatan Dunia (WHO)](https://www.who.int/news-room/fact-sheets/detail/the-top-10-causes-of-death) stroke adalah penyebab kematian ke-2 secara global dan bertanggung jawab atas sekitar 11% dari total kematian tersebut.

![ss0](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055850/Random/ss0_dj72ig.png)

Dengan adanya machine learning ini, diharapkan kita dapat mengetahui apakah kita mendapati penyakit tersebut atau tidak. Dengan memasukkan beberapa parameter seperti gender, usia, penyakit, dll.

## Business Understanding

### Problem Statements

Stroke sering kali melanda manusia kapan pun dan di mana pun. Stroke sendiri adalah penyakit yang sulit kali untuk diprediksi oleh manusia. Apakah dengan bantuan machine learning, kita bisa memprediksi adanya penyakit stroke tersebut?

### Goals

Tujuan dari projek ini adalah untuk memprediksi apakah pasien tersebut mendapati penyakit stroke atau tidak dengan dengan memasukkan beberapa parameter yang sudah tersedia.

### Solution statements

Solusi kali ini adalah dengan menggunakan machine learning, diharapkan manusia dapat mengetahui apakah dia sedang terjangkit stroke atau tidak. Saya akan menggunakan lima metode machine learning yaitu:

-   **Support Vector Machine** \
    Support Vector Machine adalah algoritma machine learning yang memungkinkan kita memprediksi suatu masukkan dengan cara dengan memasukkan konsep kernel pada ruang berdimensi tinggi. Kernel disini maksudnya layaknya membagi setiap koloni dengan menarik garis pemisah antara kelas satu dan kelas lainnya.

    ![ss12](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055852/Random/ss12_y3nteu.png)

-   **Naive Baiyes** \
    Naive Baiyes adalah algoritma machine learning yang memungkinkan kita memprediksi suatu masukkan dengan cara dengan menghitung peluang dari satu kelas dari masing-masing kelompok atribut yang ada dan memntukan kelas mana yang paling optimal.

    ![ss13](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055853/Random/ss13_skdgum.png)

-   **Decision Tree** \
    Decision Tree adalah algoritma machine learning yang memungkinkan kita memprediksi suatu masukkan dengan cara dimulai dengan satu node kemudian node tersebut bercabang untuk menyatakan pilihan-pilihan yang ada.

    ![ss14](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055854/Random/ss14_iwyebh.jpg)

-   **Logistic Regression** \
    Logistic Regression adalah algoritma machine learning yang memungkinkan kita memprediksi suatu masukkan dengan cara mencari hubungan antara fitur (input) diskrit dengan probabilitas hasil output diskrit tertentu.

    ![ss15](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055854/Random/ss15_tvkb43.png)

-   **Random Forest** \
    Random Forest adalah algoritma machine learning yang memungkinkan kita memprediksi suatu masukkan dengan cara dengan berawal dari memecah data sampel yang ada kedalam decision tree secara acak.

    ![ss16](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055854/Random/ss16_lemvpk.jpg)

## Data Understanding

Dataset ini saya ambil dari situs kaggle yang berjudul [Stroke Predicition Dataset.](https://www.kaggle.com/fedesoriano/stroke-prediction-dataset) Dataset ini dibuat oleh seseorang dengan nama *fedesoriano* dan sudah diunggah ke situs kaggle mulai bulan februari 2021. Dalam dataset tersebut terdapat beberapa fitur, diantaranya adalah:

1. id: Untuk identifikasi setiap pasien.
2. gender: Kelamin dari pasien yaitu "Male", "Female" atau "Other".

    ![ss1](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055850/Random/ss1_drxrps.png)

    ![ss17](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055853/Random/ss17_gwjlls.png)

3. age: Umur dari pasien.

    ![ss8](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055851/Random/ss8_rhq1oj.png)

4. hypertension: 0 jika pasien tidak punya hipertensi, 1 jika pasien punya hipertensi.

    ![ss6](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055851/Random/ss6_dg3bag.png)

    ![ss22](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055855/Random/ss22_wfnqes.png)

5. heart_disease: 0 jika pasien tidak punya serangan jantung, 1 jika pasien punya serangan jantung.

    ![ss7](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055851/Random/ss7_g7f5rl.png)

    ![ss23](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055855/Random/ss23_fbx8ql.png)

6. ever_married: Apakah pasien sudah menikah? "No" atau "Yes".

    ![ss2](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055850/Random/ss2_e3cawg.png)

    ![ss18](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055854/Random/ss18_uvylcn.png)

7. work_type: Tipe pekerjaan pasien yaitu "children", "Govt_jov", "Never_worked", "Private" atau "Self-employed".

    ![ss3](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055850/Random/ss3_hnvpfx.png)

    ![ss19](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055854/Random/ss19_yrhpkn.png)

8. Residence_type: Tempat tinggal pasien yaitu "Rural" atau "Urban".

    ![ss4](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055851/Random/ss4_qlqhgp.png)

    ![ss20](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055854/Random/ss20_hml59o.png)

9. avg_glucose_level: rata-rata nilai gula dalam darah.

    ![ss9](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055851/Random/ss9_lutxhz.png)

10. bmi: Index massa tubuh.

    ![ss10](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055852/Random/ss10_ynecw7.png)

11. smoking_status: Status merokoknya yaitu "formerly smoked", "never smoked", "smokes" atau "Unknown".

    > **Note**: Unknown disini data tersebut tidak tersedia pada pasien

    ![ss5](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055851/Random/ss5_bkp9ko.png)

    ![ss21](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055854/Random/ss21_tgnm0q.png)

12. stroke: 1 jika pasien punya stroke atau 0 jika pasien tidak punya stroke.

    ![ss11](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055852/Random/ss11_km5sfm.png)

## Data Preparation

1. Pertama saya rubah semua nama kolom menjadi huruf kecil untuk mempermudah dalam pengerjaan.
2. Setelah itu, saya hapus daya yang sama dan saya ganti semua kolom data yang kosong dengan rata-rata nilai dari kolom tersebut.
3. Selanjutnya, saya lakukan adalah menghapus beberapa kolom yang tidak dibutuhkan yaitu id dam avg_glucose_level. Karena kedua tersebut, sangatlah tidak berkorelasi terhadap kolom yang lain.
4. Setelah itu, saya menghapus outliers data karena outliers data dapat menganggung performa model kita nanti. Karena data tersebut berbeda dari yang lain.
5. Kita rubah semua kolom kategorikal menjadi kolom numerik, karena model machine learning hanya menerima numerik sebagai masukkan.
6. Kita standarisasi data tersebut, supaya perbandingan jarak antar kolom satu dengan yang lain tidaklah jauh. Saya menggunakan StandardScaler pada scikit-learn yang memungkinkan standarisasi fitur dengan menghilangkan rata-rata dan penskalaan ke varians unit.
7. Kita split data kita menjadi data latih dan data tes, supaya model machine learning kita dapat mempelajari data baru yaitu tes, bukan hanya berkutat pada data latih.

## Modeling

Disini saya membuat lima model machine learning, yaitu Support Vector Machine, Decision Tree, Naive Baiyes, Logistic Regression, dan Random Forest. Saya menggunakan Support Vector Machine karena model ini seringkali digunakan dalam banyak klasifikasi. Saya menggunakan Naive Baiyes karena model ini dapat menghitung sebuah peluang antara kelas satu dan lainnya, itu dapat memudahkan kita untuk mengetahui komposisinya. Saya menggunakan Logistic Regression karena model ini simpel dan cepat dalam penerapannya tetapi untuk performa modelnya terbilang bagus. Saya menggunakan Random Forest karena model tersebut gabungan dari Decision Tree yang dapat menghilangkan kecenderungan memahami data latih.

## Evaluation

Metrik evaluasi adalah sebuah pengukur performa dari model tersebut bagus atau tidaknya. Disini saya menggunakan metrik evaluasi **Akurasi**, karena metrik tersebut sangatlah cocok dengan permasalahan kali ini. Akurasi adalah metrik yang biasa digunakan untuk model machine learning. Berikut adalah evaluasi model yang telah saya buat.

![ss24](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055855/Random/ss24_eo1zeu.png)

![ss25](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055855/Random/ss25_ruhs2y.png)

![ss26](https://res.cloudinary.com/hafidhsoekma/image/upload/v1633055855/Random/ss26_rv1emi.png)

Bisa dilihat dari diagram diatas, bahwasanya Logistic Regression dan Support Vector Machine memiliki performa yang hampir mirip dalam memprediksi penyakit stroke. Setiap model juga berhasil memprediksi dengan baik.
