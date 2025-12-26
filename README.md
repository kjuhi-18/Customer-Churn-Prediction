# 📊 Customer Churn Prediction 🔍  
🚀 *End-to-End Machine Learning Project*

![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)
![ML](https://img.shields.io/badge/Machine%20Learning-Supervised-green)
![XGBoost](https://img.shields.io/badge/Model-XGBoost-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

> Predict whether a bank customer will **churn or stay** using **EDA, imbalance handling, and advanced ML models**.

---

## 🚀 Project Overview 🧠

Customer churn is a major challenge for banks and subscription-based services.  
This project builds a **realistic and deployable churn prediction system** that:

- ✅ Performs in-depth **Exploratory Data Analysis (EDA)**
- ✅ Handles **imbalanced data**
- ✅ Compares multiple ML models
- ✅ Avoids **data leakage**
- ✅ Predicts churn from **user-provided input**

---

## 🧾 Dataset Overview 📂

The dataset includes customer **demographic, financial, and behavioral** information:

- Credit Score, Age, Balance, Estimated Salary  
- Number of Products, Activity Status  
- Geography, Gender, Card Type  
- Complaint, Satisfaction Score, Loyalty Points  

🎯 **Target Variable:** `Exited`  
- `0` → Customer stays  
- `1` → Customer churns  

---

## 🔍 Exploratory Data Analysis (EDA) – Key Insights 📊

### ⚖️ Class Imbalance
- Majority of customers **do not churn**
- Accuracy alone is misleading → recall & ROC-AUC prioritized

### 🚨 Complaint vs Churn (Data Leakage)
- Almost all customers who complained **eventually churned**
- `Complain` showed near-perfect correlation with `Exited`

✔ Models trained **with and without `Complain`**

### 👴 Age vs Churn
- Churned customers are **older on average**
- Age is a strong churn predictor

### 💰 Balance vs Churn
- Higher-balance customers tend to churn more

### 💳 Credit Score
- Significant overlap → limited influence

---

## 🧠 Machine Learning Models Used 🤖

### 🔹 Logistic Regression
- Baseline model
- Trained with & without `Complain`

### 🌲 Random Forest
- Accuracy: **85%**
- ROC-AUC: **0.87**

### ⚡ XGBoost (Final Model ⭐)
- Accuracy: **84%**
- Churn Recall: **71%**
- ROC-AUC: **0.88**

---

## 📁 Repository Structure 🗂️

```
customer-churn-prediction/
│
├── data/
│ └── Customer-Churn-Records.csv
│
├── notebooks/
│ ├── CustomerChurnPrediction.ipynb
│ └── UserBasedInput.ipynb
│
├── model/
│ ├── model.pkl
│ └── scaler.pkl
│
├── README.md
└── requirements.txt
```

---

## 🎯 Final Conclusion 🏁

A complete, leakage-free churn prediction system using **XGBoost**, capable of proactive customer retention.

---

## 🙌 Author ✨

**Kunal Jhindal**  

