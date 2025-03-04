# Module 12 Report Template

## Overview of the Analysis
---
This analysis aims to develop and evaluate a data model that predicts the creditworthiness of potential borrowers on peer-to-peer lending platforms. By assessing the likelihood of loan repayment, the model helps lenders make informed decisions and reduce financial risks. The feature set for this analysis included loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The model was designed to predict loan status, where 0 indicates a Healthy Loan and 1 signifies a High-Risk Loan.

To evaluate the model, the dataset was split into training and testing sets for both the feature set (X) and the label set (y). A Logistic Regression classifier was then created and trained using the X and y training data. Once trained, the classifier was used to predict loan status based on the X testing data.

## Results
---
Classification Report Scores:

    * Precision:
      * Healthy Loan: 100%
      * High-Risk Loan: 84%
      
     * Recall:
      * Healthy Loan: 99%
      * High-Risk Loan: 99%
      
    * Overall Accuracy: 99%

## Summary
--- 
Based on the results, the Logistic Regression model performs exceptionally well, achieving an overall accuracy of 99%. The Logistic Regression model demonstrates strong performance with 100% precision for healthy loans and 84% precision for high-risk loans. 

If the primary goal is to minimize financial risk, predicting high-risk loans (1s) accurately is more critical. In this case, the model’s 84% precision for high-risk loans suggests that some healthy loans may be misclassified as high-risk, leading to unnecessary loan rejections. However, the high 99% recall for high-risk loans ensures that nearly all actual high-risk loans are correctly identified, reducing the chance of approving risky borrowers.

This model is highly effective for predicting healthy loans, but if minimizing false positives (incorrectly predicting high-risk loans) is a priority, further tuning may be required.
