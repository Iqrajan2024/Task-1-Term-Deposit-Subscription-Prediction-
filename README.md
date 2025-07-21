# Term Deposit Subscription Prediction (Bank Marketing)

## Overview
This project focuses on predicting whether a bank customer will subscribe to a term deposit based on marketing campaign data. The task leverages machine learning classifiers along with explainable AI to derive meaningful, interpretable insights from the model predictions.

## Objective
To build and evaluate predictive models that can accurately forecast whether a client will subscribe to a term deposit product, using the bank's historical marketing data.

## Dataset Description
- **Source**: UCI Machine Learning Repository - Bank Marketing Dataset
- **Features**: Includes customer attributes (e.g., age, job, marital status), contact campaign details (e.g., contact method, duration), and historical campaign outcomes.
- **Target Variable**: `y` – whether the client subscribed to a term deposit (`yes` or `no`)

## My Approach
1. **Data Cleaning**: Removed irrelevant or redundant features, managed categorical columns, and dealt with class imbalance.
2. **Exploratory Data Analysis (EDA)**: Visualized relationships between key features and the target variable.
3. **Preprocessing**:
   - Encoded categorical variables
   - Addressed class imbalance using oversampling
   - Scaled numerical features for consistency
4. **Model Building**:
   - Trained Logistic Regression and Random Forest models
   - Evaluated model performance using accuracy, confusion matrix, and ROC curves
5. **Model Interpretability**:
   - Used SHAP (SHapley Additive exPlanations) to explain feature importance and model decisions

## Key Insights
- **Duration** of the last contact is the strongest predictor of term deposit subscription.
- Other important features include:
  - **poutcome**: outcome of the previous campaign
  - **contact**: communication type (e.g., cellular, telephone)
  - **housing**: whether the customer has a housing loan
- High values for key features (e.g., long duration, successful previous outcome) significantly increase the likelihood of a positive prediction.
- Low or missing feature values tend to reduce the model's confidence.

## Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- SHAP (for model interpretability)

## Skills Demonstrated
- Supervised machine learning (classification)
- Data cleaning and preprocessing
- Handling class imbalance
- Model evaluation and validation
- Explainable AI and interpretation of feature importance
