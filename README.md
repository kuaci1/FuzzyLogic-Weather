Weather Prediction System Using Machine Learning
Proyek ini adalah implementasi sistem prediksi cuaca menggunakan berbagai algoritma Machine Learning. Sistem ini dirancang sebagai alternatif dan pengembangan dari metode Fuzzy Logic, dengan tujuan mencapai akurasi prediksi yang jauh lebih tinggi.

Sistem ini mengklasifikasikan kondisi cuaca berdasarkan parameter suhu, kelembapan, dan kecepatan angin.

🚀 Fitur Utama
Generate Data Otomatis: Script memiliki kemampuan untuk membuat dummy dataset yang realistis jika tidak ada file CSV eksternal.

Preprocessing Data: Penanganan missing values, outliers (menggunakan IQR), normalisasi (MinMaxScaler), dan encoding label.

Multi-Model Comparison: Melatih dan membandingkan 4 algoritma sekaligus.

Visualisasi: Plotting akurasi, Confusion Matrix, dan Feature Importance.

📊 Dataset
Dataset yang digunakan memiliki fitur sebagai berikut:

Input Features:
Temperature (°C)
Humidity (%)
Wind Speed (km/h)

Target Classes (Label):
Sunny, Rainy, Cloudy, Windy, Foggy, Hot_Humid, Cold_Windy, Pleasant.

🧠 Model yang Digunakan
Proyek ini melatih dan mengevaluasi empat algoritma machine learning populer:

Decision Tree Classifier
Random Forest Classifier
Support Vector Machine (SVM)
Gradient Boosting Classifier
