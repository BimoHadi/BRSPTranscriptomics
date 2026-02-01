# Repository BRSP Transcriptomics 🧬

Selamat datang di repository BRSP Transcriptomics! Repository ini berisi modul praktikum dan skrip R untuk analisis data ekspresi gen (Transcriptomics) menggunakan data publik dari NCBI GEO.

Modul ini dirancang khusus untuk memahami alur kerja bioinformatika mulai dari pengambilan data mentah hingga visualisasi hasil.

## 📂 Modul 1: Respon Vaksin Influenza (GSE48018)

**Tujuan:** Mengidentifikasi gen yang mengalami perubahan ekspresi signifikan (*Differentially Expressed Genes* / DEG) antara individu yang divaksinasi dibandingkan dengan kontrol (baseline).

**Poin Pembelajaran:**
* **Pengambilan Data:** Mengunduh dataset `GSE48018` secara otomatis menggunakan `GEOquery`.
* **Platform:** Microarray Illumina HumanHT-12 V4.0.
* **Preprocessing:** Kontrol kualitas data, transformasi log2, dan inspeksi normalisasi.
* **Analisis Statistik:** Menggunakan package `limma` untuk pemodelan linear.
* **Visualisasi:**
    * **Volcano Plot:** Melihat signifikansi statistik vs *fold change*.
    * **Heatmap:** Pola klastering 50 gen teratas.
    * **UMAP:** Reduksi dimensi untuk melihat sebaran sampel.

## 📂 Modul 2: Analisis Kanker Paru (GSE10072)

**Tujuan:** Menganalisis perbedaan ekspresi gen antara jaringan Adenokarsinoma Paru (*Lung Adenocarcinoma*) dan jaringan paru normal untuk mencari kandidat biomarker.

**Poin Pembelajaran:**
* **Platform:** Microarray Affymetrix HG-U133A (GPL96).
* **Anotasi Gen:** Mapping dari ID Probe Affymetrix ke nama gen (Gene Symbol) menggunakan database `hgu133a.db`.
* **Statistik:** Penerapan koreksi *False Discovery Rate* (FDR) dengan p-value < 0.01.
* **Studi Kasus Medis:** Memahami aplikasi transcriptomics dalam riset penyakit/kanker.

