# Challenge20_CreditRiskClassification
 
## Overview of the Analysis

* In this Challenge, we used various techniques to train and evaluate models with imbalanced classes. We used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

* This challenge consists of the following subsections:
* Split the Data into Training and Testing Sets
* Create a Logistic Regression Model with the Original Data
* Predict a Logistic Regression Model with Resampled Training Data

## Results

* Machine Learning Model 1:
  If we look at the balanced accuracy score-95%, the logistic regression model works well. However, if we look at the imbalanced classification report, the model predicted healthy loans 100% of the time and predicted non-healthy loans 85% of the time. This could also be verified by the confusion matrix. The number of healthy loans highly outweighs the number of non-healthy loans indicating that the model would predict healthy loans better than being able to predict non-healthy loans.


* Machine Learning Model 2:
  If we look at the balanced_accuracy_score of the oversampled model, it is 99%, which turned out to be higher than the model fitted with imbalanced data. The recall score for non-healthy loans of imbalanced model was .91, which is also lower than the oversampled model of 0.99, which indicating the oversampled model performs better because it more likely to exclude posssibilities of labeling non-healthy loans as healthy loans.


## Summary

Overall, the oversampled model performs better because it does a exceptional job in catching mistakes such as labeling non-healthy loans as healthy. A lending company may need a model with higher recall, which means non-healthy loans is more likely to be identified to avoid further loss or future costs.

