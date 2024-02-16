# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
        
        The purpose of this analysis was to predict how many borrowers would be a credit risk. 

* Explain what financial information the data was on, and what you needed to predict.

        Financial information included in the data were factors such as loan size, interest rate, borrower's income, debt to income ratio, number of accounts, derogatory marks on borrower's accounts, interest rate, loan status and total debt.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

        The main variable that was the focus of this analysis was the "loan_status" column. This column reported which users were in good standing with their loan versus those who were not.

* Describe the stages of the machine learning process you went through as part of this analysis.

        First, we isolated the "loan_status" column to get the counts we need to feed to our machine learning model. Once we had that data we used common machine learning syntax to predict which loans were a high risk versus healthy loans.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

        We used Logistic Regression for our model by using the training data. This smaller set of data gave us our first batch of results.   
        After, we oversampled the data using the RandomOverSampler module from the imbalanced-learn library to get extra data to compare against the original training data.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

        - Accuracy: 95%
        - Precision: 100% for healthy loans / 85% for high-risk loans
        - Recall: The model was able to find 99% of healthy loans / 91% of high-risk loans

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

        - Accuracy: 95%
        - Precision: 100% for healthy loans / 86% for high-risk loans
        - Recall: The model was able to find 100% of healthy loans / 90% of high-risk loans

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?

        For the two models used, the Logistic Regression model slightly outperformed the Logistic Regression model, but not by much.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

        Performance depends on what we are trying to solve, which is which loans are high-risk. Because of this, the Logistic Regression model permformed better   
        because it was able to for 1% MORE of the high-risk loans.

If you do not recommend any of the models, please justify your reasoning.
