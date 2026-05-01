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
</p>

