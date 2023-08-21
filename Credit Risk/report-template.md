# Module 12 Report Template

## Overview of the Analysis

In this analysis, we aimed to build machine learning models to assess credit risk for borrowers using historical lending activity data from a peer-to-peer lending services company. The purpose of this analysis was to develop models that can effectively predict the creditworthiness of borrowers and identify high-risk loans.

The dataset contained various financial features such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The target variable was the loan status, which was categorized as 0 for healthy loans and 1 for high-risk loans. The data was imbalanced, with a significantly larger number of healthy loans compared to high-risk loans.

The analysis was conducted in several stages:

Data Preparation: The dataset was split into training and testing sets. The labels (y) and features (X) were separated accordingly. The imbalance in the labels was observed, with a large number of healthy loans and fewer high-risk loans.
Modeling with Original Data: A logistic regression model was trained using the original training data. The model's performance was evaluated using balanced accuracy, confusion matrix, and classification report metrics. The model demonstrated high accuracy and precision for both classes.
Modeling with Resampled Data: To address the class imbalance, the training data was resampled using the RandomOverSampler. The logistic regression model was trained on the resampled data and evaluated using the same metrics. The resampled model exhibited even higher performance, with improved precision and recall for the high-risk class.
Summary and Comparison: The results of both models were summarized and compared to determine the best-performing approach for credit risk analysis.
## Results

Logistic Regression Model with Original Data:

Balanced Accuracy Score: 0.95
Precision and Recall Scores:
Class 0 (Healthy Loans):
Precision: 1.00
Recall: 0.99
Class 1 (High-Risk Loans):
Precision: 0.85
Recall: 0.91


Logistic Regression Model with Resampled Data:

Balanced Accuracy Score: 0.99
Precision and Recall Scores:
Class 0 (Healthy Loans):
Precision: 1.00
Recall: 0.99
Class 1 (High-Risk Loans):
Precision: 0.84
Recall: 0.99

## Summary
Based on the analysis results, both the logistic regression model with the original data and the model with the resampled data performed well in predicting credit risk. However, the model trained with the resampled data demonstrated slightly superior performance in terms of precision and recall for high-risk loans. While the original data model achieved an impressive accuracy score of 0.95, the resampled model achieved an outstanding balanced accuracy score of 0.99. The resampled model's ability to predict high-risk loans with higher precision and recall makes it the recommended choice for credit risk assessment.

The model's performance may depend on the specific problem we are trying to solve. For instance, if it is more critical to identify high-risk loans accurately, the model's ability to correctly predict class 1 (high-risk loans) becomes essential. Therefore, the resampled model's better performance in predicting class 1 loans is a crucial factor in the recommendation.

In conclusion, the logistic regression model trained with resampled data provides a robust solution for credit risk assessment, particularly due to its high precision and recall scores for high-risk loans. This model is recommended for use in identifying high-risk borrowers and supporting the decision-making process in lending services.