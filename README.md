# Module 12 Report Template

## Overview of the Analysis

In this analysis, we aimed to develop a machine learning model to predict the loan status of borrowers. The purpose of this analysis was to determine the likelihood of a loan being classified as a high-risk loan (`1`) or a healthy loan (`0`). The financial data provided included various attributes such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The target variable to predict was `loan_status`.

The data analysis process involved the following stages:
1. **Data Loading**: Reading the data from a CSV file into a Pandas DataFrame.
2. **Data Preparation**: Separating the features (`X`) from the target variable (`y`).
3. **Data Splitting**: Dividing the data into training and testing sets using `train_test_split`.
4. **Model Training**: Training a Logistic Regression model on the training data.
5. **Model Evaluation**: Making predictions on the testing data and evaluating the model's performance using confusion matrix and classification report.

The machine learning process used the `LogisticRegression` algorithm to create the predictive model.

## Results

* **Logistic Regression Model**:
    * **Accuracy**: 99%
    * **Precision**:
        * For label `0` (healthy loan): 1.00
        * For label `1` (high-risk loan): 0.86
    * **Recall**:
        * For label `0` (healthy loan): 0.99
        * For label `1` (high-risk loan): 0.94
    * **F1-score**:
        * For label `0` (healthy loan): 1.00
        * For label `1` (high-risk loan): 0.90

## Summary

The Logistic Regression model demonstrated excellent performance in predicting both healthy and high-risk loans, with an overall accuracy of 99%. The precision, recall, and F1-scores for healthy loans were near-perfect, indicating that the model is highly effective at identifying healthy loans. For high-risk loans, the model also performed well, though with slightly lower precision (0.86) and F1-score (0.90), but still maintaining high recall (0.94).

Given the results, the Logistic Regression model is recommended for predicting loan status due to its high accuracy and balanced performance across both classes. The model's performance is particularly important in financial contexts where accurately identifying high-risk loans is crucial. Therefore, while the model performs exceptionally well overall, its strong recall for high-risk loans ensures that it is effective in identifying most high-risk cases, which is often a critical requirement in financial risk assessment.

Overall, the Logistic Regression model is the best-performing model for this analysis, providing reliable predictions for loan statuses.
