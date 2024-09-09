# Penerapan Machine Learning dengan Pendekatan Supervised - KNN pada Bunga Iris

## Deskripsi

Proyek ini membahas penerapan machine learning dengan pendekatan _supervised learning_, menggunakan algoritma K-Nearest Neighbors (KNN). KNN adalah algoritma yang digunakan untuk klasifikasi dan regresi, namun lebih sering digunakan untuk klasifikasi. Algoritma ini bekerja dengan mengklasifikasikan data baru berdasarkan kemiripan dengan data dalam dataset yang sudah ada.

## Konsep Dasar KNN

- **KNN bekerja dengan mengklasifikasikan data baru berdasarkan tetangga terdekat di dataset (data training)**.
- **Proses kerja KNN**:
  1. Simpan semua data training.
  2. Hitung jarak antara data baru dengan semua data dalam set training.
  3. Pilih k tetangga terdekat.
  4. Klasifikasi dilakukan berdasarkan mayoritas kelas tetangga terdekat (untuk klasifikasi) atau rata-rata nilai tetangga (untuk regresi).

## Pemilihan Nilai k

- **k kecil**: Sensitif terhadap noise dan bisa menyebabkan overfitting.
- **k besar**: Mengurangi sensitivitas terhadap noise tapi bisa menyebabkan underfitting.
- Pemilihan nilai k yang tepat dilakukan melalui cross-validation.

## Kelebihan KNN

- Algoritma yang sederhana dan intuitif.
- Tidak memerlukan fase eksplisit pelatihan.
- Mudah diimplementasikan untuk klasifikasi multi-kelas.

## Kekurangan KNN

- Lambat untuk dataset yang besar.
- Sensitif terhadap skala fitur (perlu normalisasi atau standardisasi).
- Membutuhkan memori besar untuk menyimpan seluruh dataset.

## Studi Kasus: Klasifikasi Iris dengan KNN

Dalam studi kasus ini, dataset _Iris_ yang tersedia di _scikit-learn_ digunakan untuk mengklasifikasikan spesies bunga iris (setosa, versicolor, virginica) berdasarkan panjang dan lebar sepal serta petal. Dataset berisi 150 sampel dengan 4 fitur: panjang sepal, lebar sepal, panjang petal, dan lebar petal.

**Tugas**: Membuat program machine learning menggunakan KNN untuk mengklasifikasikan spesies bunga iris dengan bahasa Python.

## Dataset

Dataset Iris dapat diunduh dari [http://archive.ics.uci.edu](http://archive.ics.uci.edu). Dataset ini berisi pengamatan bunga iris yang dilakukan oleh ahli botani Anderson.

## Persyaratan

- Python 3.x
- Libraries:
  - Scikit-learn
  - Pandas
  - NumPy
  - Matplotlib

## Instalasi

1. Clone repository ini:
   ```bash
   git clone https://github.com/yourusername/knn-iris-classification.git
   ```
2. Masuk ke direktori proyek:
   ```bash
   cd knn-iris-classification
   ```
3. Install library yang diperlukan:
   ```bash
   pip install scikit-learn pandas numpy matplotlib
   ```

## Penggunaan:

1. Jalankan skrip KNN:
   ```bash
   python knn_iris.py
   ```
2. Program akan melakukan klasifikasi pada dataset Iris dan menampilkan hasilnya.

## Visualisasi KNN

- Proyek ini menyertakan visualisasi sederhana untuk menggambarkan cara kerja KNN, seperti bagaimana data baru diklasifikasikan berdasarkan tetangga terdekat.

## Lisensi

- Proyek ini dilisensikan di bawah MIT License.

@Copyright Veendy 2024
