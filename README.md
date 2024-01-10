# 📱📱 AB-test 🧪🧪
![Python version](https://img.shields.io/badge/Python%20version-3.10%2B-lightgrey)
![GitHub last commit](https://img.shields.io/github/last-commit/Taweilo/usa_house_price_prediction)
![GitHub repo size](https://img.shields.io/github/repo-size/Taweilo/usa_house_price_prediction)
![Type of ML](https://img.shields.io/badge/Type%20of%20ML-Regression%20-red)
![License](https://img.shields.io/badge/License-MIT-green)

Badge [source](https://shields.io/)

 <img src="https://www.convertize.com/wp-content/uploads/2021/01/what-is-split-ab-testing-hero.jpg" width="1100" height="400">

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
The goal of this project is to 

## 2. Data Understanding 
The Diabetes dataset was loaded via Colab. The dataset is from Kaggle: kaggle https://www.kaggle.com/datasets/sergylog/ab-test-aggregated-data
 (also please see   attached). Basic data analysis was performed to identify the shape of data, get column names, find missing values, and generate descriptive statistics. The pair plot demonstrated the relationship between variables. The distribution of the target variable was shown.

* Data Dictionary
 
| Name | Measurement Level| Description |
| ----  | ---------------- | ---------- |
| **user_id**  | int | user unique id |
| **group**  | obj | experiment group |
| **views** | int | number of webpage views |
| **clicks** | int | number of experimental feature clicks |
 
## 3. Data Preparation 
1. check missing data
2. create click-through rate (CTR)
  
## 4. Statistical testing   


## 5. Evaluation
MSE in test data: 2193848415.96
R2 score: 0.57
