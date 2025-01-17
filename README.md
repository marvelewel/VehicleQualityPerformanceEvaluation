# 🚗 Prediksi Evaluasi Mobil (Car Evaluation Prediction)

## 📖 Latar Belakang

Evaluasi kualitas mobil merupakan hal yang penting dalam industri otomotif. Dengan menganalisis berbagai faktor seperti harga beli, biaya perawatan, kapasitas penumpang, dan tingkat keamanan, kita dapat menentukan seberapa layak sebuah mobil untuk digunakan.

## 🎯 Tujuan Proyek

Proyek ini bertujuan untuk membangun model pembelajaran mesin guna memprediksi evaluasi mobil berdasarkan dataset yang tersedia. Model ini dapat membantu dalam proses pengambilan keputusan bagi pembeli dan produsen mobil.

## 📊 Dataset

Dataset yang digunakan berasal dari **UCI Machine Learning Repository: Car Evaluation Dataset**. Dataset ini berisi atribut-atribut berikut:

- **Buying**: Harga beli mobil (low, med, high, vhigh)
- **Maint**: Biaya perawatan (low, med, high, vhigh)
- **Doors**: Jumlah pintu (2, 3, 4, 5more)
- **Persons**: Kapasitas penumpang (2, 4, more)
- **Lug_boot**: Kapasitas bagasi (small, med, big)
- **Safety**: Tingkat keamanan (low, med, high)
- **Class**: Label evaluasi mobil (unacc, acc, good, vgood)

## 🛠️ Metode yang Digunakan

1. **Pra-pemrosesan Data**
   - Mengonversi data kategorikal ke dalam bentuk numerik menggunakan Label Encoding.
   - Membagi dataset menjadi training dan testing set dengan rasio yang bervariasi (75-25, 60-40, 90-10).

2. **Model Pembelajaran Mesin**
   - **Random Forest Classifier**
   - Evaluasi model dengan berbagai parameter (n_estimators dan max_depth).

3. **Evaluasi Model**
   - **Akurasi**
   - **Precision, Recall, dan F1-Score**

## 📂 Struktur Proyek

```
📁 CarEvaluationPrediction
│── 📄 VehicleQualityPerformance.ipynb  # Notebook utama
│── 📄 car_evaluation.csv               # Dataset yang diambil dari UCL Repository
│── 📄 README.md                        # Dokumentasi proyek
```

## ⚙️ Instalasi dan Cara Menjalankan

### 1️⃣ Prasyarat

Pastikan Anda telah menginstal Python serta pustaka yang diperlukan:

```bash
pip install pandas numpy seaborn scikit-learn matplotlib
```

### 2️⃣ Jalankan Notebook

Buka Jupyter Notebook dan jalankan `VehicleQualityPerformance.ipynb` untuk melihat hasil analisis secara langsung.

```bash
jupyter notebook VehicleQualityPerformance.ipynb
```

## 📈 Hasil Akhir

- **Evaluasi Model dengan Parameter Terbaik**:
  ```
  Hasil terbaik:
  accuracy     94.91%
  precision    94.85%
  recall       94.91%
  Dengan konfigurasi: split_ratio = 0.25, n_estimators = 20, max_depth = 10
  ```

## 🏆 Kesimpulan

Berdasarkan hasil evaluasi, model **Random Forest Classifier** dengan parameter **n_estimators = 20 dan max_depth = 10** pada rasio **75-25** menghasilkan akurasi terbaik sebesar **94.91%**. Oleh karena itu, model ini dapat dianggap sebagai model yang paling optimal untuk memprediksi evaluasi mobil berdasarkan dataset yang digunakan.


🚀 **Terima kasih!**

