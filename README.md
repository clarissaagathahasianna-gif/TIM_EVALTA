# README - CASE 1 BDC MBG Classification

Deskripsi Project

Project ini bertujuan untuk melakukan klasifikasi tweet terkait program Makan Bergizi Gratis (MBG) ke dalam 8 kategori menggunakan metode TF-IDF dan Logistic Regression.

Kategori klasifikasi:

* Anggaran
* Distribusi
* Ekonomi
* Kualitas Pangan
* Politik
* Sasaran Penerima
* Tata Kelola
* Lainnya


# Struktur File

├── CASE 1.ipynb
├── tim_evalta_satriadata.xlsx
└── README.md

---

# Kebutuhan Pustaka (Libraries)

Install library berikut sebelum menjalankan program:

pip install pandas numpy scikit-learn matplotlib seaborn Sastrawi openpyxl

Library yang digunakan:

* pandas
* numpy
* re
* string
* matplotlib
* seaborn
* scikit-learn
* Sastrawi
* openpyxl

---

# Metode yang Digunakan

Model yang digunakan:

* TF-IDF Vectorizer
* Logistic Regression

Tahapan:

1. Data preprocessing
2. TF-IDF vectorization
3. Training Logistic Regression
4. Evaluasi model menggunakan balanced accuracy
5. Prediksi data test
6. Export hasil prediksi ke file excel

---

# Tahapan Preprocessing

Preprocessing yang dilakukan:

* Lowercase
* Menghapus URL
* Menghapus mention
* Menghapus hashtag
* Menghapus angka
* Menghapus tanda baca
* Menghapus karakter non-huruf
* Stopword removal
* Stemming bahasa Indonesia menggunakan Sastrawi

---

# Cara Menjalankan Program

## 1. Mount Google Drive

Pastikan dataset berada di Google Drive.

from google.colab import drive
drive.mount('/content/drive')

---

## 2. Tentukan Path Dataset

train_path = '/content/drive/MyDrive/SATRIA DATA/case_1_labeled_data.xlsx'
test_path = '/content/drive/MyDrive/SATRIA DATA/case_1_text_to_predict.xlsx'
template_path = '/content/drive/MyDrive/SATRIA DATA/case_1_template_sheet.xlsx'

---

## 3. Jalankan Seluruh Cell

Run seluruh cell pada notebook secara berurutan dari atas ke bawah.

---

## 4. Hasil Prediksi

File submission akan otomatis tersimpan di Google Drive dengan nama:

tim_evalta_satriadata.xlsx

---

# Evaluasi Model

Metrik evaluasi yang digunakan:

* Balanced Accuracy
* Classification Report
* Confusion Matrix

Hasil evaluasi model:

Balanced Accuracy: 0.6327

---

# Author

Tim Evalta Satria Data
