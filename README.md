# Bank Marketing ID3 Classification

Implementasi **Decision Tree (ID3)** untuk memprediksi keputusan nasabah dalam kampanye marketing bank (apakah nasabah akan berlangganan deposito / menerima tawaran atau tidak).  

---

## 📌 Project Overview
Tahapan utama dalam project ini meliputi:

1. **Dataset Preparation**
2. **Data Preprocessing**
3. **Training Model dengan ID3**
4. **Handling Imbalanced Dataset**
5. **Hyperparameter Tuning**
6. **Optimisasi menggunakan Genetic Algorithm (GA)**
7. **Evaluasi Model**

---

## 🎯 Tujuan
Memprediksi keputusan nasabah dalam kampanye marketing bank:

- **Yes**  → nasabah menerima / berlangganan
- **No**   → nasabah tidak menerima

---

## 📂 Struktur Folder Repository
Berikut struktur folder utama pada repository ini:

- `code/` → source code / notebook implementasi  
- `dataset/` → dataset mentah dan/atau dataset hasil preprocessing  
- `prediction_ID3/` → hasil prediksi / output model  
- `report/` → laporan tugas besar (PDF/DOC)  
- `requirement/` → ketentuan / aturan tugas besar 
- `README.md` → dokumentasi project

---

## 🧠 Algoritma yang Digunakan
### ✅ Decision Tree - ID3 (Iterative Dichotomiser 3)
ID3 membangun pohon keputusan berdasarkan **Information Gain** untuk memilih atribut terbaik sebagai node pemisah.

---

## ⚠️ Permasalahan: Imbalanced Dataset
Dataset yang digunakan memiliki **ketidakseimbangan kelas** (jumlah label *Yes* dan *No* tidak seimbang).  
Hal ini menyebabkan model cenderung bias terhadap kelas mayoritas.

✅ Solusi yang dilakukan:
- Menggunakan pendekatan penanganan imbalance (misalnya: oversampling / undersampling / class weight)  
- Evaluasi tidak hanya mengandalkan accuracy, tapi juga metrik lain seperti precision, recall, dan F1-score.

---

## 🔧 Hyperparameter Tuning
Untuk meningkatkan performa model, dilakukan **hyperparameter tuning** pada ID3, contoh parameter yang diuji:

- `max_depth` (kedalaman pohon)
- `min_samples_split`
- `min_samples_leaf`
- pemilihan fitur / batasan split

Tujuannya untuk mendapatkan konfigurasi terbaik dan mengurangi risiko **overfitting**.

---

## 🧬 Optimisasi Menggunakan Genetic Algorithm (GA)
Selain tuning, project ini juga menggunakan **Genetic Algorithm (GA)** sebagai metode optimisasi.

GA digunakan untuk mencari kombinasi parameter terbaik (atau seleksi fitur terbaik) dengan cara:
- **Selection**
- **Crossover**
- **Mutation**
- **Fitness Evaluation**

🎯 Goal: meningkatkan performa model ID3 berdasarkan nilai **fitness** (misalnya F1-score / accuracy / kombinasi metrik evaluasi).

---

## 📊 Evaluasi Model
Metrik evaluasi yang digunakan:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

Karena dataset imbalance, metrik seperti **Recall** dan **F1-score** menjadi fokus utama.

---

## 🛠️ Tools & Library
Project ini dikerjakan menggunakan:
- Python
- Jupyter Notebook
- Pandas, NumPy
- Scikit-learn
- Matplotlib / Seaborn (visualisasi)
