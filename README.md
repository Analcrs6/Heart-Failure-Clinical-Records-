Project Summary: Heart Failure Prediction & Interpretability

Overview

This project aims to predict the survival of patients with heart failure using clinical records and, crucially, to explain the predictions using various Machine Learning Interpretability (XAI) techniques. By comparing 'Glass Box' models (Logistic Regression, Decision Trees) with 'Black Box' models (Random Forest, XGBoost), the project balances predictive performance with transparency.

Dataset

The analysis uses the Heart Failure Clinical Records Data, comprising 299 patients and 13 clinical features (e.g., age, ejection fraction, serum creatinine). The target variable is DEATH_EVENT.

Methodology

Exploratory Data Analysis (EDA): Investigated distributions, correlations, and outliers. Key drivers identified included time, serum_creatinine, and ejection_fraction.
Model Training: Implemented and hyperparameter-tuned four classifiers:
Logistic Regression
Decision Tree
Random Forest
XGBoost
Explainability (XAI): Utilized state-of-the-art libraries to interpret model behavior:
ELI5: Global feature weights and permutation importance.
LIME: Local surrogate models to explain individual predictions for complex models.
SHAP: Game-theoretic approach for consistent global and local feature attribution.
Results

Performance: The Random Forest model achieved the best results with an Accuracy of ~83% and an AUC-ROC of ~0.91.
Key Findings: Across all models and XAI methods, follow-up time, serum creatinine, and ejection fraction consistently emerged as the most critical predictors of patient survival.
Tools & Libraries

Core: Python, Pandas, Scikit-learn, XGBoost
Visualization: Matplotlib, Seaborn
XAI: ELI5, LIME, SHAP
