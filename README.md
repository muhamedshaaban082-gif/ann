# Loan Approval Prediction using ANN 🧠💳

This project implements an **Artificial Neural Network (ANN)** to predict **loan approval status** based on customer demographic, financial, and credit information.

The model is built to learn complex non-linear relationships within the data and improve prediction accuracy compared to traditional machine learning models.

---

## 📌 Project Overview

- Problem Type: **Binary Classification**
- Target Variable: `loan_status`
- Model Type: **Artificial Neural Network (ANN)**
- Objective: Predict whether a loan will be **Approved or Rejected**

---

## 🗂 Dataset

- Format: CSV
- Contains:
  - Personal information (age, gender, education)
  - Financial details (income, loan amount, interest rate)
  - Credit history and credit score
  - Loan intent and previous default history

---

## ⚙️ Data Preprocessing

- Data cleaning (missing values & duplicates)
- Encoding categorical features:
  - One-Hot Encoding
  - Ordinal encoding for education level
- Feature scaling using **RobustScaler**
- Feature engineering:
  - Loan to income ratio
  - Income per experience
  - Credit history ratios
- Train/Test split with stratification

---

## 🧠 ANN Model Architecture

- Input Layer: Features from processed dataset
- Hidden Layers:
  - Fully connected (Dense) layers
  - Activation function: **ReLU**
- Output Layer:
  - Sigmoid activation (Binary Classification)
- Loss Function: **Binary Crossentropy**
- Optimizer: **Adam**

---

## 🧪 Model Training & Evaluation

- Metrics used:
  - Accuracy
  - Precision
  - Recall
  - F1-score
- Confusion Matrix for performance visualization
- Evaluation performed on unseen test data

---

## 📈 Results

- ANN achieved strong performance in capturing complex patterns
- Demonstrated better generalization compared to baseline models
- Suitable for real-world loan approval prediction tasks

---

## 📁 Project Structure

