# Customer Churn Prediction

Predicting telecom customer churn using machine learning — built as part of the AI/ML Internship at Naviotech Solution Pvt. Ltd. (June 2026).

## 📌 Overview

This project analyzes 7,043 telecom customer records to predict which customers are likely to churn (cancel their service), using a Random Forest classifier tuned and regularized for reliable, generalizable performance.

## 📊 Dataset

- **Source:** Telco Customer Churn dataset
- **Size:** 7,043 rows, 21 features
- **Target:** `Churn` (Yes/No) — 26.5% churn rate (imbalanced)

## 🛠️ Approach

1. **Data Preprocessing** — cleaned missing values, encoded categorical features, split into train/test sets
2. **Class Imbalance Handling** — compared SMOTE (oversampling) vs. Random Undersampling
3. **Model Selection** — compared Decision Tree, Random Forest, and XGBoost using Stratified K-Fold Cross Validation
4. **Hyperparameter Tuning** — used GridSearchCV to tune the best model (Random Forest)
5. **Overfitting Analysis** — detected a 22% train/test accuracy gap after tuning, and fixed it through regularization (reduced to 8%)

## 📈 Results

| Metric | Score |
|---|---|
| Test Accuracy | 77.5% |
| Churn Recall | 74% |
| Churn Precision | 56% |
| Churn F1-Score | 64% |

## 📁 Repository Contents

| File | Description |
|---|---|
| `Customer_Churn_Prediction_using_ML.ipynb` | Full Jupyter notebook — data cleaning, EDA, modeling, tuning |
| `WA_Fn-UseC_-Telco-Customer-Churn.csv` | Dataset used for training and evaluation |
| `Customer_Churn_Prediction_Report.docx` | Detailed project report |
| `Customer_Churn_Prediction.pptx` | Presentation summary (10 slides) |

## 🧰 Tech Stack

Python · pandas · scikit-learn · imbalanced-learn (SMOTE) · XGBoost · matplotlib · seaborn

## 🚀 Future Scope

- Try additional models (LightGBM, CatBoost)
- Deploy as a web app for real-time predictions
- Add SHAP-based explainability

## 👤 Author

**Arya** — B.Tech CSE (Data Science), Gandhi Engineering College, Bhubaneswar
AI/ML Intern, Naviotech Solution Pvt. Ltd.
