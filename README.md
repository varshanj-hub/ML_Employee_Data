# 🧠 ML_Employee_Data

A machine learning project aimed at predicting **employee attrition** and identifying the key factors that influence whether an employee stays or leaves the organization.  
The project combines statistical reasoning with modern ML techniques to build accurate and interpretable models.

---

## 🚀 Project Overview
This project focuses on analyzing HR data to understand the major drivers of employee attrition.  
It involves end-to-end machine learning — from data preprocessing and visualization to model training, optimization, and performance comparison.

---

## 🧹 Data Preprocessing Methods
To ensure high-quality input for modeling, several preprocessing techniques were applied:
- **Handling Missing Values:** Replaced using `SimpleImputer` for numeric and categorical variables.  
- **Feature Encoding:** Converted categorical variables using `OneHotEncoder`.  
- **Feature Scaling:** Applied `StandardScaler` for continuous features.  
- **Feature Selection:** Dropped irrelevant columns such as `EmployeeCount`, `EmployeeNumber`, `StandardHours`, and `Over18`.  
- **Imbalanced Data Handling:** Used **SMOTE (Synthetic Minority Oversampling Technique)** to balance the target variable (`Attrition`).

---

## 📊 Exploratory Data Analysis (EDA)
EDA was performed to explore the relationships between employee features and attrition:
- Distribution plots, count plots, and boxplots to visualize key patterns  
- Identification of high-risk groups such as those with low satisfaction, long working hours, or fewer promotions  

---

## 🧠 Machine Learning Algorithms Used
The project compares multiple supervised learning algorithms for binary classification:

| Algorithm | Description | Type |
|------------|--------------|------|
| **Logistic Regression** | Baseline linear model for attrition prediction | Linear |
| **Decision Tree Classifier** | Tree-based model that splits data based on information gain | Non-linear |
| **Random Forest Classifier** | Ensemble of decision trees with bagging to reduce variance | Ensemble |
| **XGBoost Classifier** | Gradient boosting model optimized for speed and accuracy | Ensemble |
| **LightGBM Classifier** | Boosting framework that handles large datasets efficiently | Ensemble |
| **CatBoost Classifier** | Gradient boosting with categorical handling and overfitting control | Ensemble |

---

## 🧩 Model Evaluation
All models were evaluated using the following performance metrics:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **ROC-AUC Score**

These metrics ensured a balanced assessment between model correctness and generalization.

---

## 🏆 Best Performing Model
### **CatBoost Classifier**
CatBoost achieved the **highest overall performance** across all metrics — particularly **F1-score and ROC-AUC** — due to its:
- Automatic handling of categorical features  
- Robustness against overfitting  
- Superior learning rate optimization  
- Faster convergence and efficient boosting on structured (tabular) data  

**Hence, CatBoost was identified as the best model** for predicting employee attrition in this dataset.

---

## ⚙️ Tech Stack
- **Language:** Python  
- **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, `lightgbm`, `catboost`, `imbalanced-learn`  

---

## 🧾 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/ML_Employee_Data.git
   cd ML_Employee_Data
