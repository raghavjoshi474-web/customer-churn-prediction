# Customer Churn Prediction

A machine learning project to predict which telecom customers are likely to cancel their subscription.

## Problem Statement
Telecom companies lose revenue when customers churn. This project builds a model to identify at-risk customers so the company can take action before they leave.

## Dataset
- Source: [Telco Customer Churn - Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- 7,032 customers | 21 features

## What I Did
- Performed EDA to find patterns in churn behavior
- Cleaned hidden missing values in TotalCharges column
- Preprocessed data using One Hot Encoding and Feature Scaling
- Trained 3 models: Logistic Regression, Random Forest, XGBoost
- Selected XGBoost as final model for best churn detection

## Results
| Model | Accuracy | Churn Recall |
|---|---|---|
| Logistic Regression | 78.82% | 0.52 |
| Random Forest | 78.82% | 0.49 |
| XGBoost | 73.92% | 0.66 |

## Key Findings
- Month-to-month contract customers churn the most
- New customers (0-10 months tenure) are at highest risk
- Customers without Online Security or Tech Support churn more
- XGBoost achieves AUC score of 0.81

## Technologies Used
Python | Pandas | NumPy | Scikit-learn | XGBoost | Matplotlib | Seaborn
