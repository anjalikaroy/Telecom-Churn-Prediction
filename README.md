# Telecom Churn Prediction

## Problem Statement
Customer churn is a major challenge for telecom companies as it directly impacts revenue and customer retention. The goal of this project is to predict whether a customer will churn based on historical customer data and usage patterns.


## Objective
To build a machine learning model that can identify customers who are likely to churn, enabling businesses to take proactive retention measures.


## Dataset
The dataset contains customer-level information including:

- Demographic details (gender, senior citizen, etc.)
- Account information (tenure, contract type, payment method)
- Service details (internet service, phone service, streaming services)
- Billing details (monthly charges, total charges)

Target variable:
- `Churn` → Indicates whether a customer has left the service


## Approach
- Data loading and initial inspection
- Data cleaning:
  - Handling missing values in `TotalCharges`
  - Converting data types
- Exploratory Data Analysis (EDA):
  - Univariate and bivariate analysis
  - Churn distribution analysis
- Data preprocessing:
  - Encoding categorical variables (label encoding / one-hot encoding)
  - Feature scaling using StandardScaler
- Train-test split
- Model building using Logistic Regression
- Model evaluation using classification metrics


## Tech Stack
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## Key Insights
- Customers with month-to-month contracts have higher churn
- Higher monthly charges are associated with increased churn
- Customers with longer tenure are less likely to churn
- Lack of add-on services (like online security/support) increases churn probability

## Model
A Logistic Regression model was used for binary classification.

Steps included:
- Feature encoding and scaling
- Model training on training dataset
- Prediction on test dataset


## Results
- Achieved good classification performance on test data
- Evaluated using:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix

- Model effectively identifies customers at risk of churn


## Outcome
Developed a predictive model that helps telecom companies identify potential churn customers and take preventive actions.

## Business Impact
- Improves customer retention strategies  
- Helps target high-risk customers  
- Reduces revenue loss due to churn  
- Enables data-driven decision making  

## Future Improvements
- Use advanced models (Random Forest, XGBoost)
- Handle class imbalance using SMOTE or class weights
- Hyperparameter tuning
- Deploy model as an API or dashboard

## Project Structure
```text
telecom-churn-prediction.ipynb
README.md
