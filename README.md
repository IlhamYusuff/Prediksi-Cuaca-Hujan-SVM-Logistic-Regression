# 🌦️ Weather Prediction — Logistic Regression & SVM

Project Machine Learning untuk memprediksi Turunnya hujan berdasarkan data cuaca dari berbagai weather station Australia

Project ini membandingkan dua algoritma klasifikasi:

- Logistic Regression
- Support Vector Machine (SVM)

## 📊 Dataset

Dataset yang digunakan adalah **Weather Australia (`weatherAUS.csv`)** dengan:

- 145,460 data
- 23 features kolom
- Target: `RainTomorrow`

Target memiliki dua kelas:

- `Yes` → Hujan
- `No` → Tidak Hujan

## ⚙️ Workflow

```text
Data Collection
      ↓
Data Cleaning
      ↓
EDA
      ↓
Preprocessing
      ↓
Feature Engineering
      ↓
Train-Test Split
      ↓
Feature Scaling
      ↓
Model Training
      ↓
Model Evaluation
      ↓
Model Comparison
🤖 Model Performance
```
## Output dan Kesimpulan
```text
Akurasi Model
Logistic Regression	84.07%
SVM	83.98%

Logistic Regression kemudian digunakan untuk proses deployment dan inference.

Precesion
*   Untuk kelas 0, precision sekitar 86%, menunjukkan bahwa sekitar 86% dari prediksi positif untuk kelas 0 adalah benar. Ini mengindikasikan model memiliki kemampuan yang baik untuk mengidentifikasi kelas 0.
*   Untuk kelas 1, precision sekitar 72%, menunjukkan bahwa sekitar 72% dari prediksi positif untuk kelas 1 adalah benar.Ini mengindikasikan model memiliki kemampuan yang baik untuk mengidentifikasi kelas 1.

Recall
*   Untuk kelas 0, recall sangat tinggi, sekitar 95%, menunjukkan bahwa model berhasil mengidentifikasi sekitar 95% dari semua instance yang sebenarnya milik kelas 0.
*   Untuk kelas 1, recall lebih rendah, sekitar 43%, menunjukkan bahwa model hanya berhasil mengidentifikasi sekitar 43% dari semua instance yang sebenarnya milik kelas 1.

F1-Score
*   Untuk kelas 0, F1-score sekitar 90%, menunjukkan keseimbangan yang baik antara precision dan recall.
*   Untuk kelas 1, F1-score sekitar 54%, menunjukkan ada ruang untuk perbaikan dalam keseimbangan antara precision dan recall untuk kelas ini.

Akurasi
*   Akurasi keseluruhan model adalah  84%, yang merupakan rasio instans yang diprediksi dengan benar dibandingkan dengan total instans.


KESIMPULAN

*   Dari tahun ke tahun untuk rata-rata temperatur maksimum dan temperatur minimum fluktuatif. Namun, temperatur maksimum dan temperatur minimum terendah ada pada tahun 2012.

*   lokasi dengan frekuensi hujan paling banyak adalah Portland,sedangkan Rata-rata banyakya turun hujan adalah di Townsville dengan rata-rata curah hujan sebesar 20.08mm selama 10 tahun terakhir.

*   Kolom yang dibuang saat melakukan modelling adalah kolom Date, month, year, dan location karena tidak berpengaruh pada prediksi. Selain itu, WindDir9am dan WindDir3pm dibuang karena telah direpresentasikan oleh kolom WindGustDir.

*   Akurasi testing data dari kedua model lebih rendah dibandingkan training data. Maka kedua model termasuk underfitting.

*   Untuk Deployment menggunakan model Logistic Regression karena akurasi data testing yang lebih tinggi dibandingkan model SVM.

*  Dari hasil deployment menggunakan LR diketahui bahwa model ini memiliki presisi yang relatif tinggi untuk kelas 0 dan presisi yang lebih rendah untuk kelas 1. Meskipun model memiliki recall yang tinggi untuk kelas 0, recall untuk kelas 1 lebih rendah.
```

## 🛠️ Tech Stack
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- SciPy
- Statsmodels
- Jupyter Notebook / Google Colab


Clone repository:

git clone https://github.com/ilhamYusuf03/H8_PYTN-Ks20-06_5.git


👤 Author

Ilham Yusuf
