# 🥩 Meat Clustering: PCA & K-Means Analysis
> Proyek Computer Vision Daging Sapi, Babi, dan Oplosan.

DATASET : https://drive.google.com/drive/folders/1UVYBMiS-a7zFldHevt-t-G-UfGzWxz40?usp=sharing

## 📌 Deskripsi Proyek
Proyek ini dikembangkan sebagai bagian dari tugas **Computer Vision**. Fokus utamanya adalah menerapkan teknik *Unsupervised Learning* untuk mengelompokkan citra daging ke dalam tiga kategori: **Daging Sapi**, **Daging Babi**, dan **Daging Oplosan**. 

Dengan menggunakan **Principal Component Analysis (PCA)** untuk reduksi dimensi dan **K-Means Clustering** untuk pengelompokan, sistem ini mampu mengenali kemiripan fitur visual antar gambar tanpa memerlukan label pada proses pembelajarannya.

## 🛠️ Teknologi yang Digunakan
- **Python**: Bahasa pemrograman utama.
- **OpenCV**: Library pengolahan citra (preprocessing, resizing, color conversion).
- **Scikit-Learn**: Implementasi algoritma ML (PCA, K-Means, StandardScaler).
- **Pandas & NumPy**: Manipulasi data dan manajemen matriks.
- **Matplotlib**: Visualisasi grafik scatter plot dan sampel gambar.

## 🚀 Metodologi
Proyek ini mengikuti alur kerja *Machine Learning* tradisional sebagai berikut:

1.  **Preprocessing**: Gambar diubah ukurannya menjadi $64 \times 64$ piksel dan dikonversi ke format warna RGB.
2.  **Flattening**: Matriks gambar dipipihkan menjadi array 1 dimensi.
3.  **Standardization**: Penyesuaian skala fitur menggunakan `StandardScaler`.
4.  **Reduksi Dimensi (PCA)**: Menyusutkan ribuan fitur piksel menjadi 2 komponen utama (PC1 & PC2) untuk menghilangkan *noise* dan memudahkan visualisasi.
5.  **Clustering (K-Means)**: Pengelompokan otomatis ke dalam $K=3$ klaster berdasarkan jarak *Euclidean*.

## 📊 Hasil dan Visualisasi
Hasil akhir proyek mencakup:
- **Scatter Plot**: Representasi visual persebaran data daging dalam koordinat 2D.
- **Cluster Samples**: Menampilkan sampel gambar dari tiap klaster untuk memverifikasi akurasi pengelompokan.
- **Export Data**: Seluruh koordinat fitur dan hasil klaster disimpan dalam format `.xlsx` (Excel) untuk analisis lebih lanjut.
