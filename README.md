credit-risk-classification
Machine learning techniques are used to analyze a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.
Overview of the Analysis
Factors considered in the analysis included data on:
•	the size of the loan
•	its interest rate
•	the borrower's income
•	the debt to income ratio
•	the number of accounts the borrower held
•	derogatory marks against the borrower
•	the total debt
Results
Logistic Regression Model 1:
•	Precision: 85% 
•	Accuracy: 95%
•	Recall: 95% (an average--the model had 99% recall in predicting low-risk loans, but 91% recall in predicting high-risk loans)
Logistic Regression Model 2:
•	Precision: 92% (an average--in predicting low-risk loans, the model was 100% precise, though the model was only 85% precise in predicting high-risk loans)
•	Accuracy: 99%
•	Recall: 100%
Summary
Logistic Regression Model 2 is less likely to predict false negative results. However, based on the confusion matrices for each model, Logistic Regression Model 2 predicted slightly more false positives (low-risk when the actual was high-risk).
If the goal of the model is to determine the likelihood of high-risk loans, neither model scores above 95% precision. Logistic Regression Model 2 had fewer false predictions of the testing data overall and would be the best model to use based on the high accuracy and recall of this model.



