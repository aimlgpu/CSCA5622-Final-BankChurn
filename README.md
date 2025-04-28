# Assignment: CSCA 5622 Supervised Learning Final Project

# Introduction: Bank Customer Churn Prediction Using Supervised Learning

## Project Overview

### Problem Statement
This project focuses on predicting bank customer churn, a critical challenge for financial institutions aiming to retain their client base. The task is to determine whether a customer will churn (close their account), which is a **binary classification problem**. The type of learning employed is **supervised learning**, where we use labeled data (Exited: 0 = No Churn, 1 = Churn) to train models that predict churn likelihood based on customer features.

### Importance and Goal
Customer churn prediction is vital for banks like HSBC or JPMorgan, as retaining high-value clients can save between 10M to 500M annually by 2025 (estimated based on industry retention costs). The **goal** of this project is to develop and compare supervised learning models—Logistic Regression, Random Forest, Neural Network, and CatBoost—to accurately identify at-risk customers. By focusing on both performance (e.g., ROC-AUC, F1-score) and interpretability (e.g., SHAP analysis), the project aims to provide actionable insights for financial applications, such as targeted retention campaigns. Additionally, this project explores advanced techniques like GPU-accelerated training and SHAP for interpretability, enhancing my skills in model development and analysis.

## Dataset Description

### Data Source
The dataset used is the **Kaggle Bank Customer Churn Prediction dataset**, sourced from Kaggle ([link to dataset](https://www.kaggle.com/datasets/shubhammeshram579/bank-customer-churn-prediction)). This public dataset is cited as:
- Meshram, S. (2023). Bank Customer Churn Prediction [Data set]. Kaggle. https://www.kaggle.com/datasets/shubhammeshram579/bank-customer-churn-prediction

### Data Characteristics
- **Size**: The dataset contains 10,002 samples (rows) and 11 features (columns) initially, reduced to 10 features after dropping the irrelevant `RowNumber` column.
- **Feature Types**: There are 8 numeric features (`CreditScore`, `Age`, `Tenure`, `Balance`, `NumOfProducts`, `HasCrCard`, `IsActiveMember`, `EstimatedSalary`) and 2 categorical features (`Geography`, `Gender`). The target variable, `Exited`, is a binary label (0 or 1).
- **Key Features**:
  - `CreditScore`: Numeric, customer’s credit score (range: ~350–850).
  - `Geography`: Categorical, customer’s location (`France`, `Spain`, `Germany`).
  - `Gender`: Categorical, customer’s gender (`Male`, `Female`).
  - `Age`: Numeric, customer’s age (range: ~18–92).
  - `Balance`: Numeric, account balance (range: 0–250,000).
  - `NumOfProducts`: Numeric, number of bank products used (1–4).
  - `Exited`: Binary target (0 = No Churn, 1 = Churn).
- **Single Source**: The data is from a single tabulated CSV file, not multi-table or gathered from multiple sources.
