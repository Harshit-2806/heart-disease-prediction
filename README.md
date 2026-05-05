# heart-disease-prediction
Heart Disease Prediction using ML + Streamlit
# 🫀 Heart Disease Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

> A machine learning pipeline that predicts whether a patient is at **high or low risk of heart disease**, based on clinical features — with an interactive Streamlit web app for real-time inference.

---

## 📸 App Screenshot

![App Screenshot](assets/app_screenshot.png)

---

## 📌 Project Overview

Cardiovascular disease is one of the leading causes of death globally. Early and accurate prediction can be life-saving. This project builds a complete ML pipeline — from raw data to a deployed web application — that classifies patients as at risk or not based on 11 clinical features.

**Key highlights:**
- Exploratory Data Analysis (EDA) on 918 patient records
- Preprocessing with one-hot encoding and StandardScaler normalization
- Trained and benchmarked 5 classification models
- Deployed as an interactive Streamlit app with real-time predictions

---

## 📊 Dataset

| Property | Details |
|---|---|
| **Source** | `heart.csv` |
| **Rows** | 918 |
| **Features** | 11 |
| **Target** | `HeartDisease` (0 = No Disease, 1 = Disease) |

### Feature Description

| Feature | Type | Description |
|---|---|---|
| `Age` | Numeric | Patient age in years |
| `Sex` | Categorical | M / F |
| `ChestPainType` | Categorical | ATA, NAP, TA, ASY |
| `RestingBP` | Numeric | Resting blood pressure (mm Hg) |
| `Cholesterol` | Numeric | Serum cholesterol (mg/dL) |
| `FastingBS` | Binary | Fasting blood sugar > 120 mg/dL (1 = True, 0 = False) |
| `RestingECG` | Categorical | Resting ECG results (Normal, ST, LVH) |
| `MaxHR` | Numeric | Maximum heart rate achieved |
| `ExerciseAngina` | Categorical | Exercise-induced angina (Y / N) |
| `Oldpeak` | Numeric | ST depression induced by exercise |
| `ST_Slope` | Categorical | Slope of peak exercise ST segment (Up, Flat, Down) |

---

## 🤖 Model Comparison

Five classification models were trained on an **80/20 train-test split** and evaluated by accuracy:

| Model | Accuracy |
|---|---|
| Logistic Regression | 86.41% |
| K-Nearest Neighbors (KNN) | 85.87% |
| Naive Bayes | 86.96% |
| Decision Tree | 79.89% |
| **SVM (RBF Kernel)** | **88.04% ✅ Best** |

> **Deployed model:** KNN (`knn_heart_model.pkl`) — chosen for its simplicity and solid generalization for real-time inference.

---

## 🛠️ Tech Stack

| Layer | Tools |
|---|---|
| Language | Python 3.8+ |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| ML Models | Scikit-Learn |
| Serialization | Joblib |
| Web App | Streamlit |

---

## 📁 File Structure
