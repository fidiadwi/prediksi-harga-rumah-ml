# Prediksi Harga Rumah Menggunakan Machine Learning

## Deskripsi Proyek
Proyek ini bertujuan untuk memprediksi harga jual rumah menggunakan metode *Machine Learning*. Dataset yang digunakan adalah Ames Housing, yang berisi informasi penjualan rumah di Ames, Iowa, Amerika Serikat.
Proyek ini membandingkan dua model regresi, yaitu Linear Regression dan Random Forest Regressor, untuk mengetahui model yang memberikan hasil prediksi lebih baik berdasarkan data pengujian.

## Tujuan
1. Memahami karakteristik dataset penjualan rumah.
2. Melakukan eksplorasi dan preprocessing data.
3. Membangun model prediksi harga rumah menggunakan dua metode regresi.
4. Mengevaluasi dan membandingkan performa model.
5. Memvisualisasikan hasil prediksi dan fitur yang berpengaruh terhadap prediksi model.

## Dataset
Dataset: Ames Housing — House Prices: Advanced Regression Techniques.
Sumber: https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data
Target prediksi: `SalePrice` (harga jual rumah).
Catatan: Dataset ini berasal dari Amerika Serikat dan tidak secara langsung merepresentasikan harga rumah di Indonesia.

## Metode yang Digunakan
- Linear Regression
- Random Forest Regressor

## Tahapan Pengerjaan
1. Memuat dataset.
2. Memahami struktur dan statistik data.
3. Melakukan eksplorasi dan visualisasi.
4. Menangani nilai kosong dan mengolah fitur kategorikal.
5. Membagi data menjadi data pelatihan dan pengujian.
6. Melatih kedua model.
7. Mengevaluasi performa model.
8. Membandingkan harga aktual dengan hasil prediksi.
9. Menganalisis fitur penting dan menyimpan hasil.

## Evaluasi Model
Performa model dievaluasi menggunakan:
- **MAE (Mean Absolute Error):** mengukur rata-rata besar kesalahan prediksi.
- **RMSE (Root Mean Squared Error):** mengukur kesalahan dengan memberikan penalti lebih besar pada kesalahan yang besar.
- **R² Score:** mengukur kemampuan model dalam menjelaskan variasi target pada data pengujian.

Hasil evaluasi dapat dilihat pada file `hasil_proyek/evaluasi_model.csv`.

## Struktur Proyek
- `Prediksi_Harga_Rumah.ipynb` — notebook berisi kode dan proses analisis.
- `README.md` — dokumentasi proyek.
- `hasil_proyek/evaluasi_model.csv` — hasil evaluasi kedua model.
- `hasil_proyek/hasil_prediksi.csv` — perbandingan harga aktual dan prediksi.
- `hasil_proyek/feature_importance.csv` — tingkat kepentingan fitur pada model Random Forest.
- `hasil_proyek/ringkasan_hasil.txt` — ringkasan hasil evaluasi.
- `hasil_proyek/model_terbaik.joblib` — model yang dipilih berdasarkan MAE.

## Teknologi
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Google Colab

## Cara Menjalankan
1. Buka `Prediksi_Harga_Rumah.ipynb` menggunakan Google Colab.
2. Jalankan setiap cell kode secara berurutan.
3. Pastikan dataset dapat diakses dari sumbernya.
4. Periksa grafik dan hasil evaluasi yang dihasilkan.

## Catatan
Model terbaik ditentukan berdasarkan nilai MAE pada data pengujian. Hasil evaluasi hanya menggambarkan performa pada pembagian data yang digunakan dan tidak menjamin akurasi yang sama pada data lain.
