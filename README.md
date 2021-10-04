# Supervised Machine Learning Homework - Predicting Credit Risk

In this assignment, a machine learning model was built that attempts to predict whether a loan from LendingClub will become high risk or not. 

## Background

LendingClub is a peer-to-peer lending services company that allows individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. LendingClub offers their previous data through an API.

You will be using this data to create machine learning models to classify the risk level of given loans. Specifically, you will be comparing the Logistic Regression model and Random Forest Classifier.

## Instructions

### Retrieve the data
I used an entire year's worth of data (2019) to predict the credit risk of loans from the first quarter of the next year (2020).

Note: these two CSVs have been undersampled to give an even number of high risk and low risk loans. In the original dataset, only 2.2% of loans are categorized as high risk. To get a truly accurate model, special techniques need to be used on imbalanced data. Undersampling is one of those techniques. Oversampling and SMOTE (Synthetic Minority Over-sampling Technique) are other techniques that are also used.

## Preprocessing: Convert categorical data to numeric

A training set was created from the 2019 loans using `pd.get_dummies()` to convert the categorical data to numeric columns. Similarly, a testing set was created from the 2020 loans, also using `pd.get_dummies()`. 

## Consider the models

Two models were created with this data: a logistic regression, and a random forests classifier.

## Fit a LogisticRegression model and RandomForestClassifier model

A LogisticRegression model was created, fit to the data, and print the model's score. The same was done for a RandomForestClassifier.

## Revisit the Preprocessing: Scale the data

The data going into these models was never scaled, an important step in preprocessing. `StandardScaler` was used to scale the training and testing sets. 

### References

LendingClub (2019-2020) _Loan Stats_. Retrieved from: [https://resources.lendingclub.com/](https://resources.lendingclub.com/)

- - -

© 2021 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
