<h1 align="center"> Natural Language Processing with Hugging Face Transformers </h1>
<p align="center"> Berisi pipe line dari Hugging Face Transformers untuk keperluan Natural Language Processing (NLP) </p>

<div align="center">

<img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54">
<img src="https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white">

<h1 align="center"> Analisis </h1>

NLP With Hugging Face Transformers

<h2>1. Zero-Shot Classification</h2>
Zero-Shot Classification ini berfungsi untuk mengklasifikasikan teks yang tidak memerlukan pelatihan pelatihan untuk setiap kategori. Model dapat mengklasifikasikan teks tersebut hanya dengan berdasarkan deskripsi label yang kita berikan. Hasil nya akan memberikan kategori yang sesuai serta menunjukkan berapa skor probabilitas dari setiap label yang ada dari klasifikasi teks yang kita berikan.
## 2. Text Generation

text - generation ini berfungsi sebagai mana untuk menghasilkan teks secara otomatis, berdasarkan teks atau kalimat awal yang telah kita inputkan. Yang mana hasil pipeline ini menciptakan kalimat atau paragraf sesuai dengan input yang diberikan. Ini berguna untuk : 

- Membantu penulis dalam mendapatkan ide.
- Menciptakan respons dalam chatbot.
- Menghasilkan dialog atau narasi.

## 3. Text Generation dengan Model DistilGPT2

Model ini adalah versi lebih ringan dari GPT-2, yaitu `distilgpt2`, yang tetap mempertahankan kualitas produksi teks yang baik. Parameter yang dapat diatur:

- **max_length**: Panjang maksimum teks yang dihasilkan.
- **num_return_sequences**: Jumlah hasil yang ingin Anda dapatkan.

## 4. Fill-Mask

Fill-mask berguna untuk mengisi bagian yang hilang dalam teks. Kata yang hilang ditandai dengan tanda `<mask>`. Dengan parameter `top_k=2`, Anda dapat menampilkan dua prediksi terbaik dari model.

## 5. Named Entity Recognition (NER)

NER digunakan untuk mengidentifikasi atau mengklasifikasikan entitas dalam teks seperti nama orang, lokasi, dan organisasi. Dengan parameter `grouped_entities=True`, model akan mengelompokkan kata-kata yang termasuk dalam satu entitas.

## 6. Question Answering

Pipeline ini menjawab pertanyaan berdasarkan konteks yang telah diberikan sebelumnya. Model yang digunakan adalah `distilbert-base-cased-distilled-squad`, yang mencari informasi relevan dalam teks.

## 7. Sentiment Analysis

Sentiment analysis berguna untuk menganalisis sentimen dari teks yang diberikan. Ini dapat digunakan untuk berbagai jenis teks seperti ulasan produk, tweet, dan artikel berita. Model akan memberikan label sentimen (positif, negatif, atau netral) beserta skor keyakinan.

## 8. Summarization

Summarization digunakan untuk merangkum teks panjang menjadi versi yang lebih singkat, tanpa kehilangan informasi penting. Parameter yang digunakan:

- **max_length**: Panjang maksimum ringkasan.
- **min_length**: Panjang minimum ringkasan.
- **do_sample=False**: Menghasilkan hasil yang deterministik.

## 9. Translation

Pipeline ini digunakan untuk menerjemahkan teks. Model yang digunakan adalah `Helsinki-NLP/opus-mt-id-en`, yang menerjemahkan dari bahasa Indonesia ke bahasa Inggris. Anda juga dapat menyesuaikan model untuk bahasa lain.
  Thank you 🫡

