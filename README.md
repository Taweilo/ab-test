# 📱📱 AB-test 🧪🧪
![Python version](https://img.shields.io/badge/Python%20version-3.10%2B-lightgrey)
![GitHub last commit](https://img.shields.io/github/last-commit/Taweilo/usa_house_price_prediction)
![GitHub repo size](https://img.shields.io/github/repo-size/Taweilo/usa_house_price_prediction)
![Type of ML](https://img.shields.io/badge/Type%20of%20ML-Regression%20-red)
![License](https://img.shields.io/badge/License-MIT-green)

Badge [source](https://shields.io/)

 <img src="https://www.convertize.com/wp-content/uploads/2021/01/what-is-split-ab-testing-hero.jpg" width="550" height="200">


```
├── Image                       
│
├── Code_USA_House_Price_Prediction.ipynb             <- code
├── LICENSE                                           <- MIT license
├── README.md                                         <- read me
├── housing_price_dataset.csv                         <- dataset
├── USA_House_Price_Prediction_Report                 <- presentation


```

## 1. Business Understanding
The goal of this project is to develop a predictive model for housing prices based on various property attributes, including area, number of bedrooms and bathrooms, etc.

## 2. Data Understanding 
The Diabetes dataset was loaded via Colab. The dataset is from Kaggle: kaggle https://www.kaggle.com/datasets/sergylog/ab-test-aggregated-data
 (also please see housing_price_dataset.csv attached). Basic data analysis was performed to identify the shape of data, get column names, find missing values, and generate descriptive statistics. The pair plot demonstrated the relationship between variables. The distribution of the target variable was shown.

* Data Dictionary
 
| Name | Modeling Role | Measurement Level| Description |
| ---- | ------------- | ---------------- | ---------- |
| **SquareFeet** | input | int | Square Feet of the house |
| **Bedrooms** | input | int | Amount of bedrooms |
| **Bathrooms**| input | int | Amount of bathrooms |
| **Neighborhood** | input | obj | Area neighborhood where the house is |
| **YearBuilt** | input |  int | Which year it was built |
| **Price** | input |  boolean | The price of the home |
 
## 3. Data Preparation 
1. Define variables (X and y) 
2. Split the data into train and test datasets; 40% of test data <br>
   train: 30000 data<br>
   test:  20000 data<br>
  
## 4. Modeling   
Several machine learning models were included:
* Linear Regression

## 5. Evaluation
MSE in test data: 2193848415.96
R2 score: 0.57
