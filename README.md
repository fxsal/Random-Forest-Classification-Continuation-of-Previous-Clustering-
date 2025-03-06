# Klasifikasi Data Menggunakan Random Forest (Lanjutan Clustering)

## 📌 Pendahuluan
Proyek ini merupakan lanjutan dari analisis **clustering** sebelumnya, di mana hasil clustering digunakan sebagai target untuk membangun model klasifikasi. Model yang digunakan adalah **Random Forest Classifier**, dengan evaluasi menggunakan metrik **Akurasi, F1-Score, dan Confusion Matrix**. Selain itu, dilakukan juga **validasi silang (cross-validation)** dan **hyperparameter tuning** untuk meningkatkan performa model.

## 📂 Dataset
Dataset yang digunakan adalah hasil clustering sebelumnya, yang disimpan dalam file `fundamentals_clusters.csv`. Dataset ini mengandung fitur-fitur numerik yang telah diproses sebelumnya, serta label cluster yang akan digunakan sebagai target klasifikasi.

## 🛠 Teknologi & Library
Proyek ini dibangun menggunakan bahasa **Python** dengan pustaka berikut:

- [`pandas`](https://pandas.pydata.org/) – Untuk manipulasi data
- [`numpy`](https://numpy.org/) – Untuk komputasi numerik
- [`scikit-learn`](https://scikit-learn.org/) – Untuk preprocessing, klasifikasi, evaluasi, dan validasi silang
- [`seaborn`](https://seaborn.pydata.org/) & [`matplotlib`](https://matplotlib.org/) – Untuk visualisasi data dan hasil evaluasi

## 🔍 Metodologi
### 1. Persiapan Data
- Memuat dataset hasil clustering
- Memisahkan fitur (`X`) dan target (`y`)
- Membagi data menjadi **training set (80%)** dan **test set (20%)**

### 2. Membangun Model Klasifikasi
- Menggunakan **Random Forest Classifier** dengan parameter default
- Melatih model menggunakan data training
- Memprediksi data testing

### 3. Evaluasi Model
- Menghitung **Accuracy Score** dan **F1-Score**
- Menampilkan **Classification Report** untuk melihat performa model pada setiap kelas
- Membuat **Confusion Matrix** untuk analisis kesalahan prediksi

### 4. Validasi Silang (Cross-Validation)
- Menggunakan **Stratified K-Fold (5 folds)** untuk memastikan model tidak overfitting
- Menghitung rata-rata akurasi dan F1-Score dari beberapa iterasi pelatihan

### 5. Hyperparameter Tuning
- Menggunakan **GridSearchCV** untuk mencari kombinasi parameter terbaik
- Melatih model ulang dengan parameter optimal dan membandingkan hasilnya dengan model awal

## 📊 Hasil & Visualisasi
Beberapa hasil utama dari klasifikasi ini meliputi:

- **Akurasi & F1-Score** dari model awal dan setelah tuning
- **Confusion Matrix** untuk analisis lebih lanjut
- **Perbandingan performa model sebelum dan sesudah tuning**

## 🚀 Cara Menjalankan
1. Pastikan Anda memiliki **Python 3.x** dan pustaka yang diperlukan telah diinstal.
2. Clone repository ini:
   ```sh
   git clone https://github.com/username/repository-name.git
   cd repository-name
   ```
3. Install dependensi:
   ```sh
   pip install -r requirements.txt
   ```
4. Jalankan script utama:
   ```sh
   python classification_script.py
   ```

## 📌 Kesimpulan
Dengan menggunakan **Random Forest Classifier**, dataset hasil clustering berhasil diklasifikasikan dengan performa yang baik. **Validasi silang dan tuning hyperparameter** membantu dalam meningkatkan akurasi dan stabilitas model.


---
Jika ada pertanyaan atau saran, silakan ajukan **issue** atau **pull request** di repository ini. 🚀

