# Telco Customer Churn Prediction

This project uses Machine Learning (XGBoost) to identify customers at risk of leaving a telecommunications company. 

## Project Objective
The goal was to build a model that prioritizes catching as many potential churners as possible (High Recall). This allows the retention team to intervene before the customer actually leaves.

## Tech Stack
* **Python** (Pandas, Scikit-learn)
* **XGBoost** (Machine Learning Model)
* **Matplotlib** (Visualization)

## Key Results
* **Initial Model:** 50% Recall for churners.
* **Tuned Model:** Optimized with scale_pos_weight and custom thresholds to reach **79% Recall**.
* **Main Insights:** Long-term contracts (1-2 years) and Fiber Optic internet service are the most significant predictors of customer behavior.

## How to Run
The analysis is contained in the `Customer_Churn_Data_Prep.ipynb` notebook. It includes data cleaning, one-hot encoding, and model evaluation.
