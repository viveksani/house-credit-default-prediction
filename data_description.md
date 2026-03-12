# Dataset Description

This project uses the Home Credit Default Risk dataset.

Each row in the dataset represents a loan application submitted by a client.

The goal is to predict whether the applicant will default on the loan.

## Target Variable

TARGET

0 → Client successfully repaid the loan  
1 → Client defaulted on the loan

## Important Features

AMT_INCOME_TOTAL  
Total income of the client.

AMT_CREDIT  
Total credit amount requested by the client.

AMT_ANNUITY  
Loan annuity payment amount.

EXT_SOURCE_1 / EXT_SOURCE_2 / EXT_SOURCE_3  
External credit risk scores provided by third-party agencies.

DAYS_BIRTH  
Age of the client.

DAYS_EMPLOYED  
Employment duration of the client.

## Feature Engineering

Additional features were created to capture financial relationships:

credit_income_ratio  
Ratio between credit amount and total income.

annuity_income_ratio  
Ratio between annuity payment and income.

credit_annuity_ratio  
Relationship between total credit and annuity.

ext_source_mean  
Average of external risk scores.

ext_source_pred  
Multiplication of external risk scores.

ext_diff  
Difference between external risk scores.

These engineered features help the model better understand financial risk patterns.