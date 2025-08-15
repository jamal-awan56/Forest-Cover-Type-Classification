# 🌲 Forest Cover Type Classification

This project predicts the forest cover type from cartographic variables such as elevation, slope, soil type, and wilderness area.  
It uses machine learning models to classify forest cover into one of seven types based on data from the UCI Covertype dataset.

## 📌 Overview
- Goal: Build an accurate model to classify forest cover type from environmental features.
- Dataset: UCI Covertype (~581k rows, 54 features, 7 cover types).
- Approach: Data preprocessing, EDA, model training, and explainability using SHAP.
- Best Model: XGBoost classifier with high accuracy.

---

## 📂 Dataset
- Source: [UCI Machine Learning Repository - Covertype Dataset](https://archive.ics.uci.edu/ml/datasets/covertype)
- Target Variable: `Cover_Type` (values 1–7)
- Features: Elevation, Aspect, Slope, Horizontal/Vertical Distances, Soil Type, Wilderness Area, etc.

---

## 🛠️ Technologies Used
- Languages: Python
- Libraries: 
  - Data: `pandas`, `numpy`
  - Visualization: `matplotlib`, `seaborn`
  - Machine Learning: `scikit-learn`, `xgboost`
  - Explainability: `shap`
  - Utilities: `joblib`

---

## 🚀 Project Workflow
1. Imports & Constants – Load libraries and set parameters.
2. Data Loading – Download and read dataset into DataFrame.
3. Data Inspection – Check structure, types, and missing values.
4. Exploratory Data Analysis (EDA) – Visualize class distribution, correlations, and feature impacts.
5. Preprocessing – Train-test split, scaling, and encoding.
6. Model Training – Compare Logistic Regression, Random Forest, and XGBoost.
7. Evaluation – Accuracy, Precision, Recall, F1-score.
8. Explainability – SHAP analysis to understand feature importance.

---

## 📊 Results
- Best model: XGBoost
- Top features: Elevation, Soil Type, Horizontal Distance to Hydrology
- Key insight: Elevation and soil type have the strongest influence on forest cover classification.
