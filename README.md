#  Instacart Market Basket Analysis & Prediction

##  Project Overview
This project applies **Machine Learning classification and regression models** to analyze and predict customer reorder behavior using the **Instacart Market Basket dataset**.

The project focuses on two main tasks:
- **Binary Classification:** Predict whether a user will reorder a specific product.
- **Regression:** Predict the total number of times a user will reorder products.

Multiple models were evaluated, with **XGBoost** emerging as the best-performing approach for both tasks.

---

##  Objectives
- Understand customer purchasing behavior
- Handle class imbalance and high-cardinality data
- Engineer meaningful behavioral features
- Compare linear, tree-based, and boosting models
- Evaluate model robustness and explainability

---

##  Dataset Description
The dataset consists of multiple relational tables:
- `orders`
- `products`
- `aisles`
- `departments`
- `order_products__prior`
- `order_products__train`

Key challenges include:
- Severe class imbalance in the `reordered` target
- Temporal dependency between orders
- Non-linear user–product interactions

---

##  Technologies & Libraries
- Python  
- Pandas, NumPy  
- Scikit-learn  
- XGBoost  
- Imbalanced-learn (SMOTE, RandomUnderSampler)  
- Statsmodels  
- SHAP  
- Matplotlib  
- Google Colab  

---

##  Project Workflow
1. Data loading and preprocessing  
2. Exploratory Data Analysis (EDA)  
3. Feature engineering (user, product, interaction features)  
4. Handling class imbalance (SMOTE & under-sampling)  
5. Model training and evaluation  
6. Hyperparameter tuning using TimeSeriesSplit  
7. Model explainability (SHAP)  
8. Robustness and statistical testing  

---

## ▶ How to Run the Project (Google Colab)

1. Open the notebook in **Google Colab**
2. Mount Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
3. Ensure the dataset files are placed inside your Drive directory
4. Run the notebook cells **in order**
5. Model outputs, metrics, and visualizations will be generated automatically

---

##  Models Implemented

### Classification
- Logistic Regression  
- SVM (Linear)  
- K-Nearest Neighbors  
- Decision Tree  
- Random Forest  
- **XGBoost (Best Performer)**  

### Regression
- Ridge, Lasso, ElasticNet  
- KNN Regressor  
- Decision Tree Regressor  
- Random Forest Regressor  
- **XGBoost Regressor (Best Performer)**  

---

##  Evaluation Metrics

### Classification
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- ROC AUC  

### Regression
- MAE  
- RMSE  
- R² Score  

Time-aware validation was applied using **TimeSeriesSplit** to prevent data leakage.

---

##  Model Explainability
- Feature importance analysis
- SHAP values for global and local interpretability
- Behavioral insights derived from top predictive features

---

##  Robustness & Statistical Analysis
- Gaussian noise sensitivity testing
- Outlier injection stress testing
- Learning curve analysis (data sparsity)
- Breusch–Pagan test for heteroscedasticity

---

##  Key Findings
- Tree-based and boosting models significantly outperform linear models
- XGBoost captures complex, non-linear user behavior effectively
- The model is robust to small noise but sensitive to extreme outliers
- User history is the strongest predictor of future reorders

---

##  Limitations
- SMOTE is computationally expensive for large datasets
- Under-sampling may discard potentially useful data
- Regression variance increases for high-frequency users

---

##  Future Improvements
- Advanced cold-start handling for new users
- Real-time input validation and outlier clipping
- Model deployment with reduced feature set for faster inference

---

##  Author
Machine Learning Project – Instacart Market Basket Analysis  
January 2026
