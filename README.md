#Problem
The COVID-19 pandemic highlighted the need for accurate and timely forecasting of daily case counts, enabling governments and healthcare organizations to prepare and allocate resources more effectively. Predicting daily COVID-19 cases, however, is challenging due to the highly dynamic nature of the pandemic, with variations across regions, timeframes, and demographic factors.

#Solution
This project builds a machine learning model using the XGBoost regression algorithm to accurately predict daily COVID-19 cases. By applying advanced regression methods and optimizing hyperparameters, this model outperforms many traditional prediction techniques. The predictive capabilities of this model offer a reliable tool for stakeholders to make informed decisions, contributing to improved responses and preparations against the ongoing challenges of COVID-19.

#Data
Dataset: The dataset contains historical data on COVID-19 case counts from various states, with each feature representing a different region or case attribute.
Source: Kaggle COVID-19 Daily Cases Prediction Challenge
#Data Description:
Training samples: 2700
Testing samples: 893
Features: 94 columns, with each column representing attributes like case counts in different states (e.g., "CA" for California, "TX" for Texas, etc.).
#Model
Algorithm: XGBoost Regressor
#Hyperparameters:
objective='reg:squarederror'
n_estimators=100
learning_rate=0.024
eval_metric='mae' (Mean Absolute Error for validation)
device='cuda:0' (utilizing GPU for training efficiency)
#Preprocessing Steps:
Imputed missing values, if any, using column-wise means or modes
Categorical encoding: Converted categorical features into numerical ones using one-hot encoding
Standardization: Scaled numerical features for optimal model performance
#Evaluation
Evaluation Metric: Root Mean Squared Error (RMSE)
Cross-Validation Score: Mean RMSE of 0.9071, providing a reliable measure of model generalization across different data splits.
#Citation
ntuee. ML2021Spring-hw1. Kaggle COVID-19 Daily Cases Prediction Challenge, 2021. Kaggle.
