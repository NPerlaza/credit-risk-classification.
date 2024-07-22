
# Module  Report

## Overview of the Analysis

The purpose of this analysis was to build and evaluate a machine learning model to predict the creditworthiness of borrowers using historical lending data from a peer-to-peer lending services company. The dataset contained financial information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The target variable was `loan_status`, where a value of 0 indicated a healthy loan and a value of 1 indicated a high-risk loan.

The analysis involved several stages:
1. **Data Preparation:** The data was read into a Pandas DataFrame, and the target variable (`loan_status`) was separated from the features.
2. **Data Splitting:** The data was split into training and testing sets using `train_test_split`.
3. **Model Training:** A logistic regression model was trained using the training data.
4. **Model Evaluation:** The model's performance was evaluated using a confusion matrix and a classification report.

The primary method used in this analysis was `LogisticRegression` from the scikit-learn library.

Results

Machine Learning Model 1: Logistic Regression
- Accuracy: 0.99
- Precision:
  - Class 0 (Healthy Loan): 1.00
  - Class 1 (High-Risk Loan): 0.85
- Recall:
  - Class 0 (Healthy Loan): 0.99
  - Class 1 (High-Risk Loan): 0.91

 Summary

The logistic regression model performed exceptionally well in predicting both healthy and high-risk loans. The model achieved an accuracy of 99%, with a precision of 1.00 for healthy loans and 0.85 for high-risk loans. The recall was 0.99 for healthy loans and 0.91 for high-risk loans.

Given these results, the logistic regression model is highly recommended for predicting the creditworthiness of borrowers. The model's high accuracy and recall for high-risk loans are particularly important for minimizing the risk of defaults. The performance of the model indicates that it can reliably distinguish between healthy and high-risk loans, making it a valuable tool for the company's lending decisions.

