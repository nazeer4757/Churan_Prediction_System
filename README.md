# Customer Churn Prediction & Retention Analysis

## 📌 Problem Statement

Customer churn is a major concern for businesses as it directly impacts revenue.
The goal of this project is to predict whether a customer will churn and identify key factors influencing churn to enable better retention strategies.

---

## 📊 Dataset

* Telco Customer Churn Dataset
* ~7000 customers with demographic, service, and billing information
* Target variable: **Churn (Yes/No)**

---

## ⚙️ Project Workflow

### 1. Data Understanding & Exploration

* Analyzed dataset structure, data types, and missing values
* Identified class imbalance in churn distribution

### 2. Data Cleaning

* Converted `TotalCharges` to numeric
* Removed irrelevant features (`customerID`)
* Handled missing values

### 3. Feature Engineering & Preprocessing

* Encoded categorical variables using **OneHotEncoder**
* Scaled numerical features using **StandardScaler**
* Built preprocessing pipeline using **ColumnTransformer**

### 4. Handling Imbalanced Data

* Applied **SMOTE (Synthetic Minority Oversampling Technique)**
* Balanced churn and non-churn classes

### 5. Model Building

Trained and compared multiple models:

* Logistic Regression (baseline)
* Random Forest
* XGBoost (best performing)

---

## 📈 Model Evaluation

* Used **AUC-ROC** as the primary evaluation metric
* Also evaluated using:

  * Confusion Matrix
  * Precision, Recall, F1-score

👉 **Best Model:** XGBoost
👉 **AUC Score:** ~0.85+ (depends on run)

---

## 🔍 Model Explainability (SHAP)

* Used **SHAP (SHapley Additive exPlanations)** to interpret predictions
* Identified feature impact on churn

### Key Findings:

* Customers with **low tenure** are more likely to churn
* **Month-to-month contracts** have higher churn rates
* **High monthly charges** increase churn probability

---

## 💡 Business Insights & Recommendations

* Encourage customers to opt for long-term contracts
* Provide targeted offers to high-risk customers
* Focus on retaining new customers (low tenure group)

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* XGBoost
* Imbalanced-learn (SMOTE)
* SHAP

---

## 🚀 Conclusion

This project demonstrates an end-to-end machine learning pipeline including data preprocessing, handling class imbalance, model building, evaluation, and explainability, providing actionable insights for customer retention.

---
