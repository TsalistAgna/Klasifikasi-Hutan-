# Klasifikasi Hutan sebagai Langkah Restorasi Dini di Tengah Pertumbuhan Kawasan Industri

Deskripsi singkat tentang apa proyek ini dan tujuan utamanya.

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
1.Menghitung GLCM dari tiap citra:
GLCM dihitung dari citra satelit atau udara dari area hutan dan kawasan industri. Ini akan membantu mengidentifikasi pola tekstur yang berbeda antara hutan sehat, hutan terdegradasi, dan area industri.
2.Analisa Fitur pada GLCM tiap citra:
Fitur seperti kontras, korelasi, energi, dan homogenitas dianalisis untuk membedakan karakteristik hutan dari area industri. Misalnya, hutan cenderung memiliki tekstur yang lebih heterogen dibanding area industri.
3.Akurasi Tes citra original:
Model diuji menggunakan citra asli untuk melihat seberapa baik ia dapat membedakan area hutan dari kawasan industri tanpa preprocessing.
4.Melakukan Preprocessing:
Citra satelit atau udara mungkin memerlukan koreksi atmosferik, normalisasi, atau peningkatan kontras untuk membedakan vegetasi dengan lebih baik.
5.Menghitung GLCM citra yang telah di preprocessing:
GLCM dihitung kembali dari citra yang telah dipreprocessing untuk mendapatkan representasi tekstur yang lebih akurat.
6.Menganalisa fitur terhadap GLCM:
Analisis fitur diulang pada citra yang telah dipreprocessing untuk melihat apakah ada peningkatan dalam kemampuan membedakan hutan dari area industri.
Akurasi Tes citra preprocessing:
Model diuji kembali menggunakan citra yang telah dipreprocessing untuk melihat apakah ada peningkatan akurasi dalam klasifikasi hutan dan area industri.
7.Mencari model terbaik:
Berbagai model klasifikasi (misalnya Random Forest, SVM, atau Deep Learning) diuji untuk menemukan yang terbaik dalam membedakan hutan dari area industri.
8.Tes hasil pemodelan antara data asli dan prediksi:
Hasil klasifikasi dibandingkan dengan peta penggunaan lahan yang telah diverifikasi di lapangan untuk menilai akurasi model.
## Training Model

## Confusion Matrix

## Accuracy

## Anggota Tim
Baiq Annisa Tsalist Agna(F1D022036)
Dewi Agustin Asri(F1D022039)
Muhamad Gilang Rahardi Putra(F1D022066)
Kalsum Rahmawati(F1D022126)
Regia Puspa Amaranthi(F1D022156)