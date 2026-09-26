# Breast Cancer Classification using Logistic Regression

A machine learning classification project using **Logistic Regression** to classify breast cancer tumors as **Malignant (M)** or **Benign (B)**.

## 📌 Project Overview

This project demonstrates the complete workflow of a binary classification problem:

* Data cleaning
* Feature and target separation
* Train-test splitting
* Feature scaling
* Logistic Regression
* Model evaluation
* Confusion Matrix
* Precision, Recall and F1 Score
* ROC-AUC
* Dummy Classifier baseline
* ROC Curve visualization

The goal is to understand how Logistic Regression performs on the Breast Cancer dataset and compare it against a simple baseline model.

---

## 📂 Dataset

The project uses the **Breast Cancer Wisconsin Diagnostic Dataset**.

The dataset contains numerical measurements computed from breast cell nuclei images.

### Target

The target column is:

`diagnosis`

It contains two classes:

* `M` → Malignant → `1`
* `B` → Benign → `0`

### Features

The dataset contains numerical features related to properties such as:

* Radius
* Texture
* Perimeter
* Area
* Smoothness
* Compactness
* Concavity
* Concave points
* Symmetry
* Fractal dimension

Each measurement has corresponding mean, standard error, and worst-value features.

---

## 🧹 Data Preprocessing

Two unnecessary columns were removed:

```python
df = df.drop(["Unnamed: 32", "id"], axis=1)
```

### Why?

* `Unnamed: 32` contained no useful information.
* `id` is only an identifier a
