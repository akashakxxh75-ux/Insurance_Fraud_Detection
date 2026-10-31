# Insurance Fraud Detection using Decision Tree Classifier
## Problem Statement:
`Insurance companies face huge losses due to fraudulent claims. The goal was to build a machine learning model that can automatically detect whether a claim is fraud or not.`

## Dataset:
- 1000 insurance claim records
- 39 columns (customer details, policy details, incident details, claim amounts, etc.)
- `Target variable`: fraud_reported (Yes/No)

## Data Preprocessing:
- Removed unnecessary columns (policy number, dates, location)
- Replaced missing values (?) with “unknown”
- Converted target to 0 and 1
- Used One-Hot Encoding for categorical features
- Applied stratified train-test split (80-20)

## Model Used:
- Decision Tree Classifier
- Parameters: max_depth=5, min_samples_leaf=5, class_weight='balanced'
- Why Decision Tree? Easy to interpret and understand feature importance

## Result:
- `Accuracy`: 81%
- `Recall (Fraud)`: 85.7% (model catches most fraud cases)
- `F1 Score`: 68.9%
- `5-Fold Cross Validation F1`: 72%

## Key Insights:
- Most important features:
- Insured Hobbies (especially chess & cross-fit)
- Incident Severity
- Collision Type

- Note: `Model is good at detecting fraud (high recall)`

## Decision Tree:

## Top features for classification

## Tools Used:
- Python, Pandas, Scikit-learn, Matplotlib
