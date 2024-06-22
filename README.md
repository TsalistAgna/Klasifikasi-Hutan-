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

GLCM (Gray-Level Co-Occurrence Matrix) digunakan dalam proyek ini sebagai metode utama untuk ekstraksi fitur tekstur dari data hutan. GLCM menganalisis tekstur gambar dengan melihat bagaimana pasangan piksel dengan nilai intensitas tertentu muncul pada jarak dan orientasi tertentu. Dalam proyek ini, beberapa fungsi didefinisikan untuk menghitung berbagai fitur tekstur dari GLCM, seperti homogenitas, energi, korelasi, entropi, dan ASM (Angular Second Moment).

Selain itu, terdapat fungsi-fungsi tambahan untuk menghitung rata-rata dan deviasi standar nilai GLCM, yang diperlukan dalam perhitungan beberapa fitur tekstur. Rata-rata untuk baris dan kolom dihitung dengan menjumlahkan produk indeks dan nilai GLCM. Deviasi standar dihitung sebagai akar kuadrat dari jumlah kuadrat perbedaan antara indeks dan nilai rata-rata yang dikalikan dengan nilai GLCM.

## Ekstraksi Fitur

- Kontras: Mengukur perbedaan antara intensitas piksel yang berdekatan, dan nilai kontras yang tinggi menunjukkan adanya perbedaan yang tajam antara piksel-piksel tersebut.
- Korelasi: Mengukur sejauh mana piksel yang berdekatan memiliki hubungan linier. Nilai korelasi yang tinggi menunjukkan adanya pola yang teratur.
- Energi: Mengukur kebesaran energi dalam gambar, dihitung sebagai jumlah kuadrat elemen GLCM. Nilai energi yang tinggi menunjukkan tekstur yang seragam.
- Homogenitas: Mengukur kedekatan distribusi elemen GLCM ke diagonal matriks. Semakin besar homogenitas, semakin halus teksturnya.
- Entropi: Mengukur keacakan dalam gambar. Nilai entropi yang tinggi menunjukkan tekstur yang kompleks dan tidak teratur.
- ASM (Angular Second Moment): Mengukur ketidakteraturan gambar. Nilai ASM yang tinggi menunjukkan tekstur yang lebih homogen.

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

8. Mencari model terbaik:
   Berbagai model klasifikasi (misalnya Random Forest, SVM, atau KNN) diuji untuk menemukan yang terbaik dalam membedakan hutan.

9. Tes hasil pemodelan antara data asli dan prediksi:
   Hasil klasifikasi dibandingkan dengan confusion matrix untuk menilai akurasi model.

## Training Model

Training model dilakukan dengan menggunakan 3 model klasifikasi yaitu K-Nearest Neighbour (KNN), Support Vector Machine (SVM), dan Random Forest (RF). Data yang telah diekstraksi fiturnya dibagi menjadi tiga set, yaitu set pelatihan, set validasi, dan set uji. Pembagian ini penting untuk mengevaluasi performa model secara objektif dan menghindari overfitting. Set pelatihan digunakan untuk melatih model, set validasi untuk menyetel parameter model, dan set uji untuk mengukur kinerja akhir model.

## Confusion Matrix

Confusion matrix bertujuan untuk menyajikan visualisasi mengenai persebaran hasil prediksi yang dihasilkan oleh model. Mulai dari nilai true positive, true negative, false positive, dan false negative.

## Accuracy

## Anggota Tim

- Baiq Annisa Tsalist Agna(F1D022036)
- Dewi Agustin Asri(F1D022039)
- Muhamad Gilang Rahardi Putra(F1D022066)
- Kalsum Rahmawati(F1D022126)
- Regia Puspa Amaranthi(F1D022156)
