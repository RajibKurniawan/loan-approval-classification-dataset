# loan-approval-classification-dataset

## New Machine Learning Project: Loan Approval Classification

Peningkatan jumlah pengajuan pinjaman pada lembaga keuangan dan fintech menuntut sistem evaluasi kredit yang cepat, objektif, dan efisien. Proyek ini membangun model machine learning untuk memprediksi apakah seorang pemohon layak disetujui atau termasuk kategori berisiko tinggi (default).
Model yang dikembangkan memanfaatkan variabel-variabel finansial, demografis, dan historis peminjam untuk menghasilkan prediksi yang lebih akurat.

## Business Objectives

Model ini dikembangkan untuk membantu lembaga keuangan dalam:

- Mengidentifikasi pemohon yang layak disetujui secara otomatis
- Mendeteksi pemohon berisiko tinggi secara lebih dini
- Meningkatkan efisiensi proses analisis kelayakan kredit
- Mengurangi risiko kredit macet (default)

## Dataset Overview

- Jumlah data: ±45.000 baris
- Fitur: 14 fitur prediktor + 1 target (Loan_Status)
- Target variable:
  - 0 = Pinjaman ditolak
  - 1 = Pinjaman disetujui
- Tipe fitur:
  - Numerik -> Age, Income, Credit_Score, Loan_Amount, Loan_Interest_Rate, dll.
  - Kategorikal -> Gender, Education_Level, Loan_Purpose, Home_Status, dll.
- Preprocessing mencakup:
  - Imputasi missing values
  - Outlier clipping (IQR)
  - Encoding (One-hot / Label encoding)
  - Scaling fitur numerik
  - Feature importance & selection

## Methodology

Pendekatan yang digunakan:

- Exploratory Data Analysis (EDA)
- Feature Engineering & Preprocessing
- Supervised Learning – Classification
- 5-Fold Cross Validation
- Hyperparameter Tuning

## Modeling & Evaluation

- Modeling Algorithms
  - Decision Tree
  - Random Forest
  - K-Nearest Neighbors (KNN)
  - Support Vector Machine (SVM)
  - XGBoost (Best Model)
  - Evaluation Metrics
  - F1-Score (utama)
  - ROC-AUC
  - Accuracy
  - Model XGBoost dipilih karena menghasilkan performa paling baik & tidak mengalami overfitting.

## Project Deliverables

- Model terbaik: best_model_xgboost.pkl

- Notebook utama: EDA -> preprocessing -> modeling -> evaluation

- Notebook inference: prediksi data user baru

- Streamlit App untuk real-time prediction

## Key Business Insights

- Pemohon dengan income stabil, skor kredit tinggi, dan rasio pinjaman rendah memiliki peluang besar untuk disetujui.
- Variabel Default_On_Payment dan Credit_Score merupakan indikator risiko paling kuat.
- Implementasi sistem otomatis dapat:
  - Mengurangi bias manual
  - Meningkatkan kecepatan approval
  - Menekan angka kredit macet

## Tech Stack

- Python 3.10+
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn
  - xgboost
  - pickle
- Tools:
  - Jupyter Notebook, Google Colab, Streamlit

## Explore the Project

- GitHub Repository : (<https://github.com/RajibKurniawan/loan-approval-classification-dataset>)
- Streamlit App : (<https://loanapprovaldeploy-rajibkurniawan.streamlit.app/>)
- Dataset : (<https://www.kaggle.com/datasets/taweilo/loan-approval-classification-data/data>)
