# Telco Customer Churn Prediction 📉

## Overview
Acquiring a new customer is significantly more expensive than retaining an existing one. This project provides an end-to-end Machine Learning solution using XGBoost to predict customer churn in the telecommunications sector. 

The primary business objective was to maximize **Recall**—ensuring the retention team catches as many at-risk customers as possible before they cancel their service.

![Model Results](chart.png)

## The Business Challenge
* **The Problem:** High churn rates directly impact Monthly Recurring Revenue (MRR). 
* **The Goal:** Build a predictive model optimized for identifying actual churners by minimizing False Negatives. 

## Methodology & Approach
1. **Data Preprocessing:** Handled missing values, standardized numerical features, and applied One-Hot Encoding to categorical variables.
2. **Baseline Model:** Trained an initial XGBoost classifier which yielded a 50% Recall for the minority churn class.
3. **Hyperparameter Tuning:** Addressed class imbalance by implementing `scale_pos_weight` and adjusting decision thresholds.
4. **Final Evaluation:** Successfully increased the churn Recall rate from **50% to 79%**, allowing the business to capture a significantly higher volume of at-risk accounts.

## Key Business Insights
* **Contract Type:** Month-to-month contracts are the highest driver of churn. Customers on 1-year or 2-year contracts show significantly higher loyalty.
* **Internet Service:** Fiber Optic customers have a surprisingly high churn rate, suggesting potential issues with pricing competitiveness, service reliability, or competitor targeting in that tier.

## Tech Stack
* **Python:** Core programming language.
* **Pandas & Scikit-learn:** Data cleaning, encoding, and pipeline preparation.
* **XGBoost:** Gradient boosting classification model.
* **Matplotlib:** Evaluation and feature importance visualization.

## How to Run & Review
All data preparation, EDA, modeling, and evaluation steps are thoroughly documented in the main Jupyter Notebook. 

To review the code and methodology, open: `Customer_Churn_Data_Prep.ipynb`
