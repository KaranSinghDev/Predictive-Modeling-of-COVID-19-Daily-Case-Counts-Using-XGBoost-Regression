# Predictive Modeling of COVID-19 Daily Case Counts Using XGBoost Regression

## Problem
Accurate forecasting of daily COVID-19 cases is crucial for effective resource allocation and planning during the pandemic. With the highly dynamic nature of the virus's spread, relying on traditional methods often leads to inaccurate predictions that hinder response efforts. This project aims to address the challenge of predicting daily case counts based on historical data.

## Solution
This project employs machine learning techniques to build a regression model that predicts daily COVID-19 cases using the XGBoost algorithm. By leveraging historical case data across various states, the model enhances prediction accuracy compared to traditional forecasting methods. The insights gained from this predictive model provide valuable information to public health officials and policymakers, facilitating more effective decision-making in response to the pandemic.

## Dataset
The dataset used in this project consists of historical COVID-19 case counts from various states, encompassing a wide array of features. Key columns include:
- **id**: Unique identifier for each entry
- **AL**: Case counts in Alabama
- **AK**: Case counts in Alaska
- **AZ**: Case counts in Arizona
- **...**: (continues for other states)
- **tested_positive**: Number of positive test cases

**Source**: [Kaggle COVID-19 Daily Cases Prediction Challenge](https://www.kaggle.com/competitions/ml2021spring-hw1/data)

## Model Details
The model implemented is the **XGBoost Regressor**, a robust gradient boosting framework that excels in regression tasks. The hyperparameters used for the model include:
- **Objective**: `reg:squarederror`
- **Number of estimators**: 100
- **Learning rate**: 0.024
- **Evaluation metric**: `mae` (Mean Absolute Error)
- **Device**: `cuda:0` (for GPU acceleration)

## Evaluation
The model's performance is assessed using Root Mean Squared Error (RMSE) as the evaluation metric. The cross-validation mean score achieved was **0.9071**, indicating the model's strong predictive capability.

## Citation
ntuee. *ML2021Spring-hw1*. [Kaggle COVID-19 Daily Cases Prediction Challenge](https://kaggle.com/competitions/ml2021spring-hw1), 2021. Kaggle.
