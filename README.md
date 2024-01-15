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
Now we will run A/B testing for CTR.
For A/B testing to be applied, the data set must satisfy the Normality and Variance homogeneity assumptions.
If normality and variance homogeneity is provided, an independent two-sample t-test (parametric test) is applied.
If normality and homogeneity of variance are not provided, the Mann-Whitney U test (non-parametric test) is performed. How to check the assumption of normality? In this, we will first determine the H0 and H1 hypotheses.

1. Shapiro-Wilk test
- H0: The assumption of normality is provided.
- H1: The assumption of normality is not provided. Now let's check the assumption of normality.

2. Mann-Whitney U test
- H0: There is no significant difference between the two groups in terms of click rate to the desired page.
- H1: There is a difference.

## 5. Evaluation
1. The Shapiro-Wilk Test suggests the data set does not follow the Normality and Variance homogeneity assumptions.
2. The Mann-Whitney U test suggests CTR is a difference between the control and test groups. <br>
While the average conversion rate was 3.46% in the Control group, this rate increased to 3.86% in the Test group. 
As a result of our tests, we can say that this rate increase is not accidental, but has been proven statistically.
