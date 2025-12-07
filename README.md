# Mini Project - Machine Learning  
Klasifikasi Kategori Pencurian Berdasarkan Teks Putusan Pengadilan

![Python](https://img.shields.io/badge/python-3.12%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![License](https://img.shields.io/badge/license-MIT-green)

Proyek ini mengimplementasikan algoritma **machine learning** dan **deep learning** untuk mengklasifikasikan kategori tindak pidana pencurian (**Pencurian Biasa** vs **Pencurian Berat**) berdasarkan analisis teks putusan Pengadilan Negeri Samarinda.

Dengan memanfaatkan Natural Language Processing (NLP) dan transformer, analisis putusan dapat dilakukan secara otomatis dan lebih akurat. Model ini bertujuan:
- Mengklasifikasikan putusan pencurian ke dalam kategori tertentu (misal: pencurian ringan, pencurian dengan pemberatan, dll)
- Mendukung analisis hukum berbasis data (legal analytics)
- Mengurangi beban kerja analis, peneliti hukum, dan lembaga peradilan
- Dataset diperoleh melalui web scraping dari direktori putusan Mahkamah Agung RI.

## Tujuan
Meningkatkan efisiensi analisis hukum dengan otomatisasi klasifikasi putusan pengadilan menggunakan NLP dan machine learning.

## Fitur Utama
- Preprocessing teks bahasa Indonesia (case folding, stopword removal, stemming dengan **Sastrawi**)
- Labeling otomatis berdasarkan kata kunci pasal KUHP
- Ekstraksi fitur: **TF-IDF**, **CountVectorizer** (1-gram & 2-gram), seleksi fitur **Chi-Square**
- Model yang diuji:
  - Naive Bayes
  - Support Vector Machine (SVM)
  - Random Forest
  - Bidirectional LSTM
  - **IndoBERT** (transfer learning – base uncased)
- Evaluasi lengkap: Accuracy, Precision, Recall, F1-Score, Confusion Matrix

## Persyaratan Sistem
- Python 3.20+
- Google Colab atau Jupyter Notebook
- Akses Google Drive

## Dataset
Dataset yang digunakan berupa teks putusan pencurian dari Direktorti Pengadilan Negeri Samarinda yang telah melalui preprocessing.
  
## Contoh Prediksi
Input                                          | Output

"terdakwa terbukti melakukan pencurian ayam"   | pencurian biasa
"terdakwa melakukan pencurian rumah di malam"  | pencurian berat

## Kontributor
- 202210370311304 - Nilla Mery Handayani
- 202210370311311 - Adhim Hendra Maulana
- 202210370311323 - Bastian Feraries WIjaya

## Instalasi
```bash
git clone https://github.com/NilaaMH/Machine-Learning.git
cd NilaaMH
pip install Sastrawi scikit-learn pandas nltk tensorflow transformers torch




