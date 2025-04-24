# HR Analytics - Employee Attrition Prediction

## Overview

This project focuses on analyzing employee attrition using the IBM HR Analytics dataset from Kaggle. The goal is to understand the key factors that contribute to employee attrition and to build a predictive model that can identify employees who are at a higher risk of leaving the company.

**Dataset:** [IBM HR Analytics Attrition Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

## Project Highlights

* Exploratory Data Analysis (EDA) to understand the data and identify key factors influencing attrition.
* Model training and hyperparameter tuning for several classification algorithms:
    * Random Forest
    * Gradient Boosting
    * CatBoost
    * XGBoost
    * Decision Tree
    * Support Vector Classifier (SVC)
    * Logistic Regression
* Model selection based on accuracy and false positive rate.
* Identification of key predictors of employee attrition.

## Conclusions from EDA

Employee attrition is linked to a combination of categorical and numerical factors:

* **High-Risk Factors:**
    * Frequent travel
    * Overtime work
    * Single marital status
    * Sales or Lab Tech roles
    * Younger age
    * Lower income
    * Longer commute
    * Less tenure
    * Less promotion history

* **Low-Risk Factors (Factors associated with retention):**
    * Married marital status
    * R&D department
    * Higher compensation
    * Greater experience
    * Job stability
    * Recent promotions

* **Strongest Predictors:** Compensation and tenure-related features are the strongest overall predictors of attrition.

## Model Selection

The Support Vector Classifier (SVC) was chosen as the best model due to its high accuracy (0.8980) and low false positive rate (23).

## Repository Structure
