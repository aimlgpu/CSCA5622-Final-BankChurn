# CSCA5622-Final-BankChurn

# Bank Customer Churn Prediction

## CSCA 5622 Supervised Learning Final Project

This repository contains the final project for CSCA 5622, focusing on predicting bank customer churn using supervised learning models. The project develops and compares four models—Logistic Regression, Random Forest, Neural Network, and CatBoost—to identify at-risk customers, emphasizing performance and interpretability.

### Dataset
- **Source**: [Kaggle Bank Customer Churn Prediction Dataset](https://www.kaggle.com/datasets/shubhammeshram5797/bank-customer-churn-prediction)
- **Citation**: Meshram, S. (2023). Bank Customer Churn Prediction [Data set]. Kaggle.

### Project Structure
- **Notebook**: [Bank_Churn_Prediction_Final.ipynb](5622-Final-BankCustomerChurn.ipynb) – Contains all steps: problem definition, EDA, preprocessing, model training, results, and conclusion.
- **Output Files** (in `output_files/`):
  - **Plots**:
    - [Numeric Distributions](output_files/numeric_distributions.png) (Step 3b)
    - [Age vs. Churn](output_files/age_vs_churn.png) (Step 3c)
    - [Churn by Geography](output_files/churn_geography.png) (Step 3c)
    - [Correlation Matrix](output_files/correlation_matrix.png) (Step 3c)
    - [Random Forest Feature Importance](output_files/feature_importance_rf.png) (Step 4a)
    - [Neural Network Training History](output_files/nn_training_history.png) (Step 4b)
    - [SHAP Summary](output_files/shap_summary.png) (Step 4c)
    - [ROC Curve Comparison](output_files/roc_curve.png) (Step 4d)
  - **Predictions**:
    - [Logistic Regression & Random Forest](output_files/lr_rf_predictions.csv) (Step 4a)
    - [Neural Network](output_files/nn_predictions.csv) (Step 4b)
    - [CatBoost](output_files/cb_predictions.csv) (Step 4c)
  - **Preprocessed Data**: CSVs in `output_files/` (Steps 1–3d)
- **Video Presentation**: [YouTube Link](#) (to be updated) – 10-minute presentation summarizing the problem, approach, and results.

### Results
- **Best Model**: CatBoost achieved the highest performance (ROC-AUC: 0.88, Class 1 F1-score: 0.62).
- **Key Predictors**: Age, NumOfProducts, Tenure, and Geography (especially Germany) are top drivers of churn.

### How to Run
1. **Environment**: Use Kaggle with GPU P100 enabled (Settings > Accelerator > GPU P100).
2. **Install Dependencies**: Run `!pip install catboost shap` in the notebook.
3. **Execute Notebook**: Run `Bank_Churn_Prediction_Final.ipynb` end-to-end to reproduce results.
4. **View Outputs**: Plots and predictions are in the `output_files/` folder.

### Acknowledgments
- Dataset provided by Shubham Meshram via Kaggle.
- Built using Kaggle’s GPU P100 environment for model training.
