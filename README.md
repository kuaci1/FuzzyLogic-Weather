# Weather Prediction using Fuzzy Logic Systems

Repository ini berisi **Final Project mata kuliah Artificial Intelligence Fundamentals**  
**Kelompok 6 – Semester Genap 2024/2025**.

Proyek ini mengimplementasikan dan membandingkan beberapa metode **Fuzzy Inference System (FIS)** serta **Multi-Criteria Decision Making (MCDM)** untuk memprediksi kondisi cuaca berdasarkan data historis cuaca.

---

## 📌 Project Overview

Tujuan utama dari proyek ini adalah **memprediksi ringkasan cuaca**  
(seperti *Clear, Partly Cloudy, Mostly Cloudy, Overcast*) menggunakan tiga variabel input utama:

- **Temperature (Suhu)**
- **Humidity (Kelembapan)**
- **Wind Speed (Kecepatan Angin)**

Metode yang diimplementasikan dan dibandingkan dalam proyek ini adalah:

1. **Fuzzy Mamdani** (Min–Max Inference)
2. **Fuzzy Sugeno** (Linear Output)
3. **Fuzzy Tsukamoto** (Weighted Average)
4. **SAW (Simple Additive Weighting)**

---

## 📊 Dataset

Dataset yang digunakan adalah **Weather History Dataset**  
(contoh: data cuaca Szeged, Hungaria periode 2006–2016).

- **Sumber file**: `weatherHistory.csv`

### 🔧 Tahapan Preprocessing
Proses preprocessing data meliputi:

- Penanganan *missing values* menggunakan **median imputation**
- Penghapusan *outlier* dengan metode **Interquartile Range (IQR)**
- Normalisasi data menggunakan **MinMaxScaler**
- Reduksi data untuk fokus pada label cuaca utama:
  - Clear  
  - Partly Cloudy  
  - Mostly Cloudy  
  - Overcast  

---

## ⚙️ Methodology

### 1️⃣ Fuzzification

Fungsi keanggotaan yang digunakan adalah **Trapezoidal Membership Function (trapmf)** untuk setiap variabel input:

**Temperature (°C)**
- Cold (Dingin)
- Normal
- Hot (Panas)

**Humidity (0–1)**
- Low (Rendah)
- Medium (Sedang)
- High (Tinggi)

**Wind Speed (km/h)**
- Weak (Lemah)
- Medium (Sedang)
- Strong (Kencang)

---

### 2️⃣ Fuzzy Rules

Sistem menggunakan seperangkat aturan linguistik, contohnya:

