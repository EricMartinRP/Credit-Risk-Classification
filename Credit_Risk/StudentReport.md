# Module 12 Report Template

## Overview of the Analysis

Lending companies give loans to borrowers and want to minimize the risk of losing money. Credit Risk is the risk of borrowers not returning the money or assets. In this analysis, we used Machine Learning to analyze a dataset from a peer-to-peer lending company. The goal was to build a model that can determine the creditworthiness of borrowers.

## Results

We used the Logistic Regression Algorithm for our machine learning model because it is commonly used for classification problems. The model achieved an accuracy score of 95% but had a lower recall value (0.91) for non-healthy loans compared to healthy loans (0.99). This imbalance in the dataset affected the model's ability to predict non-healthy loans accurately.

To address this issue, we oversampled the data using the RandomOverSampler module from the imbalanced-learn library. This created a balanced dataset with an equal number of healthy and non-healthy loans. With the oversampled data, the Logistic Regression Model achieved an accuracy score of 99% and improved the recall value for non-healthy loans to 0.99.

## Summary

In summary, the Logistic Regression Model fitted with the oversampled data performed better than the model fitted with the imbalanced data. It had a higher accuracy score and recall value, indicating fewer mistakes in classifying non-healthy loans. This is important for a lending company to avoid misclassifying loans, which could lead to financial losses or customer dissatisfaction.

The lending company should prioritize minimizing false positives, as misclassifying non-healthy loans as healthy could result in the loss of funds. Based on the analysis, we recommend using Model 2, the Logistic Regression Model fitted with Balanced (oversampled) data.
