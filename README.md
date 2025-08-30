# Diagnosis Sentimen Publik: Mengubah Ulasan Media Sosial menjadi Insight Strategis dengan IBM Granite

**Oleh: Adam Dorman - S1 Sistem Informasi - Universitas Pembangunan Nasional "Veteran" Jakarta**

*Proyek Capstone - IBM SkillsBuild Student Development Initiative*
(Agustus - September 2025)

---

## Latar Belakang dan Masalah yang ada (Project Overview)

Di era digital, media sosial merupakan sebuah dan salah satu sumber data real-time yang krusial untuk memahami opini publik. Namun, volume data yang masif dan tidak terstruktur membuat analisis manual menjadi tidak begitu efisien dan efektif tentunya. Maka dengan itu semua, proyek ini bertujuan dan berusaha untuk mengatasi masalah tersebut dengan mengembangkan solusi analitis berbasis AI dengan sebuah LLM bentukan IBM bernama IBM Granite.

Saya memanfaatkan dan menggunakan sebuah dataset publik dari Kaggle yang berisi ribuan ulasan dari berbagai platform media sosial dalam pengerjaan proyek ini. Proyek ini tidak hanya melakukan tindakan klasifikasi sentimen, melainkan juga berusaha menggali insight yang strategis dari data untuk memberikan pemahaman serta pengetahuan yang lebih mendalam dan praktis tentang perasaan konsumen atau user pada umumnya.


### Tujuan Utama Proyek Saya lakukan ialah sebagai berikut:
1.  **Mengklasifikasikan sentimen ratusan ulasan ( tepatnya dalam proyek ini, sesuai dengan dataset yang dimuat di kaggle ialah sebanyak 732 data mentah ) menjadi ulasan yang Positif, Negatif, atau Netral**.
2.  **Mengidentifikasi isu-isu spesifik yang memicu sentimen negatif, seperti masalah produk, layanan pelanggan, atau harga**.
3.  **Meringkas temuan utama menjadi poin-poin strategis yang ringkas dan dapat ditindaklanjuti**
4.  **Mendemonstrasikan bagaimana model IBM Granite dapat menjadi alat strategis untuk membantu dan memfasilitasi serta menjadi alat pertimbangan pengambilan keputusan berbasis data**.

---

## Proses Analisa dan Peran Strategis AI dalam project saya ini:

Untuk mencapai tujuan di atas, saya menerapkan alur kerja yang sistematis dan berbasis Large Language Model (LLM):

1. **Akuisisi Data: Menggunakan dataset publik dari Kaggle --> Link: (https://www.kaggle.com/code/alkidiarete/social-media-analysis-sentiment/notebook)**.
2. **Pembersihan & Pra-pemrosesan Teks: Melakukan pembersihan data, termasuk penghapusan tautan, mentions, tanda baca, dan standarisasi teks untuk meningkatkan akurasi analisis AI**.
3. **Analisis Sentimen dengan IBM Granite: Menggunakan model ibm-granite/granite-3.3-8b-instruct untuk mengklasifikasikan sentimen setiap ulasan, memberikan hasil yang lebih akurat dibandingkan metode tradisional**.
4. **Klasifikasi Tema Negatif (jika ada): Menganalisis lebih dalam ulasan yang memiliki sentimen negatif untuk mengidentifikasi tema-tema masalah utama, seperti "Layanan Pelanggan" atau "Kualitas Produk"**.
5. **Visualisasi & Interpretasi Hasil: Menggunakan matplotlib dan seaborn untuk memvisualisasikan distribusi sentimen dan tema, yang membantu mengidentifikasi tren utama secara visual**.

## Alur Kerja & Metodologi
1. **Pengumpulan & Konfigurasi Data**
- Sumber Data: Menggunakan dataset ulasan produk nyata yang diunggah dari Kaggle. Total data yang diproses adalah 732 ulasan.
- Konfigurasi AI: Menyiapkan kunci API Replicate yang aman di Google Colab Secrets untuk mengakses model AI IBM Granite secara lancar.
2. **Pra-pemrosesan Data**
- Pembersihan Teks: Menghapus tautan, hashtag, emoji, dan karakter yang tidak relevan untuk memastikan teks siap untuk dianalisis oleh AI.
3. **Analisis Sentimen & Tema**
- Klasifikasi Sentimen: Setiap ulasan dikirimkan ke model IBM Granite untuk diklasifikasikan sebagai 'Positif', 'Negatif', atau 'Netral'.
- Klasifikasi Tema: Ulasan yang berlabel 'Negatif' dianalisis lebih lanjut untuk mengidentifikasi tema masalah utama, seperti 'Layanan Pelanggan', 'Kualitas Produk', atau 'Bug/Error'.
4. **Visualisasi & Analisis Lanjutan**
- Grafik Distribusi: Membuat grafik batang untuk memvisualisasikan proporsi sentimen dan tema masalah.
- Analisis Tren: Menggunakan heatmap untuk melihat bagaimana sentimen negatif berfluktuasi dari waktu ke waktu dan di platform yang berbeda (misalnya, Twitter vs. Instagram).
5. **Sintesis & Rekomendasi Bisnis**
- Ringkasan Otomatis: Menggunakan AI untuk merangkum poin-poin kritis dari ulasan yang paling relevan.
- Rekomendasi Strategis: Menerjemahkan semua temuan (kuantitatif dan kualitatif) menjadi rekomendasi bisnis yang konkret dan terukur, menggunakan kerangka kerja OKR (Objectives and Key Results).

### AI Support Explanation - Penjelasan Bantuan AI LLM IBM Granite dalam proyek ini:
Saya menggunakan IBM Granite dalam proyek ini karena kemampuannya yang unggul dibandingkan metode analisis berbasis leksikon:

-   **Pemahaman Kontekstual yang Mendalam:** Model ini mampu memahami nuansa, sarkasme, dan bahasa informal, menghasilkan klasifikasi sentimen yang jauh lebih akurat.
-   **Kemampuan Multifungsi:** IBM Granite tidak hanya digunakan untuk klasifikasi sentimen, tetapi juga untuk mengidentifikasi tema dari teks dan meringkas ulasan yang panjang menjadi poin-poin strategis.
-   **Konversi Format Data:** Dengan AI IBM Granite ini, saya dapat mengubah teks yang tidak terstruktur menjadi data terukur dan ringkasan strategis yang siap digunakan alias dalam format berbagai macam graf yang memudahkan pembacaan data dan pemahaman client atau yang dalam hal ini orang yang melihat hasil olah data dalam proyek ini.

---

## Temuan Kunci & Insight (Hasil Analisis)

---

## Kesimpulan & Rekomendasi Strategis

### Kesimpulan
Proyek ini berhasil membuktikan bahwa dengan memanfaatkan kekuatan AI canggih seperti IBM Granite, saya dapat mengubah data kualitatif yang masif dan "berisik" menjadi insight strategis yang jernih. Analisis saya menunjukkan bahwa ketidakpuasan karyawan tidak disebabkan oleh satu faktor tunggal, melainkan oleh interaksi kompleks antara kompensasi yang tidak memadai, peluang karir yang terbatas, dan kualitas manajemen yang perlu ditingkatkan.

### Rekomendasi Strategis (Actionable)


---

## Detail Teknikal Proyek
- **Dataset:** [Social Media-Analysis Sentiment](https://www.kaggle.com/code/alkidiarete/social-media-analysis-sentiment/notebook)
- **Data Quantity:** 732 Reviews ( Counted on Raw dataset )
- **AI Model:** ibm-granite/granite-3.3-8b-instruct via Replicate API (`ibm-granite/granite-3.3-8b-instruct`).
- **Tools & Library:** Python, Google Colab, Pandas, Matplotlib, Seaborn, replicate, tqdm.
