# 🪨 Well Log Lithofacies Classification using Machine Learning

[

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)

](https://www.python.org/)
[

![XGBoost](https://img.shields.io/badge/XGBoost-81.14%25_Accuracy-green.svg)

](https://xgboost.readthedocs.io/)
[

![SHAP](https://img.shields.io/badge/Explainability-SHAP-orange.svg)

](https://shap.readthedocs.io/)
[

![Dataset](https://img.shields.io/badge/Dataset-SEG_2016-red.svg)

](https://github.com/seg/2016-ml-contest)
[

![License](https://img.shields.io/badge/License-MIT-yellow.svg)

](LICENSE)

> **Automated lithofacies prediction from wireline well log data using XGBoost, with SHAP explainability and prediction confidence analysis.**

---

## 📌 Project Overview

This project presents an end-to-end machine learning pipeline that:

- 🎯 Classifies **9 lithofacies classes** from wireline well log data
- 📊 Achieves **81.14% accuracy** using XGBoost on the SEG 2016 dataset
- 🔍 Applies **SHAP** to explain predictions geologically
- 📈 Quantifies **prediction confidence** for operational deployment
- ✅ Structured across **5 professional notebooks**
## 🗂️ Project Structure

well-log-lithofacies-classification/
│
├── 01_Problem_and_Objectives.ipynb
├── 02_Data_Understanding.ipynb
├── 03_EDA.ipynb
├── 04_Preprocessing.ipynb
├── 05_Modeling_and_Evaluation.ipynb
│
├── data/
│   ├── facies_data.csv
│   ├── X_train.csv
│   ├── X_test.csv
│   ├── y_train.csv
│   └── y_test.csv
│
├── models/
│   └── scaler.pkl
│
└── README.md

---

## 📊 Dataset & Results

| Property | Value |
|---|---|
| Total Samples | 3,232 |
| Training Samples | 2,585 (80%) |
| Test Samples | 647 (20%) |
| Classes | 9 Lithofacies |
| Missing Values | None |

| Model | Accuracy | Macro F1 |
|---|---|---|
| Logistic Regression | 59.97% | 0.58 |
| Random Forest | 78.05% | 0.80 |
| **XGBoost** | **81.14%** | **0.82** |
## 🔍 SHAP Feature Importance

| Rank | Feature | Mean |SHAP| | Geological Meaning |
|---|---|---|---|
| 1 | NM_M | 1.75 | Depositional environment |
| 2 | GR | 1.50 | Lithology discriminator |
| 3 | RELPOS | 1.25 | Stratigraphic position |
| 4 | PE | 0.50 | Mineralogy indicator |
| 5 | DeltaPHI | 0.45 | Gas effect |
| 6 | ILD_log10 | 0.40 | Fluid identification |
| 7 | PHIND | 0.35 | Porosity index |
| 8 | Depth | 0.25 | Depth proxy |

## ⚙️ Quick Start

```bash
git clone https://github.com/josephsolomonaldu-create/well-log-lithofacies-classification.git
cd well-log-lithofacies-classification
pip install -r requirements.txt
