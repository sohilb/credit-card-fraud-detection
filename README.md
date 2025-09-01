# 🕵️‍♂️ Credit Card Fraud Detection

This project focuses on building and evaluating machine learning models for **credit card fraud detection**.  
Fraud detection is a highly imbalanced classification problem where fraudulent transactions are very rare compared to normal ones.  

---

## 📌 Project Overview

- Exploratory Data Analysis (EDA) to understand the distribution of fraudulent vs. non-fraudulent transactions.  
- Handling **class imbalance** using techniques such as **SMOTE**, **ADASYN**, **Oversampling**, and **Undersampling**.  
- Training and evaluating multiple machine learning models including:  
  - Logistic Regression  
  - Decision Tree  
  - Random Forest  
  - XGBoost  
- Comparison of models based on **ROC-AUC**, **Precision**, **Recall**, and **F1-Score**.  
- Business-driven recommendations based on cost-benefit analysis.  

---

## ⚖️ Handling Class Imbalance

- **Resampling Techniques**: Undersampling, Oversampling, SMOTE, ADASYN  
- **Why Undersampling is not preferred**: It leads to information loss, poor generalization, and higher risk of overfitting with small datasets.  

---

## 📊 Model Evaluation

- Logistic Regression and XGBoost performed best in terms of **ROC-AUC**.  
- **XGBoost** achieved ROC scores of:  
  - **0.99** on train data  
  - **0.97** on test data  
- With SMOTE, **Logistic Regression** showed strong **Recall**, making it well-suited for detecting fraudulent transactions while being simple and explainable.  

---

## 💰 Cost-Benefit Analysis

- Complex models (Random Forest, SVM, XGBoost) → Higher performance but expensive in terms of computation and deployment.  
- Simple models (Logistic Regression) → Lower cost, faster training, easier explainability.  
- Business decision: Depends on transaction value and tolerance for **false positives vs. false negatives**.  

---

## 🏦 Business Recommendations

- For **small-value transactions** → Prioritize **Precision** to reduce false alarms.  
- For **large-value transactions** → Prioritize **Recall** to minimize the risk of missing fraud.  
- Final choice: **Logistic Regression with SMOTE** balances accuracy, recall, and explainability.  

---

## ⚙️ Tech Stack

- **Python**  
- **Jupyter Notebook**  
- **Libraries**: pandas, numpy, scikit-learn, imbalanced-learn, xgboost, matplotlib, seaborn  

---

## 🚀 How to Run

1. Clone this repository  
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
