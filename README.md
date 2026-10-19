# Exploratory Data Analysis: Student Dropout and Academic Success

Proyek ini berisi analisis eksploratif data (*Exploratory Data Analysis/EDA*) terhadap dataset **Predict Students' Dropout and Academic Success** dari UCI Machine Learning Repository. Analisis dilakukan menggunakan Python untuk memahami kualitas data, distribusi status akhir mahasiswa, serta pola hubungan antara karakteristik akademik dan status mahasiswa.

## Tujuan Analisis

- Memahami struktur, ukuran, dan tipe data pada dataset.
- Memeriksa nilai kosong dan baris duplikat.
- Membandingkan distribusi status akhir mahasiswa: **Dropout**, **Enrolled**, dan **Graduate**.
- Mengeksplorasi perbedaan nilai semester pertama, jumlah mata kuliah yang lulus, usia saat mendaftar, dan status akhir mahasiswa.
- Mengamati hubungan antara nilai akademik semester pertama dan kedua serta korelasi beberapa variabel numerik.

## Dataset

- **Nama:** Predict Students' Dropout and Academic Success
- **Sumber:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success)
- **Ukuran data:** 4.424 baris dan 37 kolom
- **Variabel target:** `Target`, dengan kategori Dropout, Enrolled, dan Graduate

Dataset diambil melalui pustaka `ucimlrepo`. Informasi lebih lanjut mengenai definisi variabel dapat dilihat pada halaman resmi dataset UCI.

## Tools dan Pustaka

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- ucimlrepo

## Tahapan Analisis

1. **Memuat dan memahami data** — memeriksa contoh data, ukuran dataset, tipe data, statistik deskriptif, nilai kosong, dan duplikat.
2. **Distribusi status akhir mahasiswa** — membandingkan jumlah dan persentase mahasiswa pada setiap kategori target.
3. **Karakteristik akademik** — membandingkan nilai semester pertama dan jumlah mata kuliah yang lulus berdasarkan status akhir.
4. **Hubungan nilai ant semester** — menggunakan korelasi Pearson dan scatter plot.
5. **Analisis usia dan gender** — mengeksplorasi distribusi status akhir berdasarkan usia saat mendaftar dan gender.
6. **Korelasi antarvariabel numerik** — menampilkan matriks korelasi dan heatmap untuk beberapa variabel akademik dan usia.

## Ringkasan Temuan

Berdasarkan hasil analisis pada notebook:

- **Graduate** merupakan kelompok terbesar, sebanyak 2.209 mahasiswa (49,93%), diikuti Dropout sebanyak 1.421 mahasiswa (32,12%) dan Enrolled sebanyak 794 mahasiswa (17,95%).
- Pemeriksaan awal menunjukkan tidak terdapat nilai kosong maupun baris duplikat identik.
- Kelompok Graduate memiliki rata-rata nilai semester pertama dan jumlah mata kuliah yang lulus lebih tinggi daripada kelompok Dropout.
- Nilai semester pertama dan kedua memiliki korelasi Pearson positif yang kuat, sekitar **0,837**.
- Rata-rata usia saat mendaftar pada kelompok Dropout lebih tinggi dibandingkan kelompok Enrolled dan Graduate.
- Dalam dataset ini, proporsi Dropout pada kelompok laki-laki lebih tinggi daripada kelompok perempuan.

Temuan tersebut bersifat **deskriptif dan tidak membuktikan hubungan sebab-akibat**. Proyek ini berfokus pada EDA dan tidak mencakup pembangunan model Machine Learning.

## Notebook Analisis

Buka notebook lengkap yang berisi kode, hasil analisis, dan visualisasi:

[**eda_student_dropout.ipynb**](./eda_student_dropout.ipynb)
