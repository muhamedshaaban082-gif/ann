# Loan Approval Prediction System 💳📊

This project focuses on building and evaluating machine learning models to predict **loan approval status** based on customer personal, financial, and credit-related information.

The goal is to compare multiple models, apply feature engineering, and improve performance using ensemble learning techniques.

---

## 📌 Project Overview

- Problem Type: **Binary Classification**
- Target Variable: `loan_status`
- Objective: Predict whether a loan will be **approved or rejected**

---

## 🗂 Dataset

- Source: Loan dataset (CSV file)
- Includes:
  - Personal data (age, gender, education)
  - Financial data (income, loan amount, interest rate)
  - Credit history and credit score
  - Loan intent and previous defaults

---

## ⚙️ Data Preprocessing

- Handling missing values and duplicates
- Exploratory Data Analysis (EDA)
- Encoding categorical variables:
  - One-Hot Encoding
  - Ordinal Encoding for education level
- Feature scaling using **RobustScaler**
- Feature Engineering:
  - Income per experience
  - Loan-to-income ratio
  - Credit history ratios

---

## 🔍 Exploratory Data Analysis (EDA)

- Count plots for categorical features
- Histograms and boxplots for numerical features
- Crosstab analysis with loan status
- Correlation heatmap
- Mutual Information for feature importance

---

## 🤖 Models Implemented

- Logistic Regression
- Support Vector Classifier (SVC)
- XGBoost Classifier
- Ensemble Models:
  - Stacking Classifier
  - Voting concepts
- Oversampling Technique:
  - SMOTE (to handle class imbalance)

---

## 🧪 Model Evaluation

- Train/Test Split with stratification
- Cross-Validation using StratifiedKFold
- Metrics:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix
- Hyperparameter Tuning:
  - GridSearchCV
  - RandomizedSearchCV

---

## 🏆 Best Performing Model

- Tuned **XGBoost Classifier**
- Stacking ensemble combining:
  - Logistic Regression
  - SVC
  - XGBoost

---

## 💾 Model Saving

The trained Logistic Regression model is saved using Pickle:

```python
modellogreg.pkl
