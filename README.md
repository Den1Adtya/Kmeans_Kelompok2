# 🏫 K-Means Clustering Fasilitas Sekolah Dasar

## 📌 Deskripsi Proyek

Proyek ini bertujuan untuk mengelompokkan kecamatan berdasarkan kondisi ruang kelas dan fasilitas sekolah dasar menggunakan algoritma **K-Means Clustering**.

Pengelompokan dilakukan berdasarkan beberapa indikator fasilitas sekolah seperti:

* Kelas Baik
* Kelas Rusak Ringan
* Kelas Rusak Sedang
* Perpustakaan
* Tempat Olahraga
* Toilet
* Air Bersih
* Listrik

Hasil clustering diharapkan dapat membantu dalam identifikasi wilayah yang memerlukan prioritas peningkatan fasilitas pendidikan.

---

## 🎯 Tujuan

* Melakukan preprocessing dan pembersihan data fasilitas sekolah dasar.
* Menentukan jumlah cluster optimal menggunakan Elbow Method.
* Mengelompokkan kecamatan menggunakan algoritma K-Means.
* Mengevaluasi kualitas cluster menggunakan Silhouette Score.
* Menampilkan hasil clustering melalui aplikasi Streamlit.

---

## 📊 Dataset

Dataset yang digunakan adalah:

**Jumlah Ruang Kelas Menurut Kondisi dan Fasilitas Sekolah Dasar**

Informasi dataset:

* Jumlah Data : 24 Kecamatan
* Jumlah Fitur Awal : 25 Kolom
* Format : Excel (.xlsx)

---

## 🧹 Data Cleaning

Tahapan preprocessing yang dilakukan:

### Menghapus Kolom Identitas

* No.
* Kecamatan

### Menghapus Kolom Kurang Relevan

* Ruang UKS Baik

* Ruang UKS Rusak

* Jumlah Ruang UKS

* Laboratorium Baik

* Laboratorium Rusak

* Jumlah Laboratorium

### Menghapus Kolom Redundan

* Kelas Rusak Total
* Jumlah Kelas
* Ruang Kelas Seluruh

### Missing Value Handling

Missing value diisi menggunakan median.

### Standardisasi Data

Menggunakan:

```python
StandardScaler()
```

---

## 🤖 Algoritma

Metode clustering yang digunakan:

### K-Means Clustering

Tahapan:

1. Data Cleaning
2. Standardisasi
3. Elbow Method
4. K-Means Clustering
5. Evaluasi Cluster
6. Visualisasi Cluster

---

## 📈 Evaluasi Model

Evaluasi cluster menggunakan:

### Elbow Method

Digunakan untuk menentukan jumlah cluster optimal.

### Silhouette Score

Digunakan untuk mengukur kualitas cluster.

Interpretasi:

* > 0.70 = Sangat Baik
* 0.50 - 0.70 = Baik
* 0.25 - 0.50 = Cukup
* < 0.25 = Kurang Baik

### Davies Bouldin Index

Semakin kecil nilainya semakin baik.

### Calinski Harabasz Index

Semakin besar nilainya semakin baik.

---

## 📍 Visualisasi

Visualisasi yang digunakan:

* Elbow Method
* Silhouette Plot
* Scatter Plot PCA
* Scatter Plot dengan Centroid

---

## 🚀 Deployment

Aplikasi dibangun menggunakan:

* Streamlit
* Pandas
* Scikit-Learn
* Matplotlib
* Seaborn

Fitur aplikasi:

* Upload Dataset
* Data Cleaning
* Elbow Method
* Clustering
* Visualisasi Cluster
* Visualisasi Centroid
* Download Hasil Clustering

---

## 📂 Struktur Project

```text
project-kmeans/

│
├── app.py
├── requirements.txt
├── README.md
├── hasil_clustering.csv
├── jumlah-ruang-kelas-menurut-kondisi-dan-fasilitas-sekolah-dasar-sd.xlsx
└── data_cleaning.ipynb
```

---

## ⚙️ Instalasi

Clone repository:

```bash
git clone https://github.com/username/project-kmeans.git
```

Masuk ke folder project:

```bash
cd project-kmeans
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Menjalankan Aplikasi

```bash
streamlit run app.py
```

---

## 👨‍🎓 Identitas

Nama : Deni Aditya Saputra

Program Studi : Teknik Informatika

Universitas Nusa Putra

---

## 📚 Teknologi yang Digunakan

* Python
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib
* Seaborn
* Yellowbrick
* Streamlit

---

## 📄 Kesimpulan

Hasil clustering menunjukkan bahwa kecamatan dapat dikelompokkan berdasarkan kemiripan kondisi fasilitas sekolah dasar. Kelompok hasil clustering dapat digunakan sebagai dasar dalam menentukan prioritas peningkatan sarana dan prasarana pendidikan.
