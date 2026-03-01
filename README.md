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

Top 20 feature generation for high-impact variables are *EXT_SOURCE(1,2,3), ORGANIZATION_TYPE, CREDIT_TERM, DAYS_EMPLOYED, DAYS_BIRTH, DAYS_ID_PUBLISH, AMT_ANNUITY, DAYS_REGISTRATION, DAYS_LAST_PHONE_CHANGE, AMT_GOODS_PRICE, AMT_CREDIT, OCCUPATION_TYPE, OWN_CAR_AGE, ANNUITY_INCOME_PERCENT, CREDIT_INCOME_PERCENT, REGION_POPULATION_RELATIVE, AMT_INCOME_TOTAL AND education_encoded.*

Automated Preprocessing: Clean pipelines for median imputation, One-Hot Encoding for low-cardinality features, and Label Encoding for high-cardinality categories.

# Technical Stack
Data Source : Kaggle

Analysis: Python (Pandas, NumPy)

Visualization: Matplotlib, Seaborn

Modeling: LightGBM, XGBoost, Scikit-Learn (Logistic Regression, Random Forest)

Experiment Tracking: [e.g., MLflow or Weights & Biases]

application_{train|test}.csv: Main data that is unchanged for all applications.

bureau.csv: Previous credits from other financial institutions.

previous_application.csv: History of previous applications within the Home Credit.
