# Project Machine Learning - SDGs 3: Good Health and Well-Being
## Prediksi Risiko Penyakit Jantung menggunakan Algoritma Klasifikasi

Proyek ini dikembangkan untuk memenuhi tugas kelompok Machine Learning dengan berfokus pada penerapan kecerdasan buatan untuk mendukung capaian **Sustainable Development Goals (SDGs) 3: Good Health and Well-Being**.

---

## 👥 Anggota Kelompok (Kelompok 3)

* **Muhammad Hidayat** (NIM: F1G125043)
* **Ni Made Santi Wardani** (NIM: F1G125014)
* **Israwati** (NIM: F1G125009)

**Program Studi:** Ilmu Komputer  
**Fakultas:** Matematika dan Ilmu Pengetahuan Alam  
**Instansi:** Universitas Halu Oleo  

---

## 📌 Latar Belakang & Keterkaitan SDGs

* **Topik SDGs:** Target 3.4 — Mengurangi sepertiga dari kematian dini akibat penyakit tidak menular melalui pencegahan dan pengobatan, serta meningkatkan kesehatan mental dan kesejahteraan.
* **Masalah:** Penyakit jantung merupakan salah satu penyebab utama kematian dini di seluruh dunia. Penanganan dini melalui deteksi risiko berbasis data klinis sangat krusial untuk mencegah komplikasi fatal.
* **Solusi:** Membangun model prediksi risiko penyakit jantung berbasis machine learning untuk membantu penapisan awal risiko kesehatan pasien.

---

## 🎯 Tujuan Proyek

1. Mengembangkan model klasifikasi machine learning untuk memprediksi risiko penyakit jantung pasien berdasarkan fitur-fitur klinis.
2. Membandingkan performa dari 6 algoritma machine learning:
   * **Logistic Regression**
   * **K-Nearest Neighbors (KNN)**
3. Menentukan algoritma terbaik berdasarkan metrik evaluasi (Accuracy, Precision, Recall, dan F1-Score).

---

## 📊 Dataset

* **Nama Dataset:** [Heart Failure Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction) (Kaggle)
* **Deskripsi:** Dataset ini menggabungkan 5 himpunan data penyakit jantung yang berbeda dengan 11 fitur klinis yang digunakan untuk memprediksi kemungkinan pasien mengalami penyakit jantung.

---

## 📈 Hasil Evaluasi Model

Berikut adalah tabel hasil perbandingan performa 6 model Machine Learning yang dievaluasi:

| No | Model | Accuracy | Precision | Recall | F1-Score |
|---|---|---|---|---|---|
| 1 | **K-Nearest Neighbors** | **0.866667** | **0.825000** | **0.916667** | **0.868421** |
| 2 | **Logistic Regression** | 0.853333 | 0.828947 | 0.875000 | 0.851351 |

### 💡 Kesimpulan Performa:
* **K-Nearest Neighbors (KNN)** memperoleh performa terbaik di antara seluruh model dengan **Akurasi 86.67%**, **Recall 91.67%**, dan **F1-Score 86.84%**.
* Model **Logistic Regression** menempati posisi kedua terbaik dengan Akurasi 85.33% dan F1-Score 85.13%.
* High Recall pada K-Nearest Neighbors (KNN) sangat menguntungkan dalam konteks medis (SDGs 3) karena dapat meminimalisir kesalahan deteksi pada pasien yang sebenarnya berisiko tinggi (*False Negative*).

---

## 🛠️ Teknologi & Library yang Digunakan

* **Bahasa Pemrograman:** Python
* **Library Utama:**
  * `Pandas` & `NumPy` — Data Manipulation & Processing
  * `Matplotlib` & `Seaborn` — Data Visualization
  * `Scikit-Learn` — Model Building, Evaluation, & Pipeline

---

## 📁 Struktur Repositori

```text
.
├── datasets/              # Dataset mentah (heart.csv)
├── notebooks/             # Jupyter Notebook (EDA & Pemodelan)
├── models/                # Models tersimpan
├── README.md              # Dokumentasi proyek
└── requirements.txt       # Daftar pustaka / dependensi Python
```

## 🚀 Cara Menjalankan Proyek

### Clone repositori ini:

```bash
git clone https://github.com/Mhmmdhdyt067/deteksi-risiko-serangan-jantung.git
cd deteksi-risiko-serangan-jantung

```

### Buat dan aktifkan Virtual Environment (opsional):


```bash
python -m venv venv
source venv/bin/activate  # Untuk Linux/Mac
# atau
venv\Scripts\activate     # Untuk Windows

```

### Install dependensi:

```bash
pip install -r requirements.txt
```

📝 Lisensi
Proyek ini dibuat untuk tujuan akademis di lingkungan Universitas Halu Oleo.
