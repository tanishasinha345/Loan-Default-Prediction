# Loan-Default-Prediction

## Project Overview
This project develops a machine learning model to predict whether a borrower is likely to default on a loan. By leveraging historical loan data and machine learning techniques, this project builds accurate, explainable, and scalable loadn default prediction system.

# Dataset Description
The dataset contains historical information about loan applicants and their repayment status.
Features Include:
- Applicant Income
- Co-applicant Income
- Loan Amount
- Loan Amount Term
- Credit History
- Education
- Self Employment Status
- Property Area
- Marital Status
- Gender
- Dependents

### Target Variable
- **0 -> Non-Default**
- **1 -> Default**

# Project Overflow
Data collection -> Data cleaning -> EDA -> Feature Engineering -> Categorical Encoding -> Train Test Split -> SMOTE -> Model Training -> Hyperparameter Tuning -> Cross Validation -> Model Evaluation -> SHAP Explainability 

#  Exploratory Data Analysis (EDA)

EDA was performed to understand the structure and distribution of the dataset.
The analysis included:

- Missing value detection
- Data type inspection
- Class distribution visualization
- Numerical feature distributions
- Outlier identification
- Correlation analysis
- Feature relationship analysis

#  Feature Engineering

Several preprocessing techniques were applied before model training:

- Missing value handling
- Label Encoding of categorical variables
- Feature scaling (where required)
- Removal of unnecessary variables
- Feature transformation
- Train-Test Split

These steps improved model performance and data quality.

#  Handling Class Imbalance (SMOTE)

Loan default datasets are typically imbalanced, with significantly fewer default cases than non-default cases.

To address this issue, the project uses **SMOTE (Synthetic Minority Oversampling Technique)**.

Benefits of using SMOTE:

- Generates synthetic minority class samples
- Prevents model bias toward majority class
- Improves recall for default prediction
- Enhances overall classification performance

#  Models Used

Multiple machine learning algorithms were trained and compared:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost

Each model was evaluated using the same training pipeline to identify the best-performing classifier.

# Hyperparameter Tuning

Hyperparameter optimization was performed to improve model performance.

The tuning process optimized parameters such as:

- Number of estimators
- Regularization parameters
- Maximum features

This resulted in better generalization and improved predictive accuracy.

#  Cross-Validation

To ensure model robustness and reduce overfitting, **Stratified K-Fold Cross Validation** was implemented.

Benefits include:

- Preserves class distribution across folds
- Produces more reliable performance estimates
- Reduces variance caused by a single train-test split

#  Evaluation Metrics

Models were evaluated using multiple classification metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Confusion Matrix
- Classification Report

Using multiple evaluation metrics provides a more comprehensive assessment, especially for imbalanced datasets.

#  SHAP Explainability

To improve model transparency, **SHAP (SHapley Additive exPlanations)** was used.

SHAP helps explain:

- Feature importance
- Individual prediction contributions
- Positive and negative impacts of each feature
- Global model interpretability

This makes the model more trustworthy and suitable for real-world financial applications.

#  Results

The project successfully demonstrates an end-to-end loan default prediction pipeline.

Key achievements include:

- Comprehensive data preprocessing
- Effective handling of class imbalance using SMOTE
- Comparison of multiple machine learning algorithms
- Hyperparameter tuning for performance improvement
- Robust evaluation using Stratified K-Fold Cross Validation
- Model explainability through SHAP analysis

The final selected model provides strong predictive performance while maintaining interpretability.

## Model Performance Comparison

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-------|---------:|----------:|--------:|---------:|--------:|
| Logistic Regression | 0.8087 | 0.8295 | 0.9125| 0.8690 | 0.7329 |
| Decision Tree | 0.6522 | 0.8030 | 0.6625 | 0.7260 | 0.6455 |
| Random Forest | 0.7391 | 0.8205 | 0.8000 | 0.8101 | 0.7507 |
| XGBoost | 0.6522 | 0.8333 | 0.6250 | 0.7143 | 0.7421 |

#  Technologies Used

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
- SHAP
- Joblib

### Machine Learning

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost 


# Future Improvements

Possible enhancements include:

- Deploy the model using Streamlit or Flask
- Build a REST API for real-time predictions
- Automate model retraining with new data
- Implement advanced ensemble techniques
- Experiment with deep learning approaches
- Integrate cloud deployment (AWS, Azure, or GCP)
- Add model monitoring and drift detection
- Develop an interactive dashboard for business users

Author

Tanisha Sinha




