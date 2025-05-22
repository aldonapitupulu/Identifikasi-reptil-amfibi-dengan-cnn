# Klasifikasi Reptil dan Amfibi Menggunakan CNN

Proyek ini merupakan bagian dari skripsi yang bertujuan untuk mengklasifikasikan gambar reptil dan amfibi menggunakan model Convolutional Neural Network (CNN).

## 📂 Struktur Repositori

```
├── dataset/               ← Contoh data & petunjuk unduh dataset
├── klasifikasi_cnn.ipynb ← Notebook utama
├── requirements.txt       ← Daftar library
├── .gitignore
└── README.md              ← Dokumentasi ini
```

## 📌 Tahapan Penelitian

1. **Pengumpulan Data:**
   - Dataset terdiri dari 9 kelas:
     - **Reptil:** iguana, buaya, tokek, kadal, ular, kura-kura
     - **Amfibi:** kodok, katak, salamander

2. **Pembagian Dataset:**
   - Data dibagi menjadi `train`, `val`, dan `test`.
   - Tiap set memiliki 2 kategori: `reptil` dan `amfibi`.

3. **Preprocessing:**
   - Resize gambar
   - Normalisasi pixel
   - Augmentasi **hanya untuk amfibi** (rotasi & scaling)

4. **Model CNN:**
   - Dibuat dengan TensorFlow/Keras.
   - Arsitektur: beberapa Conv2D + MaxPooling + Flatten + Dense.

5. **Evaluasi:**
   - Confusion Matrix
   - Akurasi & loss
   - Grafik performa

## 🚀 Cara Menjalankan Program

### 1. Clone Repositori
```bash
git clone https://github.com/username/klasifikasi-reptil-amfibi-cnn.git
cd klasifikasi-reptil-amfibi-cnn
```

### 2. Install Library
```bash
pip install -r requirements.txt
```

### 3. Jalankan Notebook
Buka `klasifikasi_cnn.ipynb` di Jupyter Notebook atau Google Colab.

## 📁 Dataset

Dataset lengkap tersedia di Google Drive:

[Link Google Drive Dataset](https://drive.google.com/your-link)

Struktur folder:
```
├── train/
│   ├── reptil/
│   └── amfibi/
├── val/
│   ├── reptil/
│   └── amfibi/
└── test/
    ├── reptil/
    └── amfibi/
```

---

## ✍️ Lisensi
Repositori ini dibuat untuk keperluan edukasi dan tugas akhir.
