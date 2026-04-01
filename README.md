# Lithofacies Classification Using Machine Learning

## 📌 Project Overview

Subsurface lithofacies classification is a critical task in reservoir characterization and petroleum exploration. Traditionally, 

geologists interpret facies manually using well logs, which can be time-consuming and subjective.

This project applies machine learning techniques to automatically classify lithofacies based on petrophysical well log measurements.

The objective is to build a reliable multi-class classification model capable of predicting rock types from well log data

## 🎯 Problem Statement

Given continuous well log measurements such as:

- Gamma Ray (GR)

- Resistivity (ILD_log10)

- Porosity (PHIND)

- Neutron-Density Separation (DeltaPHI)

- Photoelectric Effect (PE)

- Other petrophysical indicators

Can we accurately predict the lithofacies class at each depth interval?

This is formulated as a **multi-class classification problem**.

## 📊 Dataset Description

The dataset contains:

- Multiple numerical well log features

- A categorical target variable (Facies)

- No missing values

- Imbalanced class distribution across 9 facies types

Each row represents a depth interval in a well.

## 🔎 Exploratory Data Analysis (EDA)

Key findings from EDA:

- Facies classes are imbalanced.

- Some logs show moderate correlation (e.g., resistivity and other petrophysical indicators).

- Significant overlap exists between facies, indicating that classification requires multivariate analysis.

- Individual logs alone cannot perfectly distinguish lithologies.

These insights justified the use of nonlinear machine learning models.

## ⚙️ Preprocessing Steps

- Log transformation applied to resistivity to reduce skewness.

- Categorical identifiers removed to prevent data leakage.

- Dataset split into training and testing sets (stratified).

- Feature scaling applied where necessary.

- Clean and structured ML-ready dataset generated.

## 🤖 Modeling Approach

Two models were trained:

### 1️⃣ Logistic Regression (Baseline)

Accuracy ≈ 60%

Struggled due to nonlinear facies boundaries

### 2️⃣ Random Forest Classifier

- Accuracy ≈ 78%

- Strong performance across most facies

- Effectively captured nonlinear petrophysical relationships

**Random Forest significantly outperformed the linear baseline**.

## 📈 Feature Importance Analysis

Feature importance revealed that:

- Resistivity (ILD_log10) strongly influences lithology prediction.

- Porosity (PHIND) plays a key role in reservoir identification.

- Gamma Ray (GR) effectively distinguishes shale from cleaner formations.

- Multivariate interactions between logs drive classification performance.

The model learned physically meaningful geological patterns.

## Geological Interpretation

The trained model successfully captured realistic subsurface rules such as:

- High GR + Low Resistivity → Shale

- Low GR + High Resistivity + High Porosity → Clean Reservoir Rock

- Intermediate log responses → Transitional Facies

This confirms the model predictions are grounded in rock physics principles rather than random statistical patterns.

## 📌 Results Summary

- Multi-class facies classification (9 classes)

- ~78% accuracy on unseen test data

- Robust performance using tree-based learning

- Meaningful geological feature ranking

The results demonstrate that machine learning can assist in automated subsurface interpretation and reservoir characterization.

## 🚀 Future Improvements

- Hyperparameter tuning

- Cross-validation across wells

- Class imbalance handling (SMOTE or class weighting)

- SHAP-based model explainability

- Deployment as a prediction API

## 🧠 Key Skills Demonstrated

- Exploratory Data Analysis

- Feature Engineering

- Multiclass Classification

- Model Evaluation

- Feature Importance Interpretation

- Applied Geoscience + Machine Learning Integration

# 💼 Author

Joseph Solomon Aldu
Entry-Level Data Scientist | Machine Learning Engineer
Focused on applying ML to geoscience and real-world industrial problems.

