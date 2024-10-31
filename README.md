<h1 align="center"> Natural Language Processing with Hugging Face Transformers </h1>
<p align="center"> Hai, sahabat pembaca! Selamat datang di petualangan seru kita menjelajahi dunia Natural Language Processing (NLP). Siapkan diri Anda untuk menemukan berbagai model yang siap membantu Anda, mulai dari mengklasifikasikan teks hingga menerjemahkan kalimat dengan gaya yang penuh semangat! </p>

<div align="center">

<img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54">
<img src="https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white">

<h1 align="center"> Analisis </h1>
<p>Mari kita lihat apa saja yang bisa dilakukan oleh teman-teman kita yang berbasis AI ini:</p>

### 1. Zero-Shot Classification
Zero-Shot Classification ini berfungsi untuk mengklasifikasikan teks yang tidak memerlukan pelatihan pelatihan untuk setiap kategori. Model dapat mengklasifikasikan teks tersebut hanya dengan berdasarkan deskripsi label yang kita berikan. Hasil nya akan memberikan kategori yang sesuai serta menunjukkan berapa skor probabilitas dari setiap label yang ada dari klasifikasi teks yang kita berikan.

### 2. Text Generation
text - generation ini berfungsi sebagai mana untuk menghasilkan teks secara otomatis, berdasarkan teks atau kalimat awal yang telah kita inputkan. Yang mana hasil pipeline ini menciptakan kalimat atau paragraf sesuai dengan input yang diberikan. Ini berguna untuk : 

- Membantu penulis dalam mendapatkan ide.
- Menciptakan respons dalam chatbot.
- Menghasilkan dialog atau narasi.

### 3. Text Generation dengan Model DistilGPT2

Sama seperti poin no2 akan tetapi text - generation ini menggunakan model distilgpt2 dimana ini versi yang lebih ringan dari model GPT-2. Akan tetapi dapat mempertahankan kualitas produksi teks yang baik. Parameter yang dapat diatur:

- **max_length**: Panjang maksimum teks yang dihasilkan.
- **num_return_sequences**: Jumlah hasil yang ingin Anda dapatkan.

### 4. Fill-Mask
Fill-mask ini berguna untuk mengisi bagian yang hilang dalam teks dengan kata atau frasa yang sesuai. Dengan kata lain mengisi kalimat rumpang. Kata yang hilang akan ditandai dengan tanda "mask" didalam <>. Parameter top_k=2 digunakan untuk menampilkan dua prediksi terbaik dari model.

### 5. Named Entity Recognition (NER)
ner (Named Entity Recognition) digunakan unutk proses identifikasi atau klasifikasi dalam teks seperti nama orang, lokasi, organisasi dan lain-lainnya. Dimana Parameter grouped_entities=True digunakan untuk mengelompokkan kata-kata yang termasuk dalam satu entitas. Hasil contoh yang telah di buat PER adalah label untuk person dan LOC label untuk lokasi. Setiap label tersebut diberikan skor untuk menunjukkan keyakinan model untuk setiap entitas.

### 6. Question Answering
Nah pipeline ini berguna untuk menjawabn pertanyaan berdasarkan konteks ynag sebelumnya telah diberikan. Model ini mencari informasi dalam teks relevan dengan pertanyaan.

### 7. Sentiment Analysis
Sentimen-analysis berguna untuk menganalisis sentimen dari teks yang telah kita berikan. Pipeline akan memberikan hasil nya berupa identifikasi apakah sentimen dari teks tersebut positif, negatif atau netral. Model akan memberikan label sentimen beserta skor keyakinan (confidence score) untuk sentimen tersebut. Analisis sentimen dapat dilakukan pada berbagai jenis teks, seperti:
- Ulasan produk
- Tweet
- Artikel berita
- Posting media sosial
- Feedback pelanggan
- Survei.

### 8. Summarization
Summarization berguna untuk merangkum atau mengambil poin - poin utama dari teks panjang menjadi versi ynag lebih singkat, tetapi tetap mempertahankan informasi penting di dalamnya.Fungsi ini berguna dalam berbagai aplikasi seperti pembuatan ringkasan artikel, membantu pengguna memahami isi dokumen yang panjang, atau mempercepat pemrosesan informasi. Parameter yang digunakan:

- **max_length**: Panjang maksimum ringkasan.
- **min_length**: Panjang minimum ringkasan.
- **do_sample=False**: Menghasilkan hasil yang deterministik.

### 9. Translation

Pipeline ini digunakan untuk menerjemahkan teks. Model yang digunakan adalah `Helsinki-NLP/opus-mt-id-en`, yang menerjemahkan dari bahasa Indonesia ke bahasa Inggris. Anda juga dapat menyesuaikan model untuk bahasa lain.

<p>Bergabunglah dengan kami dalam petualangan NLP ini. Siapkan popcorn dan nikmati perjalanan kita menjelajahi dunia teks yang luar biasa! Jika Anda menemukan bug, jangan ragu untuk menghubungi kami. Kami akan menangani masalah itu dengan senyuman! 😄

Terima kasih telah membaca! Semoga hari Anda menyenangkan dan penuh inspirasi! 🎉</p>
