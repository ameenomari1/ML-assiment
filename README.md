# Instacart Market Basket Analysis & Prediction

## Summary
This project analyzes customer purchasing behavior using the **Instacart Market Basket dataset**. The goal is to predict:

1. Classification Task – whether a specific product will be reordered by a user (binary classification).  
2. Regression Task – the total number of times a user will reorder products (count regression).

Key steps include:
- Exploratory Data Analysis (EDA): temporal patterns, missing values, outliers, class imbalance.  
- Preprocessing and Feature Engineering: user-level, product-level, and user-product interaction features; non-linear transformations.  
- Model Selection and Tuning: linear models, tree-based models, XGBoost.  
- Evaluation: ROC AUC (classification), R² & MAE (regression).  
- Explainability and Robustness: SHAP, feature importance, sensitivity to noise and outliers.  

Final Models:
- Classification: Tuned XGBoost (ROC AUC ≈ 0.838)  
- Regression: Baseline XGBoost (R² ≈ 0.832)  

Project Contributors:
Project Contributors and Roles:

- Ameen – Responsible for Exploratory Data Analysis (EDA) and data merging/preprocessing and presention 
- Mustafa – Responsible for Feature Engineering and report 
- Both Ameen and Mustafa – Collaborated on Task A (Classification) and Task B (Regression)

---

## Run Instructions on Google Colab

### 1. Open the Notebook
- Open Google Colab: [https://colab.research.google.com](https://colab.research.google.com)  
- Upload or open your main notebook file (e.g., `Instacart_Analysis.ipynb`).

### 2. Mount Google Drive
If your dataset is stored in Google Drive:
```python
from google.colab import drive
drive.mount('/content/drive')
