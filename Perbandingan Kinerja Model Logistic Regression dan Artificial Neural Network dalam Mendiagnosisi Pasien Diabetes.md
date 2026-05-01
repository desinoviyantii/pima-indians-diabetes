### **DATABASE**<br>
[Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)

### **ANALISIS SEBARAN VARIABEL BEBAS DAN VARIABEL TARGET** <br>
<p align="justify">
Data Pima Indians Diabetes terdiri dari delapan variabel bebas dengan satu variabel target (kategori: 1 dan 0). Variabel bebas meliputi Pregnancies, Glucose, Blood Pressure, Skin Thickness, Insulin, BMI, Diabetes Pedigree Function (DPF), dan Age.<br>
  
Berdasarkan variabel target, terdapat 268 pasien positif diabetes dengan persentase sebesar 35% dan 500 pasien dinyatakan negatif diabetes dengan persentase sebesar 65%.
<img width="1100" height="731" alt="image" src="https://github.com/user-attachments/assets/9b0f0efd-85f2-4e39-a701-b9e930ba5d89" />
  <p align="center">
    Distribusi Variabel Bebas
<p align="justify">
Variabel Glucose, Blood Pressure, Skin Thickness, Insulin, dan BMI akn dilakukan penanganan missing value karena nilai minumum 0 pada variabel-variabel ini mungkin menunjukkan adanya data yang tidak valid. Sedangkan, variabel Pregnancies dapat memiliki nilai 0 karena variabel ini menggambarkan jumlah kehamilan pasien, sehingga tidak memerlukan penanganan. Namun pada penelitian ini, outliers tidak ditangani secara khusus.

### **DETEKSI DAN PENANGANAN MISSING VALUE**
<p align="justify">
Penanganan missing values menggunakan metode Pengahapusan Baris (<5%) dan Imputasi Regresi Linear. Tujuan dari tahap ini adalah untuk memastikan bahwa data dalam kondisi bersih dan siap digunakan dalam model machine learning.

### **STANDARDISASI** <br>
<p align="justify">
Proses ini dilakukan khusus pada variabel bebas untuk memastikan bahwa semua fitur memberikan kontribusi yang seimbang dalam model, tanpa dipengaruhi oleh perbedaan skala antar variabel. Skala yang seragam dengan nilai harapan 0 dan simpangan baku 1

### **PEMBAGIAN DATA** <br>
<p align="justify">
Data Pima Indians Diabetes dibagi menjadi dua bagian, yaitu data training dan data testing dengan proporsi 70:30. Pengambilan data ini dilakukan secara acak menggunakan package train_test_split dalam library Python Scikit-learn dengan nilai RandomState=42.

### **MODEL LOGISTIC REGRESSION** <br>
<p align="justify">
Akurasi pada data testing sebesar 79.82% lebih tinggi daripada pada data training sebesar 76.68%, hal ini menunjukkan bahwa model mampu menangani data baru dengan baik. Selain itu, nilai AUC pada data testing sebesar 87.70%, yaitu lebih tinggi dari nilai AUC pada data training sebesar 82.56%, yang berarti model ini dapat membedakan kelas dengan baik pada data baru.

### **MODEL ARTIFICIAL NEURAL NETWORK** <br>
<p align="justify">
Akurasi hasil data training sedikit lebih tinggi, yaitu 81.82%, dibandingkan dengan akurasi hasil data testing sebesar 80.73%. Meskipun terdapat sedikit penurunan akurasi hasil pada data testing, model ini tetap efektif dalam menangani data baru. Selain itu, perbedaaan akurasi yang relatif kecil ini mengindikasikan bahwa model tidak mengalami overfitting. Hal ini juga diperkuat oleh nilai AUC yang baik, di mana nilai AUC pada data training sebesar 89.53% dan data testing sebesar 87.53%.

### **EVALUASI** <br>
<p align="justify">
Model terbaik berdasarkan nilai akurasi dan AUC antara kedua model adalah model Artificial Neural Network (ANN). ANN memiliki akurasi hasil yang lebih tinggi dibandingkan Logistic Regression, baik pada data training maupun data testing. Selain itu, model ANN juga lebih terhindar dari overfitting, karena selisih akurasi antara data training dan testing lebih kecil dibandingkan model Logistic Regression.

Akan tetapi berdasarkan ukuran kinerja waktu komputasinya, Logistic Regression hanya membutuhkan 0.0010 detik untuk data training dan 0.0003 detik untuk data testing, sementara ANN memerlukan 0.1291 detik pada data training dan 0.1513 detik pada data testing. Hal ini menunjukkan bahwa Logistic Regression lebih efisien dalam hal waktu komputasi dibandingkan ANN.
</p>

