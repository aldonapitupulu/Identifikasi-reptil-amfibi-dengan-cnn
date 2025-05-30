# Klasifikasi Reptil dan Amfibi Menggunakan CNN

Proyek ini merupakan bagian dari skripsi yang bertujuan untuk mengklasifikasikan gambar reptil dan amfibi menggunakan model Convolutional Neural Network (CNN).

## 📂 Struktur Repositori

```
├── klasifikasi_cnn.ipynb ← Notebook utama
└── README.md              ← Dokumentasi ini
```

## 📌 Tahapan Penelitian

1. **Pengumpulan Data:**
   - Dataset terdiri dari 10 kelas:
     - **Reptil:** bunglon, iguana, buaya, tokek, kadal, ular, kura-kura
     - **Amfibi:** kodok, katak, salamander

2. **Pembagian Dataset:**
   - Data dibagi menjadi `train` sebanyak 4228, `val` sebanyak 1205, dan `test` sebanyak 612.
   - Tiap set memiliki 2 kategori: `reptil` dan `amfibi`.

3. **Preprocessing:**
   - Resize gambar 224x224
   - Normalisasi pixel
   - Augmentasi **hanya untuk amfibi** (flip, rotasi, & scaling)

4. **Model CNN:**
   - Dibuat dengan TensorFlow/Keras.
   - Arsitektur: beberapa Conv2D + MaxPooling + Flatten + Dense.

5. **Evaluasi:**
   - Akurasi & loss
   - Confusion Matrix
   

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
