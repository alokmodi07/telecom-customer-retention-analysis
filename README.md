# Telecom Customer Retention Analysis

A practical data analytics and machine learning project that explores customer churn in a telecom dataset and builds baseline models to identify customers who may be at higher risk of leaving.

## Project objective

The goal is to move from raw customer records to actionable retention insights:

- measure the overall churn rate
- identify customer segments associated with higher churn
- examine contract, tenure, service and payment behavior
- prepare data for machine learning
- compare Logistic Regression and Random Forest
- evaluate models using precision, recall, F1 and ROC-AUC

## Tools used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Repository structure

```text
telecom-customer-retention-analysis/
├── data/
│   └── telco_customer_churn.csv
├── notebooks/
│   └── churn_analysis.ipynb
├── reports/
├── visuals/
├── src/
├── requirements.txt
├── .gitignore
└── README.md
```

## Workflow

1. Load and inspect the customer dataset.
2. Convert `TotalCharges` to numeric and handle missing values through the modeling pipeline.
3. Create a binary churn flag.
4. Explore churn across customer segments.
5. Split the data using stratification.
6. Encode categorical features and scale numerical features inside a scikit-learn pipeline.
7. Train Logistic Regression and Random Forest models.
8. Compare Accuracy, Precision, Recall, F1 and ROC-AUC.
9. Translate the analysis into retention-oriented business observations.

## How to run

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

Open `notebooks/churn_analysis.ipynb` and run the cells from top to bottom.

## Dataset

The project uses the commonly distributed Telco Customer Churn dataset. The dataset is included in the repository for reproducibility. If you redistribute the dataset, retain the original dataset's applicable attribution/license information.

## Disclaimer

This is a portfolio/learning project. The model is a baseline and should not be treated as a production customer-retention decision system without validation on current operational data.
