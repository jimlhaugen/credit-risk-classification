# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results (Scores)

* Machine Learning Model 1 (Original Data):
  * Balanced Accuracy: 95.20%
  * Precision: 100% for "healthy loans"; 85% for "high-risk loans"
  * Recall: 99% for "healthy loans"; 91% for "high-risk loans"

* Machine Learning Model 2 (Resampled Training Data):
  * Balanced Accuracy: 99.37%
  * Precision: 100% for "healthy loans"; 84% for "high-risk loans"
  * Recall: 99% for "healthy loans"; 99% for "high-risk loans"

## Summary

For the logistic regression model fit with the original data, the balanced accuracy score of the model is 95.20%.  The precision scores of healthy and high-risk loans are 100% and 85%, respectively.  The recall scores of healthy and high-risk loans are 99% and 91%, respectively.  The f1-scores of healthy and high-risk loans are 100% and 88%, respectively,

For the logistic regression model fit with the oversampled data, the accuracy score of the model is nearly perfect at 99.37%.  The precision scores of healthy and high-risk loans are 100% and 84%, respectively, the latter being a slight decrease of 1%.  The recall scores of healthy and high-risk loans are 99% and 99%, respectively, the latter being a significant increase of 8%.  The f1-scores of healthy and high-risk loans are 100% and 91%, respectively, the latter being an increase of 3%.

In conclusion, it is recommended that the oversampled data should be employed (i.e., fitted) to logistic regression model for the following reasons:

Firstly, accuracy measures how many of the loans have been classified correctly, and 99.37% of the loans have been classified correctly with the oversampled data which is 4.17% better than using the original data.  

Secondly, precision scores measure how many of the loans of the model were predicted as healthy loans and how many were predicted as high-risk loans; although the use of the original data results with a better predictor of high-risk loans, its precision score is merely 1% better when oversampled data is used.  

Thirdly, recall measures how many of the loans of the model were correctly identified as healthy loans and how many were correctly identified as high-risk loans.  With the oversampled data, 99% of the loans were correctly identified as both healthy loans and high-risk loans.

Lastly, the f1-score is the harmonic mean of precision and recall, and higher f1-scores reflect a better balance between precision and recall.  When comparing the f1-scores with the two types of data, the higher f1-score of 91% for high-risk loans produced by the oversampled data reflects a better balance between the precision and recall scores than the f1-score of 88% produced by the original data. 

