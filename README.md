# Mobil vs Motor – Transfer Learning Image Classification

Tugas ini merupakan bagian dari mata kuliah **Machine Learning**, di mana saya membangun model klasifikasi gambar untuk dua objek berbeda: **Mobil** dan **Motor** menggunakan metode **Transfer Learning**.

## Deskripsi Proyek

Proyek ini menggunakan pendekatan **Transfer Learning** dengan pretrained model **VGG16** untuk membedakan gambar **Mobil** dan **Motor** berdasarkan dataset yang dikumpulkan secara manual. Dataset berisi **200 gambar**, masing-masing 100 gambar untuk setiap kelas dengan variasi sudut pengambilan.

## Tools & Library

- Python
- Google Colab
- TensorFlow & Keras
- NumPy, Pandas, Matplotlib
- Scikit-learn
- OpenCV (jika digunakan untuk preprocessing)
- Git & GitHub

## Model Transfer Learning

- **Model**: VGG16
- **Strategi**:
  - Layer awal dibekukan (frozen)
  - Ditambahkan Dense layer untuk klasifikasi 2 kelas
  - Optimizer: Adam
  - Loss function: Binary Crossentropy
  - Metric: Accuracy

## Dataset

- **Jumlah total**: 200 gambar
  - Mobil: 100 gambar
  - Motor: 100 gambar
- **Sumber**: Koleksi pribadi/manual
- **Format**: JPG/PNG
- **Ukuran gambar**: Diresize ke (224, 224)
- **Split data**:
  - 80% training
  - 20% validation

## Hasil & Evaluasi

- **Akurasi akhir**: 100% (1.00)
- **Confusion Matrix**:

  |        | Pred Mobil | Pred Motor |
  |--------|------------|------------|
  | Mobil  | 100        | 0          |
  | Motor  | 0          | 100        |

- **Classification Report**: Precision, recall, dan f1-score semua 1.00 untuk kedua kelas, menandakan model bekerja sempurna pada dataset validasi.
- **Visualisasi**:
  - Grafik akurasi dan loss selama training
    
    ![akurasi](https://github.com/user-attachments/assets/382f6e7a-03eb-441c-a0d5-719ec91b6115)
    ![loss](https://github.com/user-attachments/assets/82921f3a-0604-43a5-aa54-d15954f0760f)

## Refleksi Pribadi

Saya mempelajari cara mengimplementasikan transfer learning menggunakan model pretrained dan pentingnya kualitas serta variasi data dalam meningkatkan akurasi klasifikasi. Tantangan utama adalah mengumpulkan gambar yang beragam dan menyesuaikan preprocessing agar sesuai dengan arsitektur model. Proyek ini membantu saya memahami alur kerja machine learning dari awal hingga evaluasi.

## File dalam Repository

| Nama File        | Deskripsi                                    |
|------------------|----------------------------------------------|
| `tugas-transfer-learning.ipynb` | Notebook utama berisi seluruh proses coding |
| `README.md`       | Deskripsi proyek ini                        |
| `laporan.pdf`     | Laporan lengkap dalam format PDF            |
| `dataset/`        | Folder dataset berisi gambar mobil dan motor |

## Link Tugas

- GitHub Repo: [https://github.com/nailafath/Mobil-vs-Motor](https://github.com/nailafath/Mobil-vs-Motor)

---
