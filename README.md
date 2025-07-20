# Analisis Pelanggan Kartu Kredit [Clustering & Klasifikasi]

Proyek ini bertujuan untuk menganalisis dan memahami perilaku pelanggan kartu kredit melalui dua pendekatan utama: **Clustering** untuk segmentasi pelanggan dan **Klasifikasi** untuk memprediksi perilaku pelanggan.

---

## Daftar Isi

1.  [Latar Belakang](#latar-belakang)
2.  [Dataset](#dataset)
3.  [Metodologi](#metodologi)
4.  [Hasil Analisis](#hasil-analisis)
5.  [Tech Stack](#tech-stack)
6.  [Cara Menjalankan Proyek](#cara-menjalankan-proyek)

---

## Latar Belakang

Memahami berbagai segmen pelanggan adalah kunci bagi perusahaan kartu kredit untuk dapat merancang strategi pemasaran yang tepat, meningkatkan retensi, dan mengoptimalkan layanan. Proyek ini menggunakan teknik *machine learning* untuk mengelompokkan pelanggan ke dalam segmen-segmen yang berbeda dan membangun model prediksi berdasarkan karakteristik mereka.

## Dataset

Dataset yang digunakan dalam proyek ini adalah **"Credit Card Customers"** yang bersumber dari Kaggle. Dataset ini berisi berbagai atribut demografis dan finansial dari para pelanggan.

-   **Sumber Dataset**: [Credit Card Customers - Kaggle](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers)

---

## Metodologi

Proyek ini dibagi menjadi dua bagian analisis utama:

1.  **Clustering Pelanggan (Tidak Terbimbing)**
    -   **Algoritma**: K-Means digunakan untuk mengelompokkan pelanggan ke dalam segmen-segmen yang berbeda berdasarkan pola perilaku dan atribut mereka.
    -   **Tujuan**: Mengidentifikasi kelompok pelanggan yang homogen untuk penargetan yang lebih efektif.

2.  **Klasifikasi Pelanggan (Terbimbing)**
    -   **Algoritma**: Random Forest Classifier digunakan untuk memprediksi kategori atau perilaku tertentu dari pelanggan (misalnya, *churn* atau tingkat penggunaan).
    -   **Tuning**: *Hyperparameter tuning* dilakukan untuk mengoptimalkan performa model klasifikasi.

---

## Hasil Analisis

### **1. Hasil Clustering**

-   Dengan menggunakan algoritma K-Means, berhasil diidentifikasi **3 cluster pelanggan** yang berbeda. Setiap cluster memiliki karakteristik unik yang dapat dianalisis lebih lanjut untuk kebutuhan bisnis.

### **2. Hasil Klasifikasi**

-   Model klasifikasi **Random Forest** menunjukkan performa yang sangat baik dalam memprediksi target.
-   Proses *hyperparameter tuning* berhasil meningkatkan akurasi dan F1-score model secara signifikan.

| Metrik | Sebelum Tuning | Setelah Tuning | Peningkatan |
| :--- | :---: | :---: | :---: |
| **Akurasi** | 94.31% | **96.12%** | **+1.81%** |
| **F1-Score** | 94.29% | **96.11%** | **+1.82%** |

---

## Tech Stack

-   **Bahasa Pemrograman**: Python
-   **Library Analisis**: Pandas, NumPy
-   **Library Machine Learning**: Scikit-learn
-   **Library Visualisasi**: Matplotlib, Seaborn

---

## Cara Menjalankan Proyek

1.  **Clone Repositori**
    ```bash
    git clone https://github.com/haaahabib/credit-card.git
    ```
2.  **Masuk ke Direktori Proyek**
    ```bash
    cd credit-card
    ```
3.  **Install Library yang Dibutuhkan**
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn jupyter
    ```
4.  **Jalankan Jupyter Notebook**
    Buka dan jalankan file `.ipynb` yang ada di dalam repositori untuk melihat seluruh proses analisis.
    ```bash
    jupyter notebook
    ```
