# Telco Churn: Data Integrity & Business Relevance Audit in Excel

## Goal:
I will check the integrity of data and check whether it align with the business problem before data cleaning.

## Dataset used:
[Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data)

## Business problem:
The company wants to reduce customer churn. Before analyzing churn patterns, I ensure that the data is complete, clean, and trustworthy.

## Step 1: Is the data relevant to the business problem? 
I asked myself:
- Does this dataset contain all the information I need?
- Are the columns relevant to the question?
- Is any important variable missing?
## Output:
I checked and all the required columns for customer churn analysis like CustomerID, Tenure, Churn, Contract, MonthlyCharges are present. 

## Step 2: Is the data reliable?
1. Check for missing values 
 - I Selected the entire data.
 - Use Conditional Formatting → Highlight Cell Rules → Blanks.
 - Result: Missing values highlighted
2. Check for duplicate values
 - I selected Customer ID column and highlight duplicate values
 - Result: No duplicates found
3. Check for Inconsistent or Invalid Data
 - Tenure should be ≥ 0
 - Use formula in new column:
   =IF(C2<0, "Invalid", "Valid")
 - MonthlyCharges & TotalCharges should be numeric


## 🧹 Pre-Cleaning Checklist

| Check                | Why It's Important                                    |
|---------------------:|:----------------------------------------------------:|
| Relevance to business goal | Avoid wasting time on unrelated data                |
| Completeness         | Incomplete data = weak insights                      |
| Consistency         | Prevents errors and confusion                         |
| Freshness            | Old data may no longer reflect reality               |
| Granularity          | Matches business decision level                       |
| Bias/skew            | Ensures fair representation                          |
| Logic rules          | Validates internal consistency                        |
| Column understanding | Avoids wrong assumptions                             |
| Duplicates           | Prevents overcounting                                 |
| Outliers             | Ensures accurate statistics                          |




