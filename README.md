# Klasifikasi Reptil dan Amfibi Menggunakan CNN

Proyek ini merupakan bagian dari skripsi yang bertujuan untuk mengklasifikasikan gambar reptil dan amfibi menggunakan model Convolutional Neural Network (CNN).

## 📂 Struktur Repositori

```
├── klasifikasi_cnn.ipynb ← Notebook utama
├── requirements.txt       ← Daftar library
└── README.md              ← Dokumentasi ini
```

## 📌 Tahapan Penelitian

1. **Pengumpulan Data:**
   - Dataset terdiri dari  kelas:
     - **Reptil:** bunglon, iguana, buaya, tokek, kadal, ular, kura-kura
     - **Amfibi:** kodok, katak, salamander

2. **Pembagian Dataset:**
   - Data dibagi menjadi `train`, `val`, dan `test`.
   - Tiap set memiliki 2 kategori: `reptil` dan `amfibi`.

3. **Preprocessing:**
   - Resize gambar
   - Normalisasi pixel
   - Augmentasi **hanya untuk amfibi** (flip, rotasi, & scaling)

4. **Model CNN:**
   - Dibuat dengan TensorFlow/Keras.
   - Arsitektur: beberapa Conv2D + MaxPooling + Flatten + Dense.

5. **Evaluasi:**
   - Confusion Matrix
   - Akurasi & loss
   

## 🚀 Cara Menjalankan Program

### 1. Jalankan Notebook
download dan jalankan `TA.ipynb` di Google Colab.

## 📁 Dataset

Dataset lengkap tersedia di Google Drive:

[Link Google Drive Dataset](https://drive.google.com/drive/folders/1nWvslXXB3hvEI2qZeDzq-tB6Xal15J-q?usp=drive_link)
[Link Google Drive Dataset](https://drive.google.com/drive/folders/1jbI_CygNIB5ppGxt3Guiku52L5kudFJI?usp=sharing)

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
