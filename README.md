# Module 12 Report Template

## Overview of the Analysis

The goal of this analysis is to build a model that can identify the credit worthiness of borrowers.
This model was build on historical lending activity from a peer-to-peer lending services company. 
Because this model is to predict the credit worthiness of borrowers, we separated the column "loan status" from the rest of the data and saved them as individual variables.
To begin this process, we import the data from the original csv file and convert it into a Pandas DataFrame. 
We then create the labels for the DataFrames for the variables discussed above.
Our next step was to split the data into training and testing datasets by using train_test_split.

Now our dataset was ready to create a logistic regression model. 
To accomplish this, we first fit a logistic regression model by using the training data. 
Then we save the predictions on the testing data labels by using the testing feature data and the fitted model. 
To evaluate the model's performance, we generate a confusion matrix and print the classificaion report. 

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Logistic Regression
    - Accuracy: 99%
    - Precision: 
        - 0: 100%
        - 1: 87%
        - marco avg: 94%
        - weighted avg: 99%
    - Recall scores: 
        - 0: 100% 
        - 1: 95%
        - marco avg: 97%
        - weighted avg: 99%

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

This model has been very successful, with an accuracy score of 99%. Due to its high accuracy, I would reccomend its use moving forward. 


* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

First it is important to consider the distribution of the labels. Ensembles can be a good way to evaluate imbalanced data. Balanced data has more options to apply different machine learning models. Performance within different learning models can vary depending on the problem we are trying to solve and the makeup of the original dataset. 

If you do not recommend any of the models, please justify your reasoning.