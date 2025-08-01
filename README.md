# Analisis Kesehatan Tidur dan Gaya Hidup

![Sleep Analysis Banner](https://img.freepik.com/free-vector/sleep-analysis-concept-illustration_114360-7057.jpg?w=1060&t=st=1722480029~exp=1722480629~hmac=657bf771e3553258849b38030fc865f14ab9d4586414731a50a316b1ed876527)

##  Deskripsi Proyek
Proyek ini bertujuan untuk menganalisis **Sleep Health and Lifestyle Dataset** untuk menemukan pola dan hubungan antara berbagai faktor gaya hidup dengan kualitas tidur. Analisis ini mencakup pembersihan data, eksplorasi data, dan visualisasi interaktif menggunakan Google Looker Studio.

**Tujuan utama dari proyek ini adalah:**
* Mengidentifikasi faktor-faktor utama yang memengaruhi durasi dan kualitas tidur.
* Memahami hubungan antara kondisi kesehatan seperti BMI dan tekanan darah dengan gangguan tidur.
* Menyajikan temuan dalam sebuah dasbor interaktif yang mudah dipahami.

---

## 🔬 Dataset
Dataset yang digunakan dalam proyek ini adalah **Sleep Health and Lifestyle Dataset**.

* **Sumber**: [Darelrk/Sleep-Health-and-Lifestyle-Dataset di GitHub](https://github.com/Darelrk/Sleep-Health-and-Lifestyle-Dataset)
* **Deskripsi**: Dataset ini berisi 374 catatan dari individu dengan berbagai metrik, termasuk Gender, Usia, Pekerjaan, Durasi Tidur, Kualitas Tidur, Level Aktivitas Fisik, Level Stres, Kategori BMI, Tekanan Darah, Detak Jantung, Langkah Harian, dan Gangguan Tidur.

---

## 🧼 Pembersihan dan Persiapan Data
Sebelum analisis, beberapa langkah pembersihan dan persiapan data dilakukan untuk memastikan kualitas dan konsistensi data:

-   **Penanganan Duplikat**: Memeriksa dan menghapus baris data yang terduplikasi.
-   **Standardisasi Kategori**: Menyeragamkan nilai pada kolom `BMI_Category` (mengubah "Normal" menjadi "Normal Weight").
-   **Rekayasa Fitur (Feature Engineering)**: Memisahkan kolom `Blood Pressure` yang berisi teks (misal, "126/83") menjadi dua kolom numerik terpisah: `Systolic` dan `Diastolic`.
-   **(Eksperimental) Data Sintetis**: Membuat dataset tambahan berisi 1000 baris data menggunakan metode **Stratified Resampling** untuk menyeimbangkan distribusi kategori pada `BMI_Category`. Dataset ini dibuat khusus untuk tujuan eksplorasi visual dan tidak digunakan untuk penarikan kesimpulan statistik akhir.

---

## 💡 Temuan Utama (Key Insights)
Analisis dari data ini mengungkapkan beberapa temuan penting:

1.  **Stres adalah Faktor Dominan**: Terdapat korelasi negatif yang kuat antara `Stress_Level` dengan `Quality_of_Sleep` dan `Sleep_Duration`. Semakin tinggi level stres, semakin buruk kualitas dan durasi tidur.
2.  **BMI dan Sleep Apnea**: Kategori BMI **Obese** memiliki hubungan yang sangat signifikan dengan diagnosis **Sleep Apnea**. Sebagian besar responden obesitas dalam dataset ini menderita Sleep Apnea.
3.  **Aktivitas Fisik Meningkatkan Kualitas Tidur**: Individu dengan `Physical_Activity_Level` yang lebih tinggi cenderung melaporkan kualitas tidur yang lebih baik.
4.  **Profil Pekerjaan**: Ditemukan pola menarik pada pekerjaan tertentu. Sebagai contoh, dalam sampel ini, responden dengan pekerjaan "Sales Representative" dan "Scientist" cenderung memiliki berat badan berlebih (Overweight/Obese).
5.  **Distribusi Tekanan Darah**: Sebagian besar responden memiliki status tekanan darah "Normal", namun ditemukan juga penderita "Hipertensi Tkt. 1 & 2" yang seringkali berkorelasi dengan BMI tinggi dan gangguan tidur.

---

## 🛠️ Teknologi yang Digunakan
* **Analisis Data**: Python (dengan library Pandas & NumPy)
* **Lingkungan Kerja**: Google Colaboratory
* **Visualisasi & Dasbor**: Google Looker Studio

---

##  dashboards Pratinjau Dasbor
Dasbor interaktif dirancang untuk menjelajahi temuan-temuan ini secara visual. Dasbor ini mencakup KPI utama, filter interaktif, serta berbagai grafik yang menyoroti hubungan antar variabel.

* **[Lihat Dasbor Interaktif di Sini]([https://lookerstudio.google.com/s/pNtgwV84HTE])**

![Pratinjau Dasbor Analisis Tidur](https://github.com/Darelrk/Sleep-Health-and-Lifestyle-Dataset/raw/main/report.jpg)

---

## ✍️ Penulis
* **Darrell Rafif Kenzie**
* **https://www.linkedin.com/in/darrell-rafif-kenzie-914037288/**
