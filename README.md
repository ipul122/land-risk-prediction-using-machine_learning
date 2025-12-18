# Land Risk Prediction Using Machine Learning

## Overview
This project focuses on **landslide risk prediction** using supervised machine learning techniques. It was developed as part of an academic assignment to demonstrate the application of data preprocessing, imbalance handling, model training, hyperparameter tuning, and evaluation in a real-world environmental risk scenario.

The system predicts the **level of landslide risk** based on several environmental and geographical factors using ensemble-based machine learning models.

---

## Objectives
The objectives of this project are:
1. To analyze environmental factors influencing landslide risk.
2. To handle imbalanced classification problems using resampling techniques.
3. To develop and compare machine learning models for multi-class classification.
4. To evaluate model performance using appropriate metrics.
5. To demonstrate a complete and reproducible machine learning pipeline.

---

## Dataset
The dataset contains **5,000 records** with the following features:

| Feature | Description |
|------|-----------|
| Temperature (°C) | Ambient temperature |
| Humidity (%) | Relative humidity |
| Precipitation (mm) | Rainfall amount |
| Soil Moisture (%) | Soil water content |
| Elevation (m) | Terrain elevation |
| Landslide Risk Prediction | Target variable (categorical) |

The dataset is clean, with no missing values or duplicates, but exhibits significant **class imbalance**, which is addressed during preprocessing.

---

## Methodology

### 1. Data Preprocessing
- Exploratory Data Analysis (EDA)
- Label encoding for categorical target variable
- Feature scaling using **StandardScaler**
- Handling class imbalance using **SMOTE (Synthetic Minority Oversampling Technique)**

### 2. Data Splitting
The dataset is divided into:
- **Training set (75%)**
- **Testing set (15%)**
- **Prediction / Hold-out set (10%)**

This separation ensures proper evaluation and independent inference testing.

---

## Machine Learning Models

### 1. XGBoost Classifier
- Gradient boosting-based ensemble model
- Hyperparameter tuning using **GridSearchCV**
- Evaluation metric: **F1-score (macro)** to address class imbalance

### 2. Random Forest Classifier
- Bagging-based ensemble model
- Balanced class weighting
- Hyperparameter optimization using **GridSearchCV**

Both models achieve high classification performance on the test dataset.

---

## Model Evaluation
The models are evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Feature importance analysis is also conducted to understand the contribution of each input variable.

---
