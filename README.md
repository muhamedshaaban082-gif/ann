# Iris Flower Classification using ANN 🌸🧠

This project demonstrates how to build and evaluate an **Artificial Neural Network (ANN)** for **multi-class classification** using the famous **Iris dataset**.

The model classifies iris flowers into three species based on their physical measurements.

---

## 📌 Project Overview

- Problem Type: **Multi-Class Classification**
- Dataset: **Iris Dataset**
- Model Type: **Artificial Neural Network (ANN)**
- Classes:
  - Setosa
  - Versicolor
  - Virginica

---

## 🗂 Dataset Description

The Iris dataset contains **150 samples** with **4 numerical features**:

- Sepal length
- Sepal width
- Petal length
- Petal width

Target variable:
- `0` → Setosa  
- `1` → Versicolor  
- `2` → Virginica  

---

## ⚙️ Data Preprocessing

- Converted dataset to Pandas DataFrame
- Split data into training and testing sets (80% / 20%)
- No missing values
- Target labels used directly with **Sparse Categorical Crossentropy**

---

## 🧠 ANN Model Architecture

- Input Layer: 4 features
- Hidden Layer 1: 10 neurons (ReLU)
- Hidden Layer 2: 8 neurons (ReLU)
- Output Layer: 3 neurons (Softmax)

**Compilation Details:**
- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Metric: Accuracy

---

## 🏋️ Model Training

- Epochs: 15
- Batch Size: 10
- Validation Split: 20%
- Training and validation performance tracked

---

## 📊 Model Evaluation

- Accuracy evaluated on:
  - Training set
  - Test set
- Performance metrics:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report

---

## 📈 Training Visualization

- Training vs Validation Loss
- Training vs Validation Accuracy
- Helps detect overfitting and underfitting

---

## 💾 Model Saving & Loading

The trained ANN model is saved using Keras:

```python
model.save("model.h5")
