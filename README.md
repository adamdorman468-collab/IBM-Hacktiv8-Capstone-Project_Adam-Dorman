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
Temuan Kunci & Insight
Distribusi Sentimen
Grafik menunjukkan bahwa sentimen ulasan secara keseluruhan sangat positif, dengan lebih dari 500 ulasan masuk dalam kategori ini. Namun, ada sekitar 180 ulasan negatif yang mengindikasikan adanya isu spesifik yang perlu ditangani. Ulasan netral jumlahnya sangat sedikit, menunjukkan bahwa sebagian besar pengguna memiliki pandangan yang kuat terhadap produk, baik positif maupun negatif.

Analisis Ulasan Negatif
Analisis lebih dalam terhadap ulasan negatif menggunakan IBM Granite mengungkapkan bahwa keluhan tidak hanya terfokus pada masalah fungsional. Meskipun tema utama yang teridentifikasi adalah "Fitur," ringkasan eksekutif menunjukkan bahwa masalah yang paling sering muncul berkaitan dengan aspek emosional dan pengalaman pengguna:

- Kebingungan: Pengguna merasa kesulitan dalam mengambil keputusan atau menavigasi.

- Stagnasi: Adanya perasaan tidak ada kemajuan atau proyek pribadi terhenti.

- Bosan & Monoton: Pengguna merasa terjebak dalam rutinitas dan merasa bosan.

- Kesepian: Adanya kerinduan akan koneksi dan interaksi sosial.

Insight: Temuan ini menunjukkan bahwa masalah utama bukanlah produk itu sendiri, melainkan bagaimana pengguna berinteraksi dan merasakan produk tersebut. Isu-isu emosional ini memiliki dampak signifikan pada pengalaman pengguna, yang pada akhirnya memicu ulasan negatif.

## Temuan Kunci dan Wawasan dari Analisis Media Sosial
Analisis sentimen pada data media sosial dari tahun 2010 hingga 2023 mengungkapkan beberapa tren dan pola penting di berbagai platform (Twitter, Instagram, Facebook).

1. Tren Kenaikan Ulasan dan Sentimen Negatif
- Dari tahun 2010 hingga 2014, volume ulasan sangat rendah. Namun, mulai tahun 2015, terjadi lonjakan signifikan pada jumlah total ulasan. Peningkatan ini menunjukkan aktivitas pengguna yang terus meningkat di media sosial. Meskipun sentimen positif selalu mendominasi dalam hal jumlah total ulasan, proporsi sentimen negatif juga mulai muncul dan meningkat, mencapai puncaknya di tahun 2023.

2. Perbedaan Perilaku Sentimen Antar Platform
Analisis menunjukkan bahwa tidak semua platform berperilaku sama.
- Twitter adalah platform yang paling sering memiliki proporsi sentimen negatif yang sangat tinggi, terutama pada tahun 2016 dan 2018. Hal ini mengindikasikan bahwa Twitter cenderung menjadi tempat bagi pengguna untuk menyuarakan ketidakpuasan atau kritik yang lebih intens.
- Instagram dan Facebook memiliki sentimen negatif yang lebih rendah dan lebih stabil secara proporsional. Namun, dalam hal jumlah total ulasan, Instagram memiliki jumlah ulasan negatif terbanyak (sekitar 65 ulasan). Ini menunjukkan bahwa meskipun proporsinya tidak setinggi Twitter, volume keluhan di Instagram tetap signifikan.

3. Dominasi Sentimen Positif
- Terlepas dari adanya sentimen negatif, sentimen positif tetap menjadi mayoritas mutlak di semua platform dan setiap tahunnya. Jumlah ulasan positif terus meningkat, mencapai puncaknya di tahun 2023. Ini menunjukkan bahwa meskipun ada masalah, produk atau topik yang dianalisis secara umum diterima dengan sangat baik oleh pengguna.

Secara keseluruhan, temuan ini menyimpulkan bahwa data media sosial adalah sumber yang kaya untuk memahami sentimen pengguna. Meskipun sentimen positif mendominasi, analisis mendalam pada sentimen negatif dapat mengungkap isu-isu spesifik yang memerlukan perhatian, terutama di platform seperti Twitter dan Instagram.

## Implikasi Strategis
Analisis sentimen ini menunjukkan bahwa meskipun produk secara umum diterima dengan baik, ada celah emosional yang signifikan yang perlu diperbaiki. Ini bukan sekadar masalah teknis yang bisa diselesaikan dengan bug fix, melainkan memerlukan pendekatan yang lebih holistik. Untuk produk ini, kepuasan pengguna tidak hanya bergantung pada fungsionalitas, tetapi juga pada bagaimana produk tersebut membuat mereka merasa.

## Keterkaitan Antar Temuan
- Hubungan antara "Fitur" dan "Kebingungan": Tema "Fitur" yang diidentifikasi oleh model AI kemungkinan besar terkait dengan rasa "kebingungan" yang dirasakan pengguna. Ini berarti ada fitur yang mungkin terlalu rumit atau tidak memiliki panduan yang jelas, sehingga membuat pengguna merasa kesulitan.

- Hubungan antara "Stagnasi" dan "Bosan": Perasaan mandek dan bosan saling berkaitan. Ketika pengguna merasa tidak ada kemajuan, mereka cenderung kehilangan motivasi dan akhirnya merasa bosan. Ini mengindikasikan bahwa produk tidak memberikan stimulus atau tantangan yang cukup untuk mempertahankan keterlibatan jangka panjang.

- Hubungan antara "Loneliness" dan "Kurangnya Koneksi": Ulasan ini menyarankan bahwa ada kebutuhan akan aspek sosial dalam produk yang saat ini tidak terpenuhi. Pengguna mungkin mencari platform untuk terhubung atau berinteraksi dengan orang lain yang memiliki tujuan atau minat yang sama.

---

## Kesimpulan & Rekomendasi

### Kesimpulan
Analisis sentimen pada media sosial mengungkapkan tren yang kompleks. Meskipun sentimen positif secara konsisten mendominasi di semua platform dari tahun 2010 hingga 2023, sentimen negatif juga mengalami peningkatan. Peningkatan ini paling signifikan di platform Twitter, yang menunjukkan proporsi sentimen negatif tertinggi, menandakan bahwa platform ini sering digunakan sebagai tempat untuk menyuarakan keluhan. Instagram dan Facebook memiliki tren yang lebih stabil, namun Instagram menonjol dengan jumlah total ulasan negatif terbanyak. Ini menunjukkan bahwa meskipun produk atau topik yang dianalisis secara umum diterima dengan baik, ada isu-isu spesifik yang memerlukan perhatian, terutama di Twitter dan Instagram.

(Ringkasan Eksekutif):
Analisis sentimen pada media sosial menunjukkan bahwa produk ini memiliki penerimaan yang sangat positif secara keseluruhan. Namun, terdapat sentimen negatif yang meningkat di platform tertentu, terutama Twitter. Analisis mendalam mengungkapkan bahwa keluhan ini tidak hanya berfokus pada masalah fungsional, tetapi juga pada isu-isu emosional seperti perasaan bosan, kebingungan, stagnasi, dan kesepian. Ini menandakan perlunya pendekatan strategis yang lebih holistik.
### Rekomendasi
Tingkatkan Pengalaman Pengguna (UX)

- Atasi Kebingungan: Sederhanakan alur pengguna dan perbaiki proses onboarding agar lebih intuitif. Tambahkan tooltip atau tutorial singkat di dalam aplikasi untuk memandu pengguna, sehingga mereka tidak merasa tersesat.
- Lawan Stagnasi dan Kebosanan: Terapkan elemen gamifikasi seperti progress bar atau lencana untuk membuat pengalaman lebih menarik. Perbarui konten atau tantangan secara berkala agar pengguna tidak merasa bosan.

Perkuat Keterlibatan Komunitas
- Bangun Koneksi: Ciptakan ruang bagi pengguna untuk terhubung, seperti forum atau grup media sosial. Langkah ini membantu membangun rasa komunitas dan mengatasi perasaan "kesepian."
- Angkat Kisah Pengguna: Tampilkan kisah sukses pengguna untuk memotivasi orang lain. Cerita-cerita ini dapat secara langsung mengatasi perasaan stagnasi dan menunjukkan potensi produk.

Sempurnakan Strategi Komunikasi
- Tunjukkan Empati: Buat konten yang tidak hanya menjual fitur, tetapi juga menunjukkan empati terhadap masalah emosional pengguna. Akui frustrasi mereka dan posisikan produk sebagai solusi yang peduli.
- Dengarkan dan Tanggapi: Sediakan saluran umpan balik yang jelas. Aktif pantau media sosial dan tanggapi setiap komentar untuk menunjukkan bahwa suara pengguna didengar. Hal ini dapat mengubah pengalaman negatif menjadi positif.
---

## Detail Teknikal Proyek
- **Dataset:** [Social Media-Analysis Sentiment](https://www.kaggle.com/code/alkidiarete/social-media-analysis-sentiment/notebook)
- **Data Quantity:** 732 Reviews ( Counted on Raw dataset )
- **AI Model:** ibm-granite/granite-3.3-8b-instruct via Replicate API (`ibm-granite/granite-3.3-8b-instruct`).
- **Tools & Library:** Python, Google Colab, Pandas, Matplotlib, Seaborn, replicate, tqdm.
