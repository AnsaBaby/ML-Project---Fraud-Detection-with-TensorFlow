# Fraud Detection Using Neural Networks
## Project Overview
Fraud detection in financial transactions is critical in the banking and finance sectors. This project demonstrates how to build a deep learning model using TensorFlow to detect fraudulent transactions based on the publicly available "Credit Card Fraud Detection" dataset. The dataset contains anonymized transaction data and aims to classify transactions as fraudulent (Class 1) or non-fraudulent (Class 0).
This article walks you through setting up the environment, loading the dataset, performing exploratory data analysis, cleaning the data, building and training a neural network model, and evaluating its performance.

### Environment Setup
To begin, install the required libraries to handle data manipulation, visualization, and machine learning model creation.

## Data Loading and Exploratory Analysis
The dataset for this project can be found here. It contains 284,807 transactions, including 31 features. The target column Class indicates whether the transaction is fraudulent (1) or not (0).

## Data Cleaning
Check for missing values and duplicates in the dataset. Since there are no missing values, I remove the duplicate entries.

### Feature Selection and Scaling
I'll exclude the Time feature and separate the target variable Class from the features. I then split the dataset into training and test sets.

## Model Building
I build a neural network with three dense layers:

The first layer has 64 neurons with a ReLU activation function.
The second layer has 32 neurons and includes dropout for regularization.
The final layer outputs a probability score using the sigmoid activation function.

### Train the Model
Now, train the model using the training data

## Model Evaluation
After training, I evaluate the model’s performance using a confusion matrix and classification reports.

## Conclusion
This project demonstrates how to use a neural network to detect fraud in credit card transactions. The imbalance in the dataset posed challenges, but the model can be improved with techniques like under sampling, oversampling, or using advanced architectures like autoencoders.
