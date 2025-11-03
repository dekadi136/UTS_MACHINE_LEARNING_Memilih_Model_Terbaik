#  Prediksi Harga Properti dengan Regresi Polinomial & Regularisasi

Proyek ini adalah studi kasus *end-to-end* machine learning untuk memprediksi harga properti. Fokus utama dari proyek ini adalah untuk menganalisis **Bias-Variance Trade-off** dengan membandingkan berbagai tingkat kompleksitas (Polynomial Degree) dan metode regularisasi (Ridge vs. Lasso) untuk menemukan model yang paling optimal.

---

## 📂 Struktur Project

Berikut adalah struktur file dan folder dalam proyek ini:

📂 **UTS_ML/** 
├── .ipynb_checkpoints/  
├── best_model_lasso_deg2.pkl  
├── dataset_properti_non_linear.csv  
├── model_evaluation_results.csv  
├── model_harga_properti_terbaik.joblib  
├── scaler.pkl  
├── UTS_MachineLearning.ipynb  
└── UTS_ML_I Gede Suryananda Adikartika_220102....pdf
---

## 🛠️ Instalasi

Untuk menjalankan proyek ini, Anda disarankan menggunakan *virtual environment* agar tidak mengganggu instalasi Python utama Anda.

1.  **Clone repositori ini (jika ada):**
    ```bash
    git clone [URL-REPOSITORI-ANDA]
    cd [NAMA-DIREKTORI-PROYEK]
    ```

2.  **Buat dan aktifkan virtual environment:**
    ```bash
    # Membuat venv
    python -m venv venv

    # Mengaktifkan venv (macOS/Linux)
    source venv/bin/activate

    # Mengaktifkan venv (Windows)
    .\venv\Scripts\activate
    ```

3.  **Install dependencies:**
    Buat file `requirements.txt` dan salin teks di bawah ini ke dalamnya:

    **requirements.txt**
    ```
    pandas
    numpy
    scikit-learn
    matplotlib
    seaborn
    joblib
    notebook
    ```

    Lalu, jalankan perintah instalasi:
    ```bash
    pip install -r requirements.txt
    ```

---

## 🚀 Cara Menjalankan Code

Seluruh analisis dan pelatihan model terdapat di dalam file Jupyter Notebook.

1.  **Pastikan virtual environment Anda aktif.**

2.  **Jalankan Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```

3.  **Buka file notebook:**
    Browser Anda akan terbuka. Klik dan buka file `Proyek_Regresi_Properti.ipynb`.

4.  **Jalankan Semua Sel (Run All):**
    Di dalam notebook, Anda dapat memilih **"Cell" -> "Run All"** untuk menjalankan seluruh *pipeline* secara berurutan. Ini akan:
    * Membuat ulang file `dataset_properti_non_linear.csv`.
    * Menjalankan semua analisis EDA dan menampilkan semua plot.
    * Melatih dan mengevaluasi 35 model.
    * Menyimpan tabel perbandingan ke `model_evaluation_results.csv`.
    * Melatih dan menyimpan model final ke `model_harga_properti_terbaik.joblib`.
    * Menjalankan prediksi contoh pada 5 data baru.
