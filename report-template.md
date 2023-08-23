# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

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

