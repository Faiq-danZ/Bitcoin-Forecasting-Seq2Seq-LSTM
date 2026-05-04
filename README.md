# 🚀 Bitcoin Price Forecasting: Seq2Seq LSTM Engine
![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.15-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-FF0000?style=for-the-badge&logo=keras&logoColor=white)
![Numpy](https://img.shields.io/badge/Numpy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)

### 📟 Overview
Proyek ini mengimplementasikan arsitektur **Deep Learning Sequence-to-Sequence (Seq2Seq)** menggunakan unit **LSTM** untuk memprediksi harga Bitcoin. Fokus utama proyek ini adalah menerapkan *Custom Layers* (Multi-Head Attention, Layer Norm) dan *Teacher Forcing* guna menangani volatilitas data *time-series* cryptocurrency.

Dikembangkan oleh mahasiswa **Mekatronika dan Kecerdasan Buatan**, Universitas Pendidikan Indonesia.

### 🏗️ Model Architecture
Model dibangun menggunakan kombinasi **Keras Functional API** dan **Model Subclassing**:
*   **Encoder-Decoder Structure**: Mengekstrak pola temporal masa lalu untuk memprediksi jendela waktu masa depan.
*   **Custom Multi-Head Attention**: Mekanisme atensi untuk menangkap korelasi antar waktu yang signifikan.
*   **Custom Layer Normalization & Dropout**: Teknik regulasi untuk stabilitas training di lingkungan GPU.
*   **Optimization**: Menggunakan **Adam Optimizer** dengan integrasi `ReduceLROnPlateau` dan `EarlyStopping`.

### 📊 Performance Results
Eksperimen dijalankan menggunakan **NVIDIA T4 GPU** dengan hasil sebagai berikut:
*   **Initial Loss**: 0.433
*   **Final Training Loss**: ~0.037
*   **Best Validation Loss**: `0.045888`
*   **Training Time**: Dioptimalkan secara signifikan dengan akselerasi hardware.

### 🛠️ Tech Stack
*   **Core**: TensorFlow 2.x, Keras
*   **Data**: Pandas, NumPy, Scikit-learn
*   **Visualization**: Matplotlib (Retro-Tech Theme)
*   **Dataset**: `Bitcoin3.csv`

### 🚀 Setup & Installation
1.  **Clone Repositori**:
    ```bash
    git clone [https://github.com/username/Bitcoin-Forecasting-Seq2Seq-LSTM.git](https://github.com/username/Bitcoin-Forecasting-Seq2Seq-LSTM.git)
    ```
2.  **Upload Dataset**: Pastikan file `Bitcoin3.csv` berada di direktori yang sama dengan notebook.
3.  **Run on Colab**: Direkomendasikan menggunakan Google Colab dengan mengaktifkan **GPU T4** pada pengaturan *Runtime*.

### 👨‍💻 Author
**Ahmad Faiq Zidane**  
*Undergraduate Student in Mechatronics and Artificial Intelligence*  
**Universitas Pendidikan Indonesia (UPI)**

---
> **Disclaimer:** Proyek ini adalah hasil riset akademik. Segala bentuk prediksi finansial yang dihasilkan tidak boleh digunakan sebagai saran investasi resmi.
