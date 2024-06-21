# Klasifikasi Hutan sebagai Langkah Restorasi Dini di Tengah Pertumbuhan Kawasan Industri

Proyek ini bertujuan untuk mengklasifikasikan hutan berdasarkan 3 label yaitu hutan lebat, sebagian lebat, dan gundul. Hal ini bertujuan untuk pengambilan langkah restorasi dini pada hutan ditengah banyaknya hutan yang beralih fungsi menjadi kawasan industri. Langkah restorasi dini bisa menjadi langkah yang tepat untuk melestarikan keberadaan hutan untuk masa depan lingkungan yang lebih baik.

## Daftar Isi

- [Tentang Proyek](#tentang-proyek)
- [GLCM](#GLCM)
- [Ekstraksi Fitur](#Ekstraksi-fitur)
- [Tahap Preprocessing](#preprocessing)
- [Training Model](#model)
- [Confusion Matrix](#matrix)
- [Accuracy](#accuracy)
- [Anggota tim](#tim)

## Tentang Proyek

Berikan deskripsi yang lebih mendetail

## GLCM

## Ekstraksi Fitur
- fitur 1
- fitur 2
- fitur n

## Tahap Preprocessing
1. Menghitung GLCM dari tiap citra:
GLCM dihitung dari citra satelit atau udara dari area hutan dan kawasan industri. Ini akan membantu mengidentifikasi pola tekstur yang berbeda antara hutan lebat, hutan setengah lebat, dan hutan gundul.

2. Analisa Fitur pada GLCM tiap citra:
Fitur seperti kontras, korelasi, energi, dan homogenitas dianalisis untuk membedakan karakteristik hutan.

3. Akurasi Tes citra original:
Model diuji menggunakan citra asli untuk melihat seberapa baik ia dapat membedakan area hutan tanpa preprocessing.

4. Melakukan Preprocessing:
Tahap preprocessing dilakukan dengan melakukan segmentasi warna, image enhancement, normalisasi, opening, dan deteksi tepi.

5. Menghitung GLCM citra yang telah di preprocessing:
GLCM dihitung kembali dari citra yang telah dipreprocessing untuk mendapatkan representasi tekstur yang lebih akurat.

6. Menganalisa fitur terhadap GLCM:
Analisis fitur diulang pada citra yang telah dipreprocessing untuk melihat apakah ada peningkatan dalam kemampuan membedakan hutan.

7. Akurasi Tes citra preprocessing:
Model diuji kembali menggunakan citra yang telah dipreprocessing untuk melihat apakah ada peningkatan akurasi dalam klasifikasi hutan.

9. Mencari model terbaik:
Berbagai model klasifikasi (misalnya Random Forest, SVM, atau KNN) diuji untuk menemukan yang terbaik dalam membedakan hutan.

10. Tes hasil pemodelan antara data asli dan prediksi:
Hasil klasifikasi dibandingkan dengan confusion matrix untuk menilai akurasi model.

## Training Model
Training model dilakukan dengan menggunakn 3 model klasifikasi yaitu K-Nearest Neighbour (KNN), Support Vector Machine (SVM), dan Random Forest (RF).

## Confusion Matrix
Confusion matrix bertujuan untuk menyajikan visualisasi mengenai persebaran hasil prediksi yang dihasilkan oleh model. Mulai dari nilai true positive, true negative, false positive, dan false negative.

## Accuracy

## Anggota Tim
- Baiq Annisa Tsalist Agna(F1D022036)
- Dewi Agustin Asri(F1D022039)
- Muhamad Gilang Rahardi Putra(F1D022066)
- Kalsum Rahmawati(F1D022126)
- Regia Puspa Amaranthi(F1D022156)
