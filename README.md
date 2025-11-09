🏆 Machine Learning Competition - UNDIP 2025

**Final Score:** 🥈 **533** on Kaggle Leaderboard  
**Author:** [Jihan Aqilah](https://github.com/jihan-aqilah)

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![PyTorch](https://img.shields.io/badge/PyTorch-2.3-orange?logo=pytorch)
![Transformers](https://img.shields.io/badge/Transformers-4.44.0-yellow?logo=huggingface)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.5-green?logo=scikitlearn)
![Kaggle Score](https://img.shields.io/badge/Score-533-lightgrey?logo=kaggle)

---

## 📘 Overview

Proyek ini merupakan hasil dari kompetisi **Machine Learning UNDIP 2025**, di mana peserta diminta untuk membangun model prediksi berbasis data nyata.  
Notebook ini berisi seluruh tahapan mulai dari *data cleaning*, *feature engineering*, *modeling*, hingga *submission* yang berhasil meraih **skor 533** di leaderboard Kaggle.

Proyek ini dapat dijadikan referensi untuk:
- Praktik *end-to-end machine learning project*
- Implementasi pipeline *data preprocessing → modeling → evaluation*
- Strategi *model improvement* berdasarkan eksperimen nyata di kompetisi

---

## 📂 Repository Structure

- 📦 lomba-undip-ml
- 📘 full_code_lomba_undip.ipynb (Notebook utama)
- 📄 submit_lomba_undip.csv (File hasil submission ke Kaggle)
- 📄 README.md (Dokumentasi proyek)
- 📄 requirements.txt (Dependency untuk menjalankan notebook)

---

## 🚀 Project Workflow

### 1. **Data Understanding**
Tahapan ini bertujuan memahami struktur data mentah yang diberikan oleh panitia lomba:
- Mengecek jumlah baris & kolom
- Menganalisis tipe data (`int`, `float`, `object`)
- Menghitung *missing values*
- Mengamati distribusi data dan hubungan antar fitur

### 2. **Data Cleaning**
Langkah pembersihan dilakukan untuk memastikan data siap digunakan model:
- Menghapus kolom tidak relevan atau terlalu banyak nilai hilang
- Mengisi nilai kosong menggunakan median/mean/modus
- Menstandarkan format teks (misal kapitalisasi, spasi, simbol)
- Menangani *outlier* bila berpengaruh signifikan

### 3. **Feature Engineering**
Bagian ini sangat penting untuk meningkatkan performa model.  
Beberapa teknik yang digunakan:
- **Encoding fitur kategorikal:** menggunakan `LabelEncoder` atau `OneHotEncoder`
- **Scaling fitur numerik:** dengan `StandardScaler`
- **Feature interaction:** membuat kolom baru seperti rasio, selisih, atau log-transform
- **Feature selection:** memilih fitur paling berpengaruh menggunakan korelasi dan feature importance

### 4. **Model Building**
Eksperimen dilakukan dengan beberapa algoritma populer:
- **RandomForestRegressor**
- **XGBoost**
- **CatBoost**
- (opsional) *Ensemble* dari beberapa model

Proses tuning parameter dilakukan dengan:
- `GridSearchCV` atau `Optuna` untuk mencari kombinasi hyperparameter terbaik
- Evaluasi menggunakan data validasi

### 5. **Model Evaluation**
Evaluasi dilakukan untuk mengukur performa model:
- Menghitung metrik evaluasi (contohnya `RMSE`, `MAE`, `R²`)
- Membandingkan hasil antar model
- Visualisasi hasil prediksi vs nilai aktual
- Analisis error untuk mengidentifikasi pola kesalahan model

### 6. **Submission**
Setelah model terbaik diperoleh:
- Model digunakan untuk memprediksi data uji
- Hasil disimpan dalam format `.csv`
- File `submit_lomba_undip.csv` diunggah ke Kaggle dan memperoleh skor **533**

---

## 📊 Evaluation Matric

Kompetisi ini menggunakan metrik tertentu (misalnya `Root Mean Square Error (RMSE)` atau `Accuracy`) sebagai dasar penilaian di leaderboard.  
Seluruh proses evaluasi juga dijelaskan dalam notebook.

---

## 💡 Key Insights

- Feature engineering sederhana dapat berdampak besar pada hasil akhir.  
- Pemilihan algoritma dan hyperparameter tuning adalah kunci peningkatan performa.  
- Validasi model secara *cross-validation* mencegah overfitting dan menghasilkan model yang lebih stabil.  
- Ensemble dari beberapa model bisa meningkatkan skor di leaderboard.

---

## ⚙️ Requirements

Untuk menjalankan proyek ini, pastikan sudah menginstal dependency berikut:

```bash
pip install -r requirements.txt
