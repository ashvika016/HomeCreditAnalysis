# HomeCreditAnalysis
Project: Home Credit Default Risk Analysis
An end-to-end Machine Learning code to predict loan repayment ability for unbanked populations using the given data (telco, transactional, and bureau history).
# Project Objectives
Identifying potential defaulters: Building a binary classification model to predict the probability of a client who has payment difficulties(Target: 1).
Broadening financial inclusion: Leverage alternative data sources to provide credit to individuals with little-to-no formal credit history.
Minimizing cost of misclassification: Optimize for ROC-AUC and Recall to ensure high-risk applicants are identified while maintaining a positive experience for reliable borrowers.

# Key Features
Relational Data Integration: Merging and joining several distinct tables (Bureau, Previous Applications, Installments, etc.) into a unified feature set.
Advanced Feature Engineering: Calculates Debt-to-Income ratios and Annuity-to-Credit percentages.
Uses time-based aggregations (e.g., last 12 months of credit card behavior).
Polynomial feature generation for high-impact variables like EXT_SOURCE.
Handling Imbalanced Data: Implements techniques like SMOTE, class weighting, or specialized boosting parameters (LightGBM/XGBoost) to handle the ~8% default rate.
Automated Preprocessing: Clean pipelines for median imputation, One-Hot Encoding for low-cardinality features, and Label Encoding for high-cardinality categories.

# Technical Stack
Analysis: Python (Pandas, NumPy)
Visualization: Matplotlib, Seaborn
Modeling: LightGBM, XGBoost, Scikit-Learn (Logistic Regression, Random Forest)
Experiment Tracking: [e.g., MLflow or Weights & Biases]
Data Source : Kaggle
application_{train|test}.csv: Main data that is unchanged for all applications.
bureau.csv: Previous credits from other financial institutions.
previous_application.csv: History of previous applications within the Home Credit.
installments_payments.csv: Detailed repayment history for previous credits.
