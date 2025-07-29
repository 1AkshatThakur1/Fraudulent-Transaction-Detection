# 🚀 Proactive Fraud Detection Project

A powerful and scalable machine learning framework for real-time fraud detection on financial transactions using Python and Google Colab.  

![Status-Complete](https://img.shields.io/badge/Status-Complete-brightgreen) ![Python-3.8+](https://img.shields.io/badge/Python-3.8%2B-blue) ![Colab](https://img.shields.io/badge/Google-Colab-F9AB00)

---

## 📊 Project Overview

This project delivers an end-to-end, production-ready workflow for detecting financial fraud:
- Cleans and analyzes >6M transactions
- Rapidly surfaces fraud using tree-based ML
- Identifies key risk factors and interprets model logic
- Provides actionable infrastructure recommendations and anti-fraud monitoring

---

## 📝 Dataset

We use the company's large financial transactions dataset:

- **`Fraud.csv`** (6M+ rows, 10 columns)  
  - Each row: a customer transaction with amount, type, balances, and fraud flag.

---

## 🎯 Key Steps & Modules

### 1. Environment Setup & Data Access  
- Install packages (`lightgbm`, `imblearn`, `shap`, etc.)
- Mount Google Drive and load CSV data

### 2. Data Cleaning & Parsing  
- Remove negative/invalid amounts, fill missing values, cap outliers
- Drop highly collinear features (using VIF)

### 3. Feature Engineering  
- Encode transaction type, create time/hour/weekend flags, balance movements, and alias similarity

### 4. Variable Selection  
- Use recursive feature elimination (RFE) with LightGBM and VIF

### 5. Modeling Pipeline  
- SMOTETomek for class balancing
- LightGBM classifier (`class_weight`, 800 estimators, 0.05 LR)
- Stratified train/test split and PR-AUC metric

### 6. Performance Analysis  
- High recall/precision achieved (Recall ≈90%, Precision ≈80%, PR-AUC ≈0.96)
- Visualize confusion matrix, PR/ROC curves, calibration curve, SHAP plots

### 7. Fraud Insights & Interpretation  
- Top predictors: amount, transaction type, time, weekend, origin-destination alias
- Factors validated against real-world fraud patterns

### 8. Prevention & Monitoring  
- Real-time scoring API, adaptive limits, step-up authentication, graph analytics, audit logs, canary deployment
- Post-deployment: monitor fraud capture, false positives, user friction, and model drift; validate with A/B tests

---

## ⚡ Quick Start (Colab)
# 🚀 Proactive Fraud Detection Project

A powerful and scalable machine learning framework for real-time fraud detection on financial transactions using Python and Google Colab.  
**Final Project Submission — Data Science**

![Status-Complete](https://img.shields.io/badge/Status-Complete-brightgreen) ![Python-3.8+](https://img.shields.io/badge/Python-3.8%2B-blue) ![Colab](https://img.shields.io/badge/Google-Colab-F9AB00)

---

## 📊 Project Overview

This project delivers an end-to-end, production-ready workflow for detecting financial fraud:
- Cleans and analyzes >6M transactions
- Rapidly surfaces fraud using tree-based ML
- Identifies key risk factors and interprets model logic
- Provides actionable infrastructure recommendations and anti-fraud monitoring

---

## 📝 Dataset

We use the company's large financial transactions dataset:

- **`Fraud.csv`** (6M+ rows, 10 columns)  
  - Each row: a customer transaction with amount, type, balances, and fraud flag.

---

## 🎯 Key Steps & Modules

### 1. Environment Setup & Data Access  
- Install packages (`lightgbm`, `imblearn`, `shap`, etc.)
- Mount Google Drive and load CSV data

### 2. Data Cleaning & Parsing  
- Remove negative/invalid amounts, fill missing values, cap outliers
- Drop highly collinear features (using VIF)

### 3. Feature Engineering  
- Encode transaction type, create time/hour/weekend flags, balance movements, and alias similarity

### 4. Variable Selection  
- Use recursive feature elimination (RFE) with LightGBM and VIF

### 5. Modeling Pipeline  
- SMOTETomek for class balancing
- LightGBM classifier (`class_weight`, 800 estimators, 0.05 LR)
- Stratified train/test split and PR-AUC metric

### 6. Performance Analysis  
- High recall/precision achieved (Recall ≈90%, Precision ≈80%, PR-AUC ≈0.96)
- Visualize confusion matrix, PR/ROC curves, calibration curve, SHAP plots

### 7. Fraud Insights & Interpretation  
- Top predictors: amount, transaction type, time, weekend, origin-destination alias
- Factors validated against real-world fraud patterns

### 8. Prevention & Monitoring  
- Real-time scoring API, adaptive limits, step-up authentication, graph analytics, audit logs, canary deployment
- Post-deployment: monitor fraud capture, false positives, user friction, and model drift; validate with A/B tests

---

## ⚡ Quick Start (Colab)

1. Click the **Open In Colab** badge  
2. Update `DATA_DIR` to your Google Drive folder path  
3. Run all cells sequentially (Runtime → Run all)  
4. Explore interactive tables, charts, and machine learning results  


