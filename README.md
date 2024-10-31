<h1 align="center"> Natural Language Processing with Hugging Face Transformers </h1>
<p align="center"> Berisi pipe line dari Hugging Face Transformers untuk keperluan Natural Language Processing (NLP) </p>

<div align="center">

<img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54">
<img src="https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white">

<h1 align="center"> Analisis </h1>

NLP With Hugging Face Transformers

<p>1. zero-shot-classification</p>

  Setelah aku melakukan percobaan menggunakan zero ini berfungsi untuk mengklasifikasikan teks yang tidak memerlukan pelatihan pelatihan untuk setiap kategori. Model dapat mengklasifikasikan teks tersebut hanya dengan berdasarkan deskripsi label yang kita berikan. Hasil nya akan memberikan kategori yang sesuai serta menunjukkan berapa  skor probabilitas dari setiap label yang ada dari klasifikasi teks yang kita berikan.
2. text-generation
  
  Dari percobaan yang telah aku buat, text - generation ini berfungsi sebagai mana untuk menghasilkan teks secara otomatis, berdasarkan teks atau kalimat awal yang telah kita inputkan. Yang mana hasil pipeline ini menciptakan kalimat atau paragraf sesuai dengan input yang diberikan. Selain itu juga membantu penulis dalam menghasilakn ide, menciptakan respons pada chatbot dan juga menghasilkan dialog atau narasi.
3. text-generation" dengan model="distilgpt2

  Sama seperti poin no2 akan tetapi text - generation ini menggunakan model distilgpt2 dimana ini versi yang lebih ringan dari model GPT-2. Akan tetapi dapat mempertahankan kualitas produksi teks yang baik. Dengan parameter :

  a. max_length: Panjang maksimum teks yang dihasilkan.

  b. num_return_sequences: Jumlah hasil yang ingin Anda dapatkan

4. fill-mask

  Dilihat dari contoh di atas, fill-mask ini berguna untuk mengisi bagian yang hilang dalam teks dengan kata atau frasa yang sesuai. Dengan kata lain mengisi kalimat rumpang. Kata yang hilang akan ditandai dengan tanda "mask" didalam <>. Parameter top_k=2 digunakan untuk menampilkan dua prediksi terbaik dari model.

5. "ner", grouped_entities=True

  Diliat dari contoh di atas, ner (Named Entity Recognition) digunakan unutk proses identifikasi atau klasifikasi dalam teks seperti nama orang, lokasi, organisasi dan lain-lainnya. Dimana Parameter grouped_entities=True digunakan untuk mengelompokkan kata-kata yang termasuk dalam satu entitas. Hasil contoh yang telah di buat PER adalah label untuk person dan LOC label untuk lokasi. Setiap label tersebut diberikan skor untuk menunjukkan keyakinan model untuk setiap entitas.

6. "question-answering", model="distilbert-base-cased-distilled-squad"

  Nah pipeline ini berguna untuk menjawabn pertanyaan berdasarkan konteks ynag sebelumnya telah diberikan. Model ini mencari informasi dalam teks relevan dengan pertanyaan.

7. sentiment-analysis

  Bisa kita lihat dari contoh diatas sentimen-analysis berguna untuk menganalisis sentimen dari teks yang telah kita berikan. Pipeline akan memberikan hasil nya berupa identifikasi apakah sentimen dari teks tersebut positif, negatif atau netral. Model akan memberikan label sentimen beserta skor keyakinan (confidence score) untuk sentimen tersebut. Analisis sentimen dapat dilakukan pada berbagai jenis teks, seperti:
Ulasan produk, Tweet, Artikel berita, Posting media sosial, Feedback pelanggan, Survei.

8. summarization

  Berdasarkan contoh yang ada, summarization berguna untuk merangkum atau mengambil poin - poin utama dari teks panjang menjadi versi ynag lebih singkat, tetapi tetap mempertahankan informasi penting di dalamnya.  Parameter max_length dan min_length mengatur panjang maksimum dan minimum dari ringkasan yang dihasilkan, sementara do_sample=False memastikan bahwa hasilnya deterministik (tidak acak). Fungsi ini berguna dalam berbagai aplikasi seperti pembuatan ringkasan artikel, membantu pengguna memahami isi dokumen yang panjang, atau mempercepat pemrosesan informasi.

9. "translation", model="Helsinki-NLP/opus-mt-id-en"

  Pipeline ini digunakan untuk menerjemahkan kata atau kalimat. Dengan model="Helsinki-NLP/opus-mt-id-en yang aku gunakan diatas, teks atau kalimat akan diterjemahkan dari bahasa indonesia ke inggris. Kita jga bisa mmebuat tejemahan bahasa lain sesuai dengan keinginan masing".

  Thank you 🫡

