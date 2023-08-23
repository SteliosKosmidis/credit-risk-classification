# credit-risk-classification
The instructions for this Challenge are divided into the following subsections:

Split the Data into Training and Testing Sets

Create a Logistic Regression Model with the Original Data

Write a Credit Risk Analysis Report

Split the Data into Training and Testing Sets
Open the starter code notebook and use it to complete the following steps:

Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.

Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

NOTE
A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

Split the data into training and testing datasets by using train_test_split.

Create a Logistic Regression Model with the Original Data
Use your knowledge of logistic regression to complete the following steps:

Fit a logistic regression model by using the training data (X_train and y_train).

Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

Evaluate the model’s performance by doing the following:

Generate a confusion matrix.

Print the classification report.

Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

Write a Credit Risk Analysis Report
Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the README.md file included in your GitHub repository.

Structure your report by using the report template that Starter_Code.zip includes, ensuring that it contains the following:

An overview of the analysis: Explain the purpose of this analysis.

The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

Requirements
Split the Data into Training and Testing Sets (30 points)
To receive all points, you must:

Read the lending_data.csv data from the Resources folder into a Pandas DataFrame. (5 points)

Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns. (10 points)

Split the data into training and testing datasets by using train_test_split. (15 points)

Create a Logistic Regression Model (30 points)
To receive all points, you must:

Fit a logistic regression model by using the training data (X_train and y_train). (10 points)

Save the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model. (5 points)

Evaluate the model’s performance by doing the following:

Generate a confusion matrix. (5 points)

Generate a classification report. (5 points)

Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels? (5 points)

Write a Credit Risk Analysis Report (20 points)
To receive all points, you must:

Provide an overview that explains the purpose of this analysis. (5 points)

Using a bulleted list, describe the accuracy, precision, and recall scores of the machine learning model. (5 points)

Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning. (10 points)




Overview: The purpose of this analysis is to evaluate the performance of machine learning models 
in predicting the credit risk associated with loans.

The stages of the machine learning process in this analysis included:

-Splitting the data 
-Creating and fitting a model 
-Evaluating the model's performance 
(Calculate the accuracy score of the model. 
Generate a confusion matrix. 
Print the classification report.) 
-Resampling the data using RandomOverSampler to find class imbalance 
-Creating and fitting another logistic regression model with the resampled data 
-Evaluating the performance of the resampled model using the same metrics 
-Methods used in this analysis include LogisticRegression and RandomOverSampler for resampling. 
Model 1 had a high accuracy on predicting: -Healthy loans (1.00)and somehow similar accuracy on predicting 
Results:
-High risk loans (0.87). After recall model 1 had similar accuracy on predicting 
-Healthy risk loans (1.00) and -High risk loans (0.89) precision recall f1-score support

       0       1.00      1.00      1.00     18759
       1       0.87      0.89      0.88       625

accuracy                           0.99)     19384
macro avg 0.94 0.94 0.94 19384 weighted avg 0.99 0.99 0.99 19384

Model 2 had a high accuracy on predicting both healthy loans and high risk loan 
-Healthy loans (0.99)and
-High risk loans (0.99). After recall model 2 had similar, but better accuracy than model 1 on predicting 
-Healthy risk loans (0.99) and 
-High risk loans (0.99) precision recall f1-score support

       0       0.99      0.99      0.99     56277
       1       0.99      0.99      0.99     56277

accuracy                           0.99    112554
macro avg 0.99 0.99 0.99 112554 weighted avg 0.99 0.99 0.99 112554 

Summary:
Based on these results only the best model for predicting health and high risk loans is model 2. 
Using model we can minimize the credit risk on loan approvals.
