# 🪨 Well Log Lithofacies Classification using Machine Learning

## 📌 Project Overview

Lithofacies classification is an important task in petroleum geoscience, helping geoscientists characterize subsurface formations and improve geological interpretation. Traditionally, facies identification relies on expert analysis of well logs and core data, which can be time-consuming and subjective.

This project applies Machine Learning to automate lithofacies classification using well log data. An XGBoost classifier was developed to predict nine lithofacies classes from petrophysical well logs. To improve model transparency and interpretability, SHAP (SHapley Additive Explanations) was used to identify the most influential features driving model predictions.

---

## 🎯 Project Objectives

* Develop a machine learning model for lithofacies classification.
* Explore relationships between well log measurements and lithofacies.
* Evaluate model performance using classification metrics.
* Apply Explainable AI (XAI) techniques to interpret model predictions.
* Demonstrate the application of machine learning in petroleum geoscience workflows.

---

## 📊 Dataset Description

The dataset contains petrophysical well log measurements used as predictor variables.

### Features

| Feature   | Description                   |
| --------- | ----------------------------- |
| GR        | Gamma Ray                     |
| ILD_log10 | Deep Resistivity (Log Scale)  |
| DeltaPHI  | Porosity Difference           |
| PHIND     | Average Porosity Indicator    |
| PE        | Photoelectric Effect          |
| NM_M      | Non-Marine / Marine Indicator |
| RELPOS    | Relative Position             |

### Target Variable

The model predicts nine lithofacies classes:

| Facies Code | Lithofacies                |
| ----------- | -------------------------- |
| 1           | Sandstone                  |
| 2           | Coarse Siltstone           |
| 3           | Fine Siltstone             |
| 4           | Marine Siltstone and Shale |
| 5           | Mudstone                   |
| 6           | Wackestone                 |
| 7           | Dolomite                   |
| 8           | Packstone-Grainstone       |
| 9           | Phylloid-Algal Bafflestone |

---

## 🔍 Project Workflow

### 1. Problem Definition

* Defined project objectives and geological significance.
* Identified lithofacies classification as a multiclass classification problem.

### 2. Data Understanding

* Explored dataset structure.
* Examined feature descriptions and data quality.

### 3. Exploratory Data Analysis (EDA)

* Statistical summaries.
* Feature distributions.
* Correlation analysis.
* Class distribution analysis.

### 4. Data Preprocessing

* Missing value handling.
* Feature preparation.
* Data scaling and transformation.
* Train-test splitting.

### 5. Model Development

* XGBoost classifier training.
* Hyperparameter selection.
* Model evaluation.

### 6. Explainable AI (SHAP)

* SHAP Summary Plot.
* SHAP Feature Importance Analysis.
* Model interpretability assessment.

---

## 🤖 Machine Learning Model

### XGBoost Classifier

XGBoost was selected because it:

* Handles structured tabular data effectively.
* Provides strong predictive performance.
* Supports multiclass classification.
* Offers feature importance insights.
* Is robust against overfitting.

---

## 📈 Results

### Model Performance

* Accuracy: **81.14%**

### Key Findings

* The model successfully classified nine lithofacies classes.
* SHAP analysis revealed the most influential features driving predictions.
* Explainable AI improved understanding of model behavior.
* Results demonstrate the potential of machine learning for automated lithofacies interpretation.

---

## 🔬 Explainable AI with SHAP

SHAP (SHapley Additive exPlanations) was used to improve model transparency and interpretability.

### Purpose of SHAP

* Explain model predictions.
* Identify important features.
* Understand feature contributions.
* Improve trust in machine learning results.

### Key Observations

The most influential features included:

* NM_M
* GR (Gamma Ray)
* RELPOS

These variables played significant roles in distinguishing lithofacies classes.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* XGBoost
* SHAP
* Matplotlib
* Seaborn
* Jupyter Notebook
* Google Colab
* Git
* GitHub

---

## 📁 Repository Structure

```text
well-log-lithofacies-classification/
│
├── Notebook_1_Problem_and_Objectives.ipynb
├── Notebook_2_Data_Understanding.ipynb
├── Notebook_3_EDA.ipynb
├── Notebook_4_Preprocessing.ipynb
├── Notebook_5_Modeling_and_Evaluation.ipynb
│
├── README.md
└── requirements.txt
```

---

## 🌍 Applications

This project demonstrates the application of machine learning in:

* Lithofacies Classification
* Well Log Interpretation
* Geological Data Analytics
* Petroleum Geoscience
* Explainable Artificial Intelligence
* Subsurface Characterization

---

## 🚀 Future Improvements

Potential future enhancements include:

* Hyperparameter optimization.
* Deep learning approaches.
* Ensemble modeling techniques.
* Cross-validation studies.
* Integration of additional well log features.
* Uncertainty quantification.

---

## 👨‍💻 Author

**Joseph Solomon Aldu**

Geology Graduate | Petroleum Geoscience & Machine Learning Enthusiast

### Areas of Interest

* Petroleum Geoscience
* Machine Learning
* Explainable AI (XAI)
* Well Log Analytics
* Geological Data Science
* Subsurface Characterization

GitHub: https://github.com/josephsolomonaldu-create

---

## 📜 License

This project is intended for educational, research, and portfolio purposes.
