# UTS_Praktikum-Machine-Learning
1227050012 Aisyah Muthmainnah

# Klasifikasi Kelayakan Kredit Komputer dengan Algoritma Naive Bayes

## Dataset
Dataset yang digunakan berisi atribut-atribut sebagai berikut:

- `Age`: Muda, Paruh Baya, Tua
- `Income`: Rendah, Sedang, Tinggi
- `Student`: Ya atau Tidak
- `Credit_Rating`: Buruk atau Baik
- `Buys_Computer`: Target (0 = Tidak Layak, 1 = Layak)

## Tahapan dan Langkah-langkah

### 1. Import Library
Library yang digunakan:
- pandas, numpy
- scikit-learn 
- seaborn & matplotlib 

### 2. Preprocessing
- Encode semua fitur kategorikal menjadi numerik dengan `LabelEncoder`.
- Pisahkan fitur (X) dan target (y).
- Bagi data menjadi data training dan testing dengan rasio 80:20.

### 3. Pembuatan Model
- Menggunakan algoritma Gaussian Naive Bayes karena data sudah dalam bentuk numerik.

### 4. Pelatihan Model
- Melatih model pada data training menggunakan `.fit()`.

### 5. Prediksi
- Melakukan prediksi pada data testing menggunakan `.predict()`.

### 6. Evaluasi Model
- Menghitung akurasi dengan `accuracy_score`.
- Melihat performa tiap kelas dengan `classification_report`.
- Menampilkan confusion matrix untuk visualisasi performa model.

## 📈 Hasil Evaluasi

- **Akurasi Model**: 74%
- **Precision Kelas Layak**: 73.6%
- **Recall Kelas Layak**: 93%
- **Recall Kelas Tidak Layak**: 39.4%

Model sangat baik dalam mengenali siapa yang layak, namun cukup sering salah saat memprediksi yang tidak layak.

## Kesimpulan

Model Naive Bayes mampu memprediksi kelayakan kredit dengan performa cukup baik. Dengan akurasi 74% dan recall tinggi untuk kelas *layak*, model cocok digunakan jika tujuannya adalah memperluas akses kredit. Namun, perlu perbaikan lebih lanjut jika ingin menghindari kesalahan pada kelas *tidak layak*.
