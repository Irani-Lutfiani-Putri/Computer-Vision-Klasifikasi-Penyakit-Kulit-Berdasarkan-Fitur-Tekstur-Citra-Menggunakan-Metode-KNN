# 🧠 Klasifikasi Penyakit Kulit Menggunakan Ekstraksi Fitur Tekstur (GLCM) & KNN
Proyek ini bertujuan untuk mengklasifikasikan jenis penyakit kulit berdasarkan citra menggunakan pendekatan Computer Vision tradisional dan metode K-Nearest Neighbors (KNN). Berbeda dengan deep learning, proyek ini menggunakan ekstraksi fitur manual (GLCM) untuk menangkap karakteristik tekstur citra sebelum dilakukan klasifikasi.

# 📌 Deskripsi Proyek
Model ini digunakan untuk mengklasifikasikan citra penyakit kulit ke dalam dua kategori:
1. Scabies
2. Chickenpox (Varicella)

Berdasarkan hasil pengujian, model KNN mampu mencapai akurasi yang tinggi (± 98%, tergantung data yang digunakan), menunjukkan bahwa fitur tekstur dari citra cukup efektif untuk membedakan kedua jenis penyakit kulit.

# 📊 Ekstraksi Fitur
Data input berupa citra diekstraksi menjadi fitur numerik menggunakan metode GLCM (Gray Level Co-occurrence Matrix), yaitu:

- Contrast → perbedaan intensitas piksel
- Dissimilarity → ketidaksamaan tekstur
- Homogeneity → keseragaman piksel
- Energy → kekuatan tekstur
- Correlation → hubungan antar piksel
- ASM (Angular Second Moment) → ukuran homogenitas

Fitur-fitur ini digunakan sebagai input untuk model KNN.

# 📂 Dataset
Dataset yang digunakan adalah dataset citra penyakit kulit dari Kaggle:
- Kaggle Dataset : https://www.kaggle.com/datasets/devdope/skin-disease-raw-dataset

Dataset terdiri dari beberapa kelas penyakit, namun pada proyek ini hanya digunakan 2 kelas:
- sc_Scabies_sarna
- ch_Chickenpox_Varicela

# 🛠️ Teknologi yang Digunakan
- Bahasa: Python
- Environment: Google Colab

Library Utama:
- OpenCV (cv2) → pemrosesan citra
- Scikit-image → ekstraksi fitur GLCM
- Scikit-learn → model KNN dan evaluasi
- Pandas & NumPy → pengolahan data
- Matplotlib & Seaborn → visualisasi

# 🧠 Metode yang Digunakan
🔍 K-Nearest Neighbors (KNN)
- Mengklasifikasikan data berdasarkan kedekatan jarak antar fitur
- Parameter utama : K (jumlah tetangga) → ditentukan melalui proses tuning (1–10)

# 🚀 Cara Penggunaan
1. Download dataset dari Kaggle
2. Upload dataset ke Google Drive
3. Buka Google Colab
4. Sesuaikan path dataset pada kode
5. Jalankan seluruh script untuk:
   - Ekstraksi fitur
   - Training model
   - Evaluasi hasil

# 📈 Hasil Evaluasi
Model dievaluasi menggunakan:
- Accuracy Score
- Confusion Matrix
- Classification Report

Hasil menunjukkan bahwa model KNN mampu mengklasifikasikan citra dengan performa yang sangat baik, terutama dalam membedakan pola tekstur antar penyakit kulit.
