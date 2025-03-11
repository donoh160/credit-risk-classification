# credit-risk-classification

# Repo Documents
The lending_data.csv file contains data for 77536 different loans and their risk level under the 'loan_status' column (0-healthy loan, 1-high risk loan)\
The credit_risk_classification file creates a supervised  logistic regression model to predict a loan's risk based on the other features in the .csv

# Overview
The purpose of the project is to predict a loan's risk based on loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, and total_debt. 

# Method
To tackle this goal, a logistic regression model was created using Scikit Learn. \
First, the data was split into training and testing data. Then, the model was fit to the training data using the LogisticRegression function from Scikit Learn utilizing the 'lbfgs' solver. Finally, the model made predictions using the testing data and the results were displayed.

# Results
- Accuracy - 0.99\
(Overall accuracy of the model)

- Precision (Healthy Loans) - 1.00\
- Precision (High-Risk Loans) - 0.88\
(Ratio of correctly predicted loan to the total predicted loan class)

- Recall (Healthy Loans) - 1.00\
- Recall (High-Risk Loans) - 0.91\
(Ratio of correctly predicted class to all data in the actual class.)

# Summary
This model does a good job at predicting healthy and high-risk loans. Out of 19384 loans, the model had only 78 false-positives (0.40%) and 56 false-negatives (0.29%) with a total of 134 incorrect classifications (0.69%). This model could be a great for predicting the risk level of loans, however, depending on what this model is used for, this may be risky to only use this model when making financial desisions.
