# Credit Risk Machine Learning Classification

## Background
This model evaluates a dataset of historical lending activity from a peer-to-peer lending services company, and attempts to identify the creditworthiness of borrowers.

## Credit Risk Analysis Report

### Summary
The linear regression model demonstrates a strong fit to the data, as evidenced by its high R-squared value (0.92). The model is able to account for 92% of changes in credit worthiness based on the lending data. The model's coefficients are also statistically significant, which shows a strong relationship between the lending data and the credit worthiness.

### Overview of Analysis
The core purpose of analyzing creditworthiness with linear regression is to predict the likelihood of a borrower repaying a loan. This prediction empowers lenders to make informed decisions about loan approvals, interest rates, and credit limits. By quantifying credit risk, lenders can mitigate potential losses and manage their portfolios more effectively.

1. **Data Collection**: We were provided with historical loan data to analyze, which is stored in the `lending_data.csv` file in the `Resources` directory. The data required minimal cleaning and preprocessing.
2. **Feature Selection**: The notebook code moves the `loan_status` variable to its own data frame, as it represents loan repayment or default. The rest of the features in the loan data were used as predicting factors.
3. **Model Building**: We trained a linear regression model to the lending data to compare the relationship between the predictors and loan repayment or default.
4. **Model Evaluation**: We generated a confusion matrix and a classification report for the model, and assessed the model performance.

### Results
Accuracy:
- The model has an overall accuracy of 99%, indicating that it correctly predicts the risk for 99% of the loans in the dataset.

Precision:
- For low-risk loans, the precision is 1.00, meaning that almost all instances predicted as low-risk are actually low-risk.
- For high-risk loans, the precision is 0.86, meaning that 86% of instances predicted as high-risk are actually high-risk.

Recall:
- For low-risk loans, the recall is 0.99, meaning that the model correctly identifies 99% of actual low-risk borrowers.
- For high-risk loans, the recall is 0.98, meaning that the model correctly identifies 98% of actual high-risk borrowers.
