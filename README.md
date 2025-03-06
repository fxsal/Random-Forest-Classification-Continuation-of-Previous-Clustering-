# Klasifikasi Data Menggunakan Random Forest (Lanjutan Clustering)

## 📌 Pendahuluan

Proyek ini merupakan lanjutan dari analisis clustering sebelumnya, di mana hasil clustering digunakan sebagai target untuk membangun model klasifikasi. Model yang digunakan adalah Random Forest Classifier, dengan evaluasi menggunakan metrik Akurasi, F1-Score, dan Confusion Matrix. Selain itu, dilakukan juga validasi silang (cross-validation) dan hyperparameter tuning untuk meningkatkan performa model.

## 📂 Dataset

Dataset yang digunakan adalah hasil clustering sebelumnya, yang disimpan dalam file fundamentals_clusters.csv. Dataset ini mengandung fitur-fitur numerik yang telah diproses sebelumnya, serta label cluster yang akan digunakan sebagai target klasifikasi.

## 🛠 Teknologi & Library

Proyek ini dibangun menggunakan bahasa Python dengan pustaka berikut:

pandas – Untuk manipulasi data

numpy – Untuk komputasi numerik

sklearn – Untuk preprocessing, klasifikasi, evaluasi, dan validasi silang

seaborn & matplotlib – Untuk visualisasi data dan hasil evaluasi

## 🔍 Metodologi

Persiapan Data

Memuat dataset hasil clustering

Memisahkan fitur (X) dan target (y)

Membagi data menjadi training set (80%) dan test set (20%)

Membangun Model Klasifikasi

Menggunakan Random Forest Classifier dengan parameter default

Melatih model menggunakan data training

Memprediksi data testing

Evaluasi Model

Menghitung Accuracy Score dan F1-Score

Menampilkan Classification Report untuk melihat performa model pada setiap kelas

Membuat Confusion Matrix untuk menganalisis kesalahan prediksi

Validasi Silang (Cross-Validation)

Menggunakan Stratified K-Fold (5 folds) untuk memastikan model tidak overfitting

Menghitung rata-rata akurasi dan F1-Score dari beberapa iterasi pelatihan

Hyperparameter Tuning

Menggunakan GridSearchCV untuk mencari kombinasi parameter terbaik

Melatih model ulang dengan parameter optimal dan membandingkan hasilnya dengan model awal

## 📊 Hasil & Visualisasi

Beberapa hasil utama dari klasifikasi ini meliputi:

Akurasi & F1-Score dari model awal dan setelah tuning

Confusion Matrix untuk analisis lebih lanjut

Perbandingan performa model sebelum dan sesudah tuning

## 🚀 Cara Menjalankan

Pastikan Anda memiliki Python 3.x dan pustaka yang diperlukan telah diinstal.

Clone repository ini:

git clone https://github.com/username/repository-name.git
cd repository-name

Install dependensi:

pip install -r requirements.txt

Jalankan script utama:

python classification_script.py

## 📌 Kesimpulan

Dengan menggunakan Random Forest Classifier, dataset hasil clustering berhasil diklasifikasikan dengan performa yang baik. Validasi silang dan tuning hyperparameter membantu dalam meningkatkan akurasi dan stabilitas model.
