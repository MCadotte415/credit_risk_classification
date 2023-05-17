# credit_risk_classification
Instructions
The instructions for this Challenge are divided into the following subsections:

Split the Data into Training and Testing Sets

Create a Logistic Regression Model with the Original Data

Predict a Logistic Regression Model with Resampled Training Data

Write a Credit Risk Analysis Report

Split the Data into Training and Testing Sets
Open the starter code notebook and use it to complete the following steps:

Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.

Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

Create a Logistic Regression Model with the Original Data
Use your knowledge of logistic regression to complete the following steps:

Fit a logistic regression model by using the training data (X_train and y_train).

Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

Evaluate the model’s performance by doing the following:

Calculate the accuracy score of the model.

Generate a confusion matrix.

Print the classification report.

Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?
Write a Credit Risk Analysis Report
Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the README.md file included in your GitHub repository.

Structure your report by using the report template that Starter_Code.zip includes, ensuring that it contains the following:

An overview of the analysis: Explain the purpose of this analysis.

The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

Overview of the Analysis:

•	The purpose of this analysis is to build a model that can identify the creditworthiness of borrowers.

•	Dependent variable (y value) in this analysis was the "loan status" indicating if a loan is healthy or at risk.

•	Independent Variables (x values) were loan size, interest rate, borrower income, debt to income ratio, number of accounts and derogatory marks.

•	In this analysis, we first split our data to training and test sets. Then, define our dependent and independent variables. Next, we create logistic regression model and fit our original data to this model. Trained model is used to make predictions. Lastly, we evaluate the model`s performance.

•	Two different Logistic Regression models were created by using the original data set and randomly over resampled data set (to get rid of the imbalances). In the end, their results -which was gathered with scikit-learn library- were compared.

Summary:

Analysis show that collected data can be effectively used to train and test the Machine Learning Classification Model. Randomly oversampling the data helps us to get higher balanced accuracy and recall scores. With higher recall value, the model can predict risky loans more accurately.

With incorrect predictions we have two issues:
False positives (where users are flagged as risky, but are actually healthy)
False negatives (where users are not flagged as risky but are actually risky)
Both cases have its costs. It is important to predict both 1s and 0s. Therefore, model should have good accuracy in terms of both.

