# Credit-Card-Fraud-Detection-Using-DataScience-Machine-Learning

# Fraud Detection using Machine Learning and SMOTE

This repository contains a fraud detection project that aims to detect fraudulent credit card transactions using machine learning techniques. The dataset used for this project is imbalanced, with a majority of non-fraudulent transactions and a small number of fraudulent transactions. To tackle this imbalance, the Synthetic Minority Over-sampling Technique (SMOTE) is used to create synthetic samples of the minority class, making the dataset balanced.

## Data Overview
The dataset contains information about credit card transactions, including various features and a binary label indicating whether the transaction is fraudulent (1) or not (0).

## Project Overview
The project is structured as follows:

1. Data Preprocessing: Data is cleaned, outliers are removed, and features are scaled as necessary.

2. Exploratory Data Analysis (EDA): Exploring the distribution of classes, correlations, and important insights from the data.

3. Model Building:
   - Logistic Regression: A logistic regression model is trained on the original imbalanced data as a baseline.
   - Logistic Regression with Random Under-Sampling: A logistic regression model is trained on the randomly under-sampled data.
   - Logistic Regression with SMOTE: A logistic regression model is trained on the SMOTE-sampled data.

4. Model Evaluation:
   - ROC Curves: ROC curves are plotted for each model to visualize their performance.
   - Precision-Recall Curves: Precision-recall curves are plotted to evaluate model performance on the positive class (fraud detection).
   - Confusion Matrix: Confusion matrices are generated to show the model's predictions on the test set.

## Model Performance
The model performance on the test set is summarized below:

- Logistic Regression (Original Data):
  - Accuracy: 0.47
  - Precision: 0.00
  - Recall: 0.50
  - F1 Score: 0.00

- Logistic Regression with Random Under-Sampling:
  - Accuracy: 0.96
  - Precision: 0.96
  - Recall: 0.96
  - F1 Score: 0.96

- Logistic Regression with SMOTE:
  - Accuracy: 0.97
  - Precision: 0.06
  - Recall: 0.90
  - F1 Score: 0.11

## Conclusion
The use of SMOTE significantly improved the performance of the logistic regression model for fraud detection. The model achieved a high recall rate of 90% for detecting fraudulent transactions, which is crucial for this type of application. However, the precision of the model remains low at 6%, indicating a higher number of false positives. This trade-off between precision and recall should be considered based on the specific use case and the impact of false positives and false negatives.

In future work, additional machine learning models and advanced techniques can be explored to further enhance the fraud detection capabilities and improve precision-recall trade-offs. Additionally, hyperparameter tuning and feature engineering may help in achieving even better results.
