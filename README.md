# 🫀 Heart Stroke Risk Prediction App

A **Machine Learning-powered Streamlit web application** that predicts the risk of heart disease based on patient health data. The project covers the full data science lifecycle from **EDA and preprocessing** to **model training, evaluation, and deployment**.

[🔗 Live Demo](https://heart-disease-prediction-greasha.streamlit.app/)

---

## 📌 Table of Contents

- [Overview](#overview)
- [Tech Stack](#tech-stack)
- [Dataset](#dataset)
- [Model Training](#model-training)
- [Streamlit App Features](#streamlit-app-features)
- [How to Run Locally](#how-to-run-locally)
- [Project Structure](#project-structure)
- [Results](#results)
- [Screenshots](#screenshots)
- [Author](#author)

---

## 📖 Overview

Cardiovascular disease is the leading cause of death globally. Early detection can save lives.

This project:
- Analyzes heart health data.
- Trains multiple classification models.
- Deploys the best-performing model (KNN) using **Streamlit**.
- Allows users to input personal data and get real-time risk predictions.

---

## ⚙️ Tech Stack

| Layer             | Tools / Libraries                            |
|------------------|-----------------------------------------------|
| Programming      | Python                                        |
| Data Handling    | Pandas, NumPy                                 |
| Visualization    | Matplotlib, Seaborn                           |
| ML Models        | Scikit-learn (KNN, SVM, Naive Bayes, etc.)    |
| Preprocessing    | One-Hot Encoding, StandardScaler              |
| Deployment       | Streamlit                                     |
| Model Persistence| Joblib                                        |

---

## 📂 Dataset

- 📁 **File**: `heart.csv`
- 👤 **Records**: 918 patients
- 📊 **Features**:
  - Age, Sex, Chest Pain Type
  - Resting Blood Pressure, Cholesterol, Fasting Blood Sugar
  - ECG Results, Max Heart Rate, Exercise-Induced Angina
  - Oldpeak (ST Depression), ST Slope

> Note: Zeros in `Cholesterol` and `RestingBP` were replaced with the column mean.

---

## 🔍 Model Training

Multiple classifiers were trained and evaluated:

| Model               | Accuracy | F1 Score |
|---------------------|----------|----------|
| Logistic Regression | 87.5%    | 0.8878   |
| ✅ K-Nearest Neighbors (KNN) | **88.6%** | **0.8986** |
| Naive Bayes         | 86.9%    | 0.8788   |
| Decision Tree       | 74.4%    | 0.7513   |
| SVM (RBF Kernel)    | 86.4%    | 0.8804   |

The best-performing model (**KNN**) was saved as `KNN_heart.pkl`.

---

## 🖥️ Streamlit App Features

- 📌 Clean UI for data entry (age, sex, cholesterol, etc.)
- 🧮 Real-time prediction using KNN model
- 📉 Displays results: `✅ Low Risk` or `⚠️ High Risk`
- 📦 Model and scaler loaded via `joblib`

---


git clone https://github.com/<your-username>/heart-stroke-prediction.git
cd heart-stroke-prediction
