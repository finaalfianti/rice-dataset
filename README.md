# Submission Proyek Model Klasifikasi Gambar Beras

Repositori ini berisi hasil pelatihan model klasifikasi gambar beras dan konversinya ke berbagai format, serta notebook dan file dependensi proyek.

## Deskripsi Proyek

Model dikembangkan untuk mengklasifikasikan gambar butiran beras ke dalam lima kategori berikut:

- **Arborio**
- **Basmati**
- **Ipsala**
- **Jasmine**
- **Karacadag**

Dataset yang digunakan terdiri dari ribuan gambar tiap kelas yang telah dibagi ke dalam folder train, validation, dan test. Augmentasi gambar juga digunakan untuk meningkatkan performa generalisasi model.

Model dilatih menggunakan arsitektur CNN (Convolutional Neural Network) dengan teknik optimasi dan regularisasi standar. Setelah proses pelatihan, model diekspor ke dalam tiga format untuk berbagai kebutuhan deployment.

## Format Model

- `saved_model/` – Format standar TensorFlow untuk inferensi server-side dan kelanjutan pelatihan.
- `tflite/` – Format TensorFlow Lite untuk digunakan pada perangkat mobile/embedded.
- `tfjs_model/` – Format TensorFlow.js untuk aplikasi berbasis web.

## Cara Menjalankan

**1. Setup environment (opsional, jika menggunakan virtualenv/pipenv):**

```bash
mkdir Klasifikasi_Beras
cd Klasifikasi_Beras
pip install -r requirements.txt
```

**2. Jalankan notebook:**
Buka notebook.ipynb untuk melihat seluruh proses mulai dari preprocessing, pelatihan, evaluasi, hingga konversi model.
