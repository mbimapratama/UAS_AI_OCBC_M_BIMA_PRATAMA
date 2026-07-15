# Analisis Sentimen Review Pengguna Aplikasi OCBC Mobile Indonesia Menggunakan Support Vector Machine (SVM)

## Deskripsi Project

Project ini merupakan tugas Ujian Akhir Semester (UAS) Mata Kuliah Artificial Intelligence di Jakarta Global University.

Penelitian ini bertujuan untuk menganalisis sentimen pengguna aplikasi **OCBC Mobile Indonesia** berdasarkan ulasan (review) yang diambil dari Google Play Store. Data review diperoleh menggunakan teknik **Web Scraping**, kemudian dilakukan proses **preprocessing**, **ekstraksi fitur menggunakan TF-IDF**, serta klasifikasi sentimen menggunakan algoritma **Support Vector Machine (SVM)**.

Sentimen diklasifikasikan menjadi tiga kategori, yaitu:

- Positif
- Netral
- Negatif

---

## Tujuan Penelitian

- Mengambil data review aplikasi OCBC Mobile Indonesia dari Google Play Store.
- Melakukan preprocessing terhadap data teks.
- Mengubah data teks menjadi fitur numerik menggunakan TF-IDF.
- Melatih model klasifikasi menggunakan Support Vector Machine (SVM).
- Menguji performa model menggunakan Accuracy, Precision, Recall, dan F1-Score.

---

## Dataset

Sumber data:

Google Play Store

Aplikasi:

**OCBC Mobile Indonesia**

Package Name

```
com.ocbcnisp.onemobileapp
```

Data diperoleh menggunakan library:

```
google-play-scraper
```

---

## Tools

- Python
- Google Colab
- Jupyter Notebook
- GitHub

---

## Library

- pandas
- numpy
- matplotlib
- seaborn
- nltk
- Sastrawi
- scikit-learn
- wordcloud
- google-play-scraper
- joblib

---

## Struktur Folder

```
UAS_AI_OCBC/

│
├── Scraping_Data_Sentimen_Analisis.ipynb
├── Pemodelan_Sentimen_Analisis_Project.ipynb
├── Testing_Sentimen_Analisis_Project.ipynb
│
├── hasil_scraping_OCBC.csv
├── dataset_preprocessing_OCBC.csv
│
├── svm_model.pkl
├── tfidf_vectorizer.pkl
│
├── requirements.txt
├── README.md
└── Poster_UAS.pdf
```

---

## Tahapan Penelitian

### 1. Web Scraping

Mengambil data review pengguna aplikasi OCBC Mobile Indonesia dari Google Play Store menggunakan library `google-play-scraper`.

---

### 2. Data Cleaning

Melakukan pembersihan data meliputi:

- Menghapus data kosong
- Menghapus data duplikat
- Menghapus URL
- Menghapus angka
- Menghapus tanda baca
- Mengubah huruf menjadi lowercase

---

### 3. Text Preprocessing

Tahapan preprocessing terdiri dari:

- Case Folding
- Tokenizing
- Stopword Removal
- Stemming menggunakan Sastrawi

---

### 4. Label Sentimen

Label sentimen ditentukan berdasarkan rating pengguna.

| Rating | Sentimen |
|---------|-----------|
| 4-5 | Positif |
| 3 | Netral |
| 1-2 | Negatif |

---

### 5. Feature Extraction

Ekstraksi fitur dilakukan menggunakan metode:

**TF-IDF (Term Frequency-Inverse Document Frequency)**

---

### 6. Training Model

Model klasifikasi menggunakan algoritma:

**Support Vector Machine (SVM)**

---

### 7. Evaluasi Model

Model dievaluasi menggunakan:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

---

### 8. Testing Model

Model diuji menggunakan kalimat baru untuk mengetahui hasil prediksi sentimen.

Contoh:

Input:

```
Aplikasi sangat membantu transaksi saya.
```

Output:

```
Positif
```

---

## Cara Menjalankan Project

### 1. Clone Repository

```bash
git clone https://github.com/username/UAS_AI_OCBC.git
```

---

### 2. Install Library

```bash
pip install -r requirements.txt
```

---

### 3. Jalankan Notebook Secara Berurutan

1. Scraping_Data_Sentimen_Analisis.ipynb

2. Pemodelan_Sentimen_Analisis_Project.ipynb

3. Testing_Sentimen_Analisis_Project.ipynb

---

## Hasil Project

Output yang dihasilkan antara lain:

- Dataset hasil scraping (.csv)
- Dataset preprocessing (.csv)
- Visualisasi distribusi sentimen
- WordCloud Positif
- WordCloud Negatif
- Confusion Matrix
- Model SVM (.pkl)
- TF-IDF Vectorizer (.pkl)

---

## Penulis

**Muhammad Bima Pratama**

Program Studi Teknik Informatika

Jakarta Global University

---

## Mata Kuliah

Artificial Intelligence

Dosen:

**Anindya Ananda Hapsari, S.ST., MIT**

---

## Lisensi

Project ini dibuat untuk memenuhi tugas Ujian Akhir Semester (UAS) Mata Kuliah Artificial Intelligence di Jakarta Global University.
