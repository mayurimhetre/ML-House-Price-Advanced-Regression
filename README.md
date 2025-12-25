# House Prices: Advanced Regression Techniques

kaggle dataset link: https://www.kaggle.com/c/house-prices-advanced-regression-techniques/overview/evaluation

## Overview
The **House Prices: Advanced Regression Techniques** dataset comes from a popular Kaggle competition focused on predicting residential house sale prices. The dataset contains detailed information about homes in **Ames, Iowa**, with a rich mixture of numerical and categorical features that describe many aspects of each property. :contentReference[oaicite:0]{index=0}

## Dataset Description
The training dataset consists of **1,460 houses** and the test dataset contains **1,459 houses**, with **81 total variables** including the target. Among these:
- Around **36 numerical features** (e.g., lot area, year built)
- Around **43 categorical features** (e.g., neighborhood, exterior type)  
These features cover physical attributes, condition, quality, size measurements, and other descriptive details of houses. 

### Examples of Features
- **Numeric:** `GrLivArea`, `TotalBsmtSF`, `LotFrontage`, `YearBuilt`  
- **Categorical:** `Neighborhood`, `HouseStyle`, `Exterior1st`, `SaleCondition`  
- **Target Variable:** `SalePrice` (the final sale price of the house) 

## Objective
The main objective is to build a **regression model** that can accurately predict the **SalePrice** of each house given its features. This involves understanding and preprocessing mixed data types, handling missing values, performing feature engineering, and applying regression algorithms that minimize prediction error.

## Evaluation Metric
Model performance is measured using **Root Mean Squared Logarithmic Error (RMSLE)** — calculated as the Root Mean Squared Error (RMSE) between the **logarithm of predicted prices and log of actual prices**. Using logarithms helps balance errors across both expensive and cheaper houses. 



## Results

**1.Random Forest Regressor:**

{'n_estimators': 800,
 'min_samples_split': 2,
 'min_samples_leaf': 1,
 'max_features': 'sqrt',
 'max_depth': 50,
 'bootstrap': False}
 
 After training the model with hyperparameters
 
 ![image](https://user-images.githubusercontent.com/68188457/119655191-edb54480-be46-11eb-85fc-cc75c261780c.png)

Output of test data

![image](https://user-images.githubusercontent.com/68188457/119655232-fb6aca00-be46-11eb-8296-b7756995d828.png)


