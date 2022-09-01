# Module 12 Report Template

## Overview of the Analysis
  This analysis takes a closer look at credit risk metrics to try and predict the creditworthiness of borrowers. Using ML models we will try and predict whether a borrower is likely a 'healthy loan' or 'high-risk loan' using a dataset of historical lending activity from a peer-to-peer lending services company.

  First, we preprocess the data by seperating the features and the labels to be used in the model. To check the balance of the target values, we use the value counts function on the Y variable. There is a heavy imbalance on the Y variable in the original data frame with 75,036 Healthy Loans and 2,500 High-risk Loans. Next, we train the model on the original data and make our predictions on the testing features.

  In the second model, we use the original preprocessed data and resample the data using the Random Over Sampler model. The model balances the Y variable so we have have an equal number of Healthy Loans and High-Risk Loans to train on. 

## Results
* Machine Learning Model 1:
  * Balanced Accuracy Score: .952
  * Precision Score 'Healthy Loans': 1.00
  * Precision Score 'High-risk Loans': .85
  * Recall Score 'Healthy Loans': .99
  * Recall Score 'High-risk Loans': .91

* Machine Learning Model 2:
  * Balanced Accuracy Score: .995
  * Precision Score 'Healthy Loans': .99
  * Precision Score 'High-risk Loans': .99
  * Recall Score 'Healthy Loans': .99
  * Recall Score 'High-risk Loans': .99

## Summary
The results of the machine learning models tell us that the model improved after resampling. We should use model 2 to predict the creditworthiness of buyers because the recall and precision scores on the second model improved to .99 for predicting the High-risk loans. If we were trying to predict the Healthy Loans, we should use model 1 as it has a 1.00 for the precision score and .99 recall. 
