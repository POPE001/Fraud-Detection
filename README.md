
# Fraud Detection using RNN and Benchmark Models

## Overview

This project focuses on fraud detection using a Recurrent Neural Network (RNN) and benchmark machine learning models. The goal is to detect fraudulent activities in financial transactions by analyzing transaction data. The project preprocesses data, trains an RNN model, and compares its performance with benchmark models like Logistic Regression and Random Forest. 

The dataset used in this project contains transaction data with features such as 'step,' 'amount,' 'oldbalanceOrg,' 'newbalanceOrig,' 'oldbalanceDest,' and 'newbalanceDest.' The 'isFraud' column indicates whether a transaction is fraudulent or not.

## Table of Contents

- [Dataset Preprocessing](#dataset-preprocessing)
- [FraudDetectionRNN](#frauddetectionrnn)
- [Benchmark Models](#benchmark-models)
- [Evaluation](#evaluation)

## Dataset Preprocessing

The project starts with preprocessing the dataset, which involves:
- Loading and checking for missing values.
- Scaling the data using StandardScaler.
- Oversampling using RandomOverSampler to handle class imbalance.
- Splitting the dataset into training, validation, and test sets.

## FraudDetectionRNN

The RNN model used in this project is `FraudDetectionRNN`. It is a neural network with input size, hidden size, and the number of layers defined. The model architecture is as follows:
- Input layer
- LSTM layers
- Fully connected layers

## Benchmark Models

This project compares the RNN model with benchmark models, including:
- **Logistic Regression**: A simple and interpretable linear model.
- **Random Forest**: An ensemble learning model known for its versatility.

These models are trained and evaluated on the dataset for fraud detection.

## Evaluation

Evaluation metrics are used to assess model performance:
- **Accuracy**: Measures overall model accuracy.
- **Precision**: Quantifies the model's ability to correctly predict positive cases.
- **Recall**: Determines the proportion of actual positives correctly predicted.
- **F1-Score**: A combination of precision and recall, offering a balanced measure.
- **ROC AUC**: Measures the ability to distinguish between classes.

The project evaluates and compares the performance of the RNN model and benchmark models using these metrics.

## License

This project is licensed under the MIT License.
