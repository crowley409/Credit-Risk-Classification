# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

My analysis hoped to build machine learning models to predict credit risk based on historical lending data. The primary goal is to assess the credit worthiness of these loans by predicting if it is healthy or high risk. The CSV included various financial data points related to loan applications, with the loan_status variable set to 0 for healthy loans, and 1 for high risk loans. The machine learning process followed these steps:
  - Loaded the dataset and investigated its structure
  - Split the data into testing and training sets
  - Built logistic regression models with both the original data and resampled data
  - Evaluated the models using balanced accuracy score, confusion matrix, and precision, recall, and f1-score values

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

  * Balanced Accuracy Score: 0.9521352751368186
  * Confusion Matrix: 
  [[14926    75]
  [   46   461]]
  * Classification Report:                
                precision    recall  f1-score   support

           0       1.00      1.00      1.00     15001
           1       0.86      0.91      0.88       507

    accuracy                           0.99     15508
   macro avg       0.93      0.95      0.94     15508
weighted avg       0.99      0.99      0.99     15508




* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

  * Balanced Accuracy Score: 0.9941749445500477
  * Confusion Matrix: 
 [[14915    86]
 [    3   504]]
  * Classification Report:                
               precision    recall  f1-score   support

           0       1.00      0.99      1.00     15001
           1       0.85      0.99      0.92       507

    accuracy                           0.99     15508
   macro avg       0.93      0.99      0.96     15508
weighted avg       1.00      0.99      0.99     15508

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )


While model 1 performed strongly, I would recommend model 2 as the better one to use. Model 2 appears to outperform model 1 in terms of balanced accuracy and overall predictive capability. With that said, model 1 outperforms model 2 in precision, and if the cost of false positives is higher than the cost of false negatives for a certain business, they may choose to prioritize model 1. With that said, the precision scores are very close, and I believe model 2 performs the best. 