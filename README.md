# Credit Card Fraud Detection

## Problem Statement

The rapid increase in online financial transactions has led to a corresponding rise in fraudulent activities, posing significant risks to both financial institutions and their customers. Detecting fraudulent transactions in real-time is a challenging task due to the complexity and diversity of fraud patterns. Traditional rule-based systems are often inadequate, resulting in high false positive rates, missed frauds, and increased operational costs.

## Objective

The primary objective of this machine learning project is to develop a predictive model that can accurately classify upcoming transactions as either fraudulent or genuine using supervised learning techniques. The model aims to enhance the security measures of financial systems by proactively identifying and mitigating fraudulent activities, thereby protecting both the organization and its customers from potential financial losses.

## Dataset

The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred over two days, including 492 frauds out of 284,807 transactions before removing duplicate transactions. The dataset is highly unbalanced, with the positive class (frauds) accounting for 0.172% of all transactions.

### Features

- **Time**: The seconds elapsed between each transaction and the first transaction in the dataset.
- **Amount**: The transaction amount, which can be used for example-dependent cost-sensitive learning.
- **V1, V2, ..., V28**: Principal components obtained with PCA (Principal Component Analysis).
- **Class**: The response variable, taking value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, it is recommended to measure accuracy using the Area Under the Precision-Recall Curve (AUPRC).

## Analysis

- **Logistic Regression** and **Gradient Boosting** both exhibit similar performance with high accuracy, precision, recall, F1-score, and ROC-AUC scores.
- **Random Forest** also performs well but has a slightly lower recall compared to Logistic Regression and Gradient Boosting.
- **Support Vector Machine (SVM)** shows significantly lower performance across all metrics.

## Conclusion

Logistic Regression and Gradient Boosting appear to be the best models based on the provided metrics. Both models have high accuracy, precision, recall, F1-score, and ROC-AUC scores, indicating they are good at correctly identifying both positive and negative classes and discriminating between them.

Since the metrics are nearly identical for Logistic Regression and Gradient Boosting, other factors such as model complexity and interpretability might be considered. Logistic Regression is simpler and more interpretable, while Gradient Boosting might capture more complex patterns at the cost of being more complex and potentially requiring more tuning and computational resources.

---
