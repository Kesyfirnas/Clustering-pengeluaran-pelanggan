# Clustering-pengeluaran-pelanggan

## 📂 Dataset
Dataset yang digunakan dalam proyek ini berasal dari Kaggle.
🔗 **Sumber Data:** [Customer Personality Analysis Dataset](https://www.kaggle.com/imakash3011/customer-personality-analysis)


## 📌 Latar Belakang & Masalah
Sebuah perusahaan mengalami kesulitan dalam menargetkan promosi pemasaran. Selama ini, mereka mengirimkan tawaran yang sama ke semua pelanggan ("Satu Promosi untuk Semua"), yang mengakibatkan biaya pemasaran tinggi namun konversi penjualan rendah.

**Tujuan Proyek:**
Melakukan segmentasi pelanggan (*Customer Segmentation*) menggunakan algoritma *Machine Learning* (Unsupervised Learning) untuk mengidentifikasi kelompok pelanggan yang berbeda berdasarkan perilaku belanja dan demografi mereka.

## 🛠️ Tools & Metodologi
Proyek ini dikerjakan menggunakan **Python** di lingkungan Jupyter Notebook (Kaggle).

* **Data Cleaning:** Menangani *missing values*, menghapus outlier pendapatan (>200k), dan *feature engineering* (membuat kolom `Total_Spend` dan `Age`).
* **Dimensionality Reduction:** Menggunakan Standard Scaler untuk menyamakan skala data.
* **Modeling:** Algoritma **K-Means Clustering**.
* **Evaluasi:** Elbow Method & Silhouette Analysis.

## 📊 Hasil Analisis (Key Insights)
Berdasarkan analisis data, ditemukan **3 Cluster Pelanggan** dengan karakteristik unik:

### 1. Segmen "Hemat" (Budget Customer)
* **Karakter:** Pendapatan rendah, pengeluaran sangat minim.
* **Perilaku Unik:** Sangat sering mengunjungi Website (*Web Visits* tinggi), tetapi jarang membeli. Mengindikasikan perilaku *Window Shopping*.
* **Rekomendasi:** Gunakan strategi diskon agresif atau kupon "Pengguna Baru" untuk memicu pembelian.

### 2. Segmen "Menengah" (Aspiring Customer)
* **Karakter:** Pendapatan menengah, pengeluaran cukup stabil.
* **Perilaku Unik:** Membeli kebutuhan standar. Potensi daya beli masih bisa ditingkatkan.
* **Rekomendasi:** Tawarkan paket *Bundling* (Beli 2 Gratis 1) untuk meningkatkan nilai keranjang belanja.

### 3. Segmen "Sultan" (Premium Customer)
* **Karakter:** Pendapatan tinggi, mendominasi pembelian **Anggur (Wines)** dan **Daging (Meat)**.
* **Perilaku Unik:** Lebih suka berbelanja via **Katalog** dan **Toko Fisik**. Kurang responsif terhadap kunjungan website.
* **Rekomendasi:** Tawarkan layanan VIP eksklusif, produk *Limited Edition*, dan hindari diskon murahan demi menjaga gengsi.

---

## 📈 Evaluasi Model
Untuk memastikan kualitas pengelompokan, model dievaluasi menggunakan metrik statistik:

1.  **Elbow Method:** Menunjukkan penurunan inersia yang tajam (siku) pada **k=3**, menandakan jumlah cluster yang optimal.
2.  **Silhouette Score:** Mencapai skor **0.347**, yang mengindikasikan bahwa pemisahan antar kelompok sudah terbentuk dengan cukup jelas dan valid secara statistik.

---

## 📸 Visualisasi Data

> **Peta Persebaran Pelanggan (Income vs Total Spend):**
<img width="862" height="550" alt="image" src="https://github.com/user-attachments/assets/4cda17b3-79bd-49e6-809f-d19a85fabb57" />

> **BOXPLOT Data Distribusi:**
<img width="1271" height="795" alt="image" src="https://github.com/user-attachments/assets/827812c8-4135-4dd6-81ff-2f680ba4aad2" />

> **Boxplot total belanja per cluster:**
<img width="864" height="552" alt="image" src="https://github.com/user-attachments/assets/5388c9ef-9754-4bd8-a01b-7369d536960e" />


> *Terlihat jelas tiga kelompok terpisah berdasarkan kemampuan ekonomi.*
<img width="704" height="464" alt="image" src="https://github.com/user-attachments/assets/5d2c2a1c-5ac9-4e32-ae85-c9a43bc9b07c" />

---

## 📂 Struktur File
* `Customer_Segmentation.ipynb`: Notebook utama berisi seluruh kode analisis.
* `marketing_campaign.csv`: Dataset mentah (sumber: Kaggle).
* `README.md`: Dokumentasi proyek.

## 🤝 Kontak
Dibuat oleh **[Nama Kamu]**.
Jika ada pertanyaan atau diskusi mengenai proyek ini, silakan hubungi via [LinkedIn/Email Kamu].
