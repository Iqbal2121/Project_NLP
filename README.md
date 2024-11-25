# Dokumentasi Proyek Analisis Sentimen
# 1. Judul Proyek
Analisis Sentimen pada Ulasan Lazada (Lazada Indonesian Reviews)

# 2. Deskripsi
Proyek ini dirancang untuk melakukan analisis sentimen pada ulasan produk Lazada dalam bahasa Indonesia. Melalui preprocessing teks, model machine learning digunakan untuk mengklasifikasikan sentimen ulasan sebagai positif atau negatif. Proyek ini bertujuan membantu bisnis memahami opini pelanggan secara lebih efektif.

# 3. Fitur Utama
Preprocessing Teks: Pembersihan, tokenisasi, dan representasi teks dengan teknik seperti TF-IDF atau word embeddings.
Klasifikasi Sentimen: Model yang digunakan meliputi SVC dan KNN.
Evaluasi Model: Hasil analisis dilengkapi dengan metrik evaluasi seperti akurasi, precision, recall, F1-score.
Visualisasi Data: Confusion matrix.

# 4. Persyaratan
Python >= 3.8
Library yang diperlukan:
numpy, pandas, scikit-learn
nltk, matplotlib, seaborn
Dataset Lazada Indonesian Reviews dari Kaggle.

# 5. Hasil Preprocessing
Proses preprocessing adalah langkah awal untuk mempersiapkan data teks agar dapat digunakan dalam analisis sentimen. Dataset Lazada Indonesian Reviews terdiri dari ulasan pelanggan dalam bahasa Indonesia. Langkah-langkah yang dilakukan selama preprocessing mencakup:
-  Pembersihan Data Teks
    a. Semua teks diubah menjadi huruf kecil untuk memastikan konsistensi.
    b. Tanda baca, angka, dan karakter khusus dihapus agar teks lebih bersih.
    c. Stopwords (kata-kata umum seperti "yang", "dan", "di") dihapus menggunakan daftar stopwords Bahasa Indonesia.
-  Tokenisasi dan Stemming
    a. Teks dipecah menjadi kata-kata (tokenisasi) agar lebih mudah diproses.
    b. Kata-kata diubah menjadi bentuk dasarnya (stemming) menggunakan library NLP seperti Sastrawi.
-  Representasi Data
Setelah preprocessing, teks direpresentasikan dalam bentuk fitur numerik. Teknik yang digunakan:
TF-IDF (Term Frequency-Inverse Document Frequency) untuk menghitung bobot pentingnya setiap kata dalam ulasan.

# 6. Hasil Klasifikasi
Setelah preprocessing, dataset yang telah diproses digunakan untuk melatih model. Berikut hasil klasifikasi yang dicapai:
-  Model yang Digunakan
    a. Support Vector Machines digunakan sebagai model baseline.
    b. Model lain seperti K-Nearest Neighbors (KNN) juga diimplementasikan untuk membandingkan performa.
-  Evaluasi Model
Model dievaluasi menggunakan beberapa metrik utama:
  a. Akurasi: Persentase prediksi benar dari keseluruhan dataset.

## hasil evaluasi (menggunakan SVC):
-  Akurasi: 93%
-  Confusion Matrix
    Confusion matrix menunjukkan performa model dalam memprediksi kelas sentimen:
      Prediksi Positif    | Prediksi Negatif
      Positif Benar: 2525 | Positif Salah: 130
      Negatif Salah: 245  | Negatif Benar: 2446

## hasil evaluasi (menggunakan KNN):
-  Akurasi: 85%
-  Confusion Matrix
    Confusion matrix menunjukkan performa model dalam memprediksi kelas sentimen:
      Prediksi Positif    | Prediksi Negatif
      Positif Benar: 2334 | Positif Salah: 321
      Negatif Salah: 457  | Negatif Benar: 2234


# 7. Kesimpulan


# 10. Lisensi
Proyek ini dilisensikan di bawah MIT License.

