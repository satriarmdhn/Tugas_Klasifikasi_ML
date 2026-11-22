# Tugas Klasifikasi Machine Learning

Tugas kelompok Pengantar Sains Data, Matana University.
Kami memprediksi apakah sebuah kejadian bencana itu **banjir** atau **tanah longsor** berdasarkan dampaknya (korban, rumah rusak, dan lain-lain).

## Anggota Kelompok

- Faridz Henry Saaba (20264920003)
- Ridwan Hamadi Alif (20264920005)
- Satria Ramadhani (20264920010)

## Dataset

Data diambil dari [Indonesia Natural Disaster Dataset (BNPB Records)](https://www.kaggle.com/datasets/maudiana/indonesia-natural-disaster-dataset-bnpb-records) di Kaggle. Data mentahnya ada di folder `data_raw/`.

## Isi Repo

- `notebooks/Klasifikasi_ML.ipynb`: notebook utama, berisi pembersihan data, EDA, Naive Bayes, Logistic Regression, dan validasi.
- `presentasi/Klasifikasi_Banjir_vs_Longsor.pptx`: slide presentasi.
- `data_raw/`: data mentah dari BNPB.
- `data_processed/`: data yang sudah dibersihkan (CSV dan Excel), hasil dari notebook.
- `requirements.txt`: daftar library yang dibutuhkan.

## Cara Menjalankan

1. Pasang library:
   ```bash
   pip install -r requirements.txt
   ```
2. Masuk ke folder `notebooks/` lalu buka `Klasifikasi_ML.ipynb` pakai Jupyter atau Google Colab.
   ```bash
   cd notebooks
   jupyter notebook Klasifikasi_ML.ipynb
   ```
3. Jalankan semua sel dari atas (Run All).

Notebook harus dibuka dari dalam folder `notebooks/`, supaya path ke `data_raw/` dan `data_processed/` terbaca.

## Hasil Singkat

Setelah dibersihkan, data menyisakan 8.438 kejadian. Logistic Regression dengan fitur dampak memberi ROC-AUC sekitar 0,77. Naive Bayes di skenario yang sama tidak lebih baik dari tebakan dummy. Penjelasan lengkapnya ada di notebook dan slide.
