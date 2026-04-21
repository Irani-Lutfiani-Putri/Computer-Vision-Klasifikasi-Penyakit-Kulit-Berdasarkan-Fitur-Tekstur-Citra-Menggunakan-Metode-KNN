# 🧠 Klasifikasi Penyakit Kulit Menggunakan Ekstraksi Fitur Tekstur (GLCM) & KNN
Proyek ini bertujuan untuk mengklasifikasikan jenis penyakit kulit berdasarkan citra menggunakan pendekatan Computer Vision tradisional dan metode K-Nearest Neighbors (KNN). Berbeda dengan deep learning, proyek ini menggunakan ekstraksi fitur manual (GLCM) untuk menangkap karakteristik tekstur citra sebelum dilakukan klasifikasi.

# 📌 Deskripsi Proyek
Model ini digunakan untuk mengklasifikasikan citra penyakit kulit ke dalam dua kategori:
1. Scabies
2. Chickenpox (Varicella)

Berdasarkan hasil pengujian, model KNN mampu mencapai akurasi yang tinggi (± 98%, tergantung data yang digunakan), menunjukkan bahwa fitur tekstur dari citra cukup efektif untuk membedakan kedua jenis penyakit kulit.

# 📊 Ekstraksi Fitur
Data input berupa citra diekstraksi menjadi fitur numerik menggunakan metode GLCM (Gray Level Co-occurrence Matrix), yaitu:

Contrast → perbedaan intensitas piksel

Dissimilarity → ketidaksamaan tekstur

Homogeneity → keseragaman piksel

Energy → kekuatan tekstur

Correlation → hubungan antar piksel

ASM (Angular Second Moment) → ukuran homogenitas

Fitur-fitur ini digunakan sebagai input untuk model KNN.
