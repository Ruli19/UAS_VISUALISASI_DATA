# 📊 UK Co-Benefit Atlas: Eco-Infrastruktur & Resilience

Dashboard interaktif yang menganalisis keterkaitan antara kualitas infrastruktur jalan raya dengan efisiensi energi dan keadilan sosial-ekonomi di Inggris Raya (proyeksi 2025-2050).

**🌐 Live Demo:** [https://ruli19.github.io/UAS_VISUALISASI_DATA/](https://ruli19.github.io/UAS_VISUALISASI_DATA/)

---

## 📂 Informasi Dataset

Proyek ini menggunakan data primer yang bersumber dari platform **UK Co-Benefits Atlas**, sebuah proyek penelitian kolaboratif yang dipimpin oleh *University of Leeds* dan mitra strategis lainnya untuk memetakan dampak kebijakan iklim di Inggris Raya.

### 🔗 Sumber Data

* **Platform Utama:** [UK Co-Benefits Atlas](https://ukcobenefitsatlas.net/)
* **Topik Spesifik:** *Action: Road Repairs* (Dampak perbaikan kualitas permukaan jalan terhadap efisiensi energi)
* **Lisensi:** Data disediakan secara terbuka untuk keperluan riset dan perencanaan kebijakan publik.

### 📝 Penjelasan Dataset

Dataset ini terdiri dari **46.550 baris** yang mencakup data tingkat distrik (*Local Authority District* atau LAD) di seluruh Inggris Raya. Data ini mengintegrasikan indikator teknis mesin kendaraan dengan profil sosial ekonomi penduduk.

| Nama Kolom | Deskripsi Singkat | Jenis Data |
| --- | --- | --- |
| **LAD** | *Local Authority District* (Kode/Nama wilayah administrasi). | String |
| **Rurality** | Klasifikasi wilayah: **1** untuk Pedesaan, **0** untuk Perkotaan. | Binary |
| **Median_Income** | Pendapatan tahunan rata-rata per rumah tangga di wilayah tersebut. | Numeric |
| **Unemployment** | Persentase tingkat pengangguran penduduk usia produktif. | Percentage |
| **Total_vkm** | *Vehicle Kilometres Traveled* (Total jarak tempuh kendaraan per tahun). | Numeric |
| **Y2025_2050** | Estimasi penghematan finansial (GBP) hasil dari pengurangan *rolling resistance*. | Numeric |
| **Number_cars** | Rata-rata jumlah kepemilikan mobil per rumah tangga. | Numeric |

### 🧠 Logika Analisis

Dashboard ini memproses variabel di atas untuk membuktikan hipotesis bahwa **perbaikan jalan adalah aksi keadilan sosial**. Dengan mengurangi hambatan gulir (*rolling resistance*) pada ban kendaraan melalui aspal yang berkualitas, konsumsi bahan bakar dapat ditekan secara signifikan. Hal ini memberikan manfaat ekonomi yang lebih besar bagi warga di wilayah dengan `Unemployment` tinggi yang selama ini terbebani oleh biaya transportasi yang tidak efisien.

---

## 📌 Deskripsi Proyek

Proyek ini menggunakan dataset masif (46.000+ baris) dari **UK Co-Benefits Atlas** untuk memvisualisasikan bagaimana perbaikan jalan raya (*Road Repairs*) bukan sekadar masalah transportasi, melainkan instrumen **Keadilan Iklim (Climate Justice)**. Dashboard ini memetakan dampak teknis terhadap penghematan biaya rumah tangga bagi kelompok masyarakat rentan.

### Pesan Utama (Insight)

Kualitas permukaan jalan yang buruk meningkatkan *rolling resistance*, yang secara langsung membebani ekonomi wilayah dengan tingkat pengangguran tinggi melalui pemborosan BBM. Investasi pada infrastruktur jalan adalah strategi mitigasi biaya hidup jangka panjang.

---

## 🛠️ Fitur Utama & Analisis

* **Analisis Korelasi (Scatter Plot):** Menghubungkan tingkat pengangguran dengan total konsumsi bahan bakar untuk mengidentifikasi area "kemiskinan transportasi".
* **Profil Demografi (Radar Chart):** Perbandingan multidimensi antara wilayah Urban dan Rural berdasarkan 5 variabel (Usia, Pendapatan, Kepemilikan Mobil, dsb).
* **Model Prediktif (Line Chart):** Proyeksi manfaat finansial kumulatif dari penghematan energi hingga tahun 2050.
* **Interaktivitas Real-time:** Filter dinamis berdasarkan Kode Wilayah (LAD), Klasifikasi Area, dan Threshold Pengangguran.

---

## 🧪 Teknologi yang Digunakan

* **Bahasa Utama:** HTML5, CSS3 (Custom Inter UI), JavaScript (ES6+).
* **Library Visualisasi:** [Chart.js](https://www.chartjs.org/) dengan [chartjs-plugin-zoom](https://www.chartjs.org/chartjs-plugin-zoom/) untuk navigasi data granular.
* **Data Processing:** [PapaParse](https://www.papaparse.com/) untuk streaming dataset CSV besar secara asinkron.
* **Ikonografi:** FontAwesome 6.

---

## 📋 Self-Assessment Checklist

| Kategori | Deskripsi Implementasi | Status |
| --- | --- | --- |
| **Clarity** | Hierarki visual yang tegas dengan penggunaan tipografi Inter dan skema warna fungsional. | ✅ |
| **Creativity** | Penggunaan Radar Chart untuk normalisasi data demografi dan fitur zoom pada scatter plot. | ✅ |
| **Accuracy** | Kalkulasi rata-rata (Mean) dan total (Sum) dilakukan secara dinamis tanpa error pembulatan signifikan. | ✅ |

---

**Dibuat oleh:** [Kelompok_2]

**Mata Kuliah:** Visualisasi Data

**Tahun:** 2025

---
