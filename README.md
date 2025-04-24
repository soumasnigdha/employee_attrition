# Employee Attrition Analysis

## Overview

This project analyzes employee attrition using the "Predicting Employee Attrition" dataset from Kaggle ([https://www.kaggle.com/datasets/pavan9065/predicting-employee-attrition/](https://www.kaggle.com/datasets/pavan9065/predicting-employee-attrition/)). The goal is to identify the key factors that contribute to employee attrition and to build a predictive model that can help organizations take proactive measures to retain valuable employees.

## Dataset

The dataset contains various employee attributes, including:

* **Demographics:** Age, Gender, MaritalStatus
* **Job-related:** Department, JobRole, JobLevel, JobSatisfaction
* **Salary:** MonthlyIncome, PercentSalaryHike
* **Work-life:** WorkLifeBalance, OverTime, DailyRate
* **Tenure:** YearsAtCompany, YearsInCurrentRole, YearsSinceLastPromotion, YearsWithCurrManager
* **Travel:** BusinessTravel
* **Attrition:** Target variable indicating whether an employee has left the company (Yes/No)

## Project Goals

1.  Perform Exploratory Data Analysis (EDA) to understand the factors influencing employee attrition.
2.  Train and evaluate several machine learning models to predict attrition.
3.  Identify the best-performing model.
4.  Provide insights and recommendations for HR departments to reduce attrition.

## Methodology

1.  **Exploratory Data Analysis (EDA):**
    * Explored the dataset to understand the distribution of features and their relationship with attrition.
    * Identified key categorical and numerical factors associated with attrition.
2.  **Model Training and Evaluation:**
    * Trained and hyper-tuned the following machine learning models:
        * RandomForestClassifier
        * GradientBoostingClassifier
        * CatBoostClassifier
        * XGBoostClassifier
        * DecisionTreeClassifier
        * SVC (Support Vector Classifier)
        * LogisticRegression
    * Evaluated model performance using accuracy and false positive rate.
3.  **Model Selection:**
    * Selected the Support Vector Classifier (SVC) as the best-performing model due to its highest accuracy (0.8980) and lowest false positive rate (23).

## Key Findings (From EDA)

Employee attrition is influenced by a combination of categorical and numerical factors:

* **Categorical Factors:**
    * **Higher Attrition:** Frequent travel, working overtime, being single, and working in Sales or Lab Tech roles.
    * **Lower Attrition (Higher Retention):** Being married and working in R&D.
* **Numerical Factors:**
    * **Higher Attrition:** Younger age, lower income, longer commute, less tenure (at the company and with the manager), and fewer promotions.
    * **Lower Attrition (Higher Retention):** Higher salary, more experience, greater job stability, and recent recognition or promotions.
* **Strongest Predictors:** Compensation and tenure-related features are the strongest indicators of attrition.
* **Less Influential Factors**: Performance rating, education, and training frequency show little distinction.

## Recommendations

Based on the analysis, the following recommendations can be implemented to reduce employee attrition:

* **Address Overtime:** Implement policies and practices to manage and reduce excessive overtime.
* **Review Compensation and Benefits:** Ensure competitive salaries and benefits, especially for younger employees and those with shorter tenure.
* **Promote Work-Life Balance:** Encourage a healthy work-life balance to reduce stress and burnout.
* **Enhance Employee Engagement:** Develop targeted engagement programs for employees in Sales and Lab Tech roles.
* **Support Career Development:** Provide opportunities for growth and promotion to increase employee retention.
* **Strengthen Manager-Employee Relationships:** Foster positive relationships between employees and their managers.
* **Consider Travel Policies:** Evaluate the impact of frequent travel on employee satisfaction and attrition.

## Conclusion

This project provides valuable insights into the factors that drive employee attrition. By understanding these factors and implementing the recommended strategies, organizations can create a more supportive and engaging work environment, leading to increased employee retention and reduced turnover costs. The Support Vector Classifier (SVC) model can be used as a tool to predict which employees are more likely to leave, allowing for targeted interventions.

## Further Improvements

* Explore other machine learning models or ensemble methods to potentially improve prediction accuracy.
* Conduct a cost-benefit analysis of different retention strategies.
* Gather more data on employee satisfaction and engagement to enhance the analysis.
* Deploy the model as a web application or API for practical use by HR departments.

