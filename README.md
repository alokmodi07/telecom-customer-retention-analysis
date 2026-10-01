 # Telecom Customer Retention & Churn Analysis

A data analytics and machine learning project focused on understanding customer churn in the telecom industry.

The project analyzes customer demographics, tenure, contracts, internet services, payment methods, and billing information to identify customer segments associated with higher churn and build baseline machine learning models for churn prediction.

## Business Problem

Customer churn can affect recurring revenue and customer lifetime value.

This project aims to answer:

- What percentage of customers are leaving?
- Which customer segments have higher churn rates?
- How does contract type relate to churn?
- Which payment methods are associated with higher churn?
- How does customer tenure differ between churned and retained customers?
- Can machine learning help identify customers at higher risk of churn?

## Key Findings

### Overall Churn

- Total customers analyzed: **7,043**
- Customers who churned: **1,869**
- Overall churn rate: **26.5%**

### Churn by Contract Type

| Contract | Churn Rate |
|---|---:|
| Month-to-month | 42.7% |
| One year | 11.3% |
| Two year | 2.8% |

Month-to-month customers had a substantially higher observed churn rate than customers on longer contracts.

### Churn by Payment Method

| Payment Method | Churn Rate |
|---|---:|
| Electronic check | 45.3% |
| Mailed check | 19.1% |
| Bank transfer (automatic) | 16.7% |
| Credit card (automatic) | 15.2% |

Electronic-check customers had the highest observed churn rate in this dataset.

### Churn by Internet Service

| Internet Service | Churn Rate |
|---|---:|
| Fiber optic | 41.9% |
| DSL | 19.0% |
| No internet service | 7.4% |

### Customer Tenure

Customers who churned generally had shorter tenure than customers who remained with the company.

## Machine Learning

Two classification models were developed:

1. Logistic Regression
2. Random Forest

### Model Performance

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 73.7% | 50.3% | 78.3% | 61.3% | 84.1% |
| Random Forest | 77.0% | 55.1% | 71.7% | 62.3% | 83.9% |

The models were evaluated using a stratified train-test split.

Because churn detection is a classification problem, Precision, Recall, F1 Score and ROC-AUC were considered alongside accuracy.

## Project Workflow

```text
Raw Data
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Customer Segmentation
   ↓
Feature Preparation
   ↓
Train-Test Split
   ↓
Feature Encoding & Scaling
   ↓
Machine Learning
   ↓
Model Evaluation
   ↓
Business Insights
