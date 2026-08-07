# heart_failure_classification
# 🫀 Heart Failure Survival Prediction | End-to-End ML Pipeline

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 📌 Overview
Cardiovascular diseases (CVDs) are the number 1 cause of death globally. This repository contains an **End-to-End Machine Learning Pipeline** designed to predict mortality caused by heart failure using clinical record features.

The project follows a structured 18-step ML workflow—starting from data quality checks and Exploratory Data Analysis (EDA) to feature scaling, model comparison, and hyperparameter tuning.

---

## 🚀 Key Features & Workflow
- **Data Quality & Integrity Checks**: Audited missing values, duplicate entries, and invalid negative numerical records.
- **Exploratory Data Analysis (EDA)**: Visualized feature distributions, correlations, and target class balance.
- **Data Preprocessing & Scaling**: Applied `StandardScaler` to distance/gradient-sensitive features post-train-test split to prevent data leakage.
- **Model Benchmark**: Trained and evaluated 5 classification algorithms:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - Support Vector Machine (SVM)
  - K-Nearest Neighbors (KNN)
- **Model Tuning**: Utilized `GridSearchCV` on the top-performing model to optimize hyperparameters based on **F1-Score**.

---

## 📊 Dataset Information
The dataset consists of **299 patient records** with **13 clinical features**:

| Feature | Description | Unit |
| :--- | :--- | :--- |
| `age` | Patient's age | Years |
| `ejection_fraction` | Percentage of blood leaving the heart per contraction | % |
| `serum_creatinine` | Level of serum creatinine in the blood | mg/dL |
| `serum_sodium` | Level of serum sodium in the blood | mEq/L |
| `time` | Follow-up period | Days |
| `DEATH_EVENT` | **(Target)** If the patient died during the follow-up period | 0 = No, 1 = Yes |

---

## 🏆 Model Performance Comparison

> **Note:** In medical diagnostics, **Recall** and **F1-Score** are prioritized over raw accuracy to minimize False Negatives.

| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Random Forest (Tuned)** | **0.88** | **0.85** | **0.82** | **0.83** |
| Logistic Regression | 0.83 | 0.80 | 0.75 | 0.77 |
| Support Vector Machine | 0.82 | 0.78 | 0.74 | 0.76 |
| K-Nearest Neighbors | 0.78 | 0.72 | 0.70 | 0.71 |
| Decision Tree | 0.75 | 0.68 | 0.68 | 0.68 |

---

## 🛠️ Tech Stack & Tools
- **Language:** Python
- **Data Handling:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-Learn
- **Environment:** Jupyter Notebook / VS Code

---

## 💻 How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/heart-failure-prediction.git](https://github.com/your-username/heart-failure-prediction.git)
   cd heart-failure-prediction
