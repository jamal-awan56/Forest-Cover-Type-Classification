# Forest Cover Type Classification

This project predicts the forest cover type (categorical class) from cartographic variables such as elevation, aspect, slope, soil type, and wilderness area.
It uses machine learning techniques to classify forest types based on the UCI Machine Learning dataset provided by the US Forest Service.

# Project Overview

The aim is to build an accurate classifier that can predict forest cover type from environmental features. This project includes:

Data loading & exploration

Data preprocessing

Exploratory Data Analysis (EDA) with visualizations

Model training and evaluation using different algorithms

Explainability using SHAP

Dataset

Source: UCI Machine Learning Repository - Covertype Dataset

Size: ~581,000 instances, 54 features

Target: Cover_Type (1–7, representing forest categories)

Features: Elevation, Aspect, Slope, Horizontal/Vertical Distances, Soil Type, Wilderness Area, etc.

Technologies & Libraries Used

Python

Pandas, NumPy – Data manipulation

Matplotlib, Seaborn – Visualization

scikit-learn – Machine learning models, preprocessing, evaluation

XGBoost – Gradient boosting classifier

SHAP – Model explainability

Joblib – Model saving/loading

Project Workflow
Step 1 — Imports and Constants

Load required libraries and define dataset paths/constants.

Step 2 — Download & Load Dataset

Download compressed dataset (.gz format)

Load it into a Pandas DataFrame with column names

Step 3 — Quick Inspection & Cleaning

Check data types, missing values, and class distribution

Handle missing values if present

Step 4 — Exploratory Data Analysis (EDA)

Class distribution plot

Feature histograms

Correlation analysis

Visual inspection of elevation, slope, and soil type impacts

Step 5 — Preprocessing

Train-test split

Optional scaling/normalization

One-hot encoding for categorical variables

Step 6 — Model Training & Evaluation

Train multiple classifiers (Logistic Regression, Random Forest, XGBoost)

Evaluate using Accuracy, Precision, Recall, F1-score

Compare models

Step 7 — Explainability

Use SHAP values to explain feature contributions

Visualize important features for each class

How to Run
1. Clone the repository
git clone https://github.com/<your-username>/forest-cover-classification.git
cd forest-cover-classification

2. Install dependencies
pip install -r requirements.txt


Or in Google Colab:

!pip install xgboost joblib shap

3. Run the notebook

Open in Jupyter Notebook or Google Colab:

jupyter notebook Forest_Cover_Type_Classification.ipynb

Results

Best performing model: XGBoost with high accuracy and interpretability using SHAP

Key influencing features: Elevation, Soil Type, Horizontal Distance to Hydrology

Author

Malik Jamal Mehboob

GitHub: jamal-awan56

LinkedIn: Jamal Awan
