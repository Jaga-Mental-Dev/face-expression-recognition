# Facial Emotion Recognition (FER) Model with TensorFlow

## 📋 Deskripsi Proyek
Proyek ini adalah implementasi model **Facial Emotion Recognition (FER)** menggunakan TensorFlow. Model ini dirancang untuk mengenali ekspresi wajah manusia berdasarkan gambar, seperti *angry*, *happy*, *neutral*, dan *sad*. Dataset yang digunakan memiliki 21,005 gambar untuk pelatihan dan 5,212 gambar untuk pengujian, yang telah diproses menggunakan **data augmentation**.

---

## 🚀 Fitur
1. **Model Kustom CNN**:
   - Menggunakan arsitektur CNN yang dirancang untuk mendeteksi ekspresi wajah.
   - Mendukung 4 kelas emosi: *angry*, *happy*, *neutral*, *sad*.
2. **Data Augmentation**:
   - Meningkatkan variasi dataset menggunakan rotasi, zoom, dan flip horizontal.
3. **Pengolahan Data Otomatis**:
   - Pemrosesan dataset langsung dari struktur direktori.
4. **Visualisasi**:
   - Menampilkan distribusi data dan contoh gambar dari dataset.
5. **Training dengan GPU**:
   - Mendukung penggunaan GPU untuk mempercepat proses pelatihan.

---

## 📂 Struktur Proyek
```
facial_emotion_recognition/
│
├── dataset_4face/
│   ├── train/          # Folder dataset pelatihan (4 kelas)
│   ├── test/           # Folder dataset pengujian (4 kelas)
│
├── scripts/
│   ├── train_model.py  # Script untuk melatih model
│   ├── test_model.py   # Script untuk menguji model
│   └── utils.py        # Utility functions seperti data augmentation
│
├── models/
│   └── fer_model.h5    # Model hasil pelatihan (tersimpan)
│
├── notebooks/
│   └── FER_Training.ipynb  # Notebook eksplorasi data dan pelatihan
│
├── requirements.txt    # File dependensi
└── README.md           # Dokumentasi proyek
```

---

## ⚙️ Persyaratan
### Dependensi:
- Python 3.9
- TensorFlow 2.10.0
- Matplotlib
- Pandas
- Numpy
- PIL (Pillow)

Instalasi semua dependensi dapat dilakukan dengan:

```bash
pip install -r requirements.txt
```

---

## 📊 Dataset
Dataset tersimpan dalam struktur berikut:

```
dataset_4face/
├── train/
│   ├── angry/
│   ├── happy/
│   ├── neutral/
│   └── sad/
├── test/
│   ├── angry/
│   ├── happy/
│   ├── neutral/
│   └── sad/
```

Dataset harus terdiri dari gambar wajah berlabel sesuai dengan nama foldernya (*angry*, *happy*, *neutral*, *sad*).

---

## 🧪 Cara Penggunaan
### 1. Persiapan Dataset
Pastikan dataset tersimpan dalam struktur direktori seperti di atas.

### 2. Latih Model
Untuk melatih model, jalankan:

```bash
python scripts/train_model.py
```

### 3. Uji Model
Setelah pelatihan selesai, Anda dapat menguji model dengan:

```bash
python scripts/test_model.py
```

---

## 🔍 Visualisasi Data
Visualisasi distribusi kelas dapat dilakukan dengan memanfaatkan fungsi berikut:

- **Distribusi Dataset**:
  Menampilkan distribusi jumlah gambar untuk setiap kategori (train/test).

- **Visualisasi Gambar Contoh**:
  Memvisualisasikan beberapa gambar dari dataset beserta labelnya.

---

## 📜 Lisensi
Proyek ini menggunakan lisensi MIT. Silakan lihat [LICENSE](./LICENSE) untuk informasi lebih lanjut.

---

## 🙌 Kontribusi
Kontribusi terbuka untuk perbaikan dan pengembangan lebih lanjut. Silakan lakukan fork dan kirimkan pull request.

---

## 📧 Kontak
Jika ada pertanyaan atau masalah, silakan hubungi:
- **Email**: [gerhardien.p@gmail.com](gerhardien.p@gmail.com)

