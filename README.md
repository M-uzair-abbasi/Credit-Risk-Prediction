# Credit-Risk-Prediction
Machine learning model to predict credit risk using classification algorithms.
Credit Risk Prediction

This project predicts the likelihood of a borrower experiencing serious delinquency (90+ days overdue) within two years. It uses machine learning classification models to analyze historical credit data and output a probability score for default risk.

📌 Overview

Goal: Predict credit risk probability based on borrower credit history and financial attributes.

Dataset: Contains numerical and categorical features such as delinquency counts, credit utilization, number of loans, and debt ratios.

Challenge: Highly imbalanced dataset (most borrowers are not delinquent).

Output: Probability of serious delinquency (0–1).


⚙️ Features Used

Delinquency history (30–59 days, 60–89 days, 90+ days overdue)

Credit utilization rates

Number of credit lines/loans

Debt-to-income ratio

Number of dependents


🛠️ Steps Performed

1. Data Cleaning

Removed high-missing-value features.

Imputed missing values using median/mode strategies.



2. Feature Engineering

Applied log transformations to skewed count features.

Created binary flags for special conditions.



3. Handling Imbalance

Used class weighting / SMOTE to address imbalance.



4. Model Training

XGBoost Classifier trained on processed features.

Optimized hyperparameters using cross-validation.



5. Prediction Output

Model outputs probabilities instead of binary labels for competition submission.




📊 Model Performance

Evaluation Metric: F1 score

Cross-validation results: 0.24
