# FindDefault (Prediction of Credit Card fraud)

A credit card is one of the most used financial products to make online purchases and payments. 
Though the Credit cards can be a convenient way to manage your finances, they can also be risky. 
Credit card fraud is the unauthorized use of someone else's 
credit card or credit card information to make purchases or withdraw cash.

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Objective](#installation)
4. [Approach](#usage)

## Introduction

A credit card is one of the most used financial products to make online purchases and payments.
Though the Credit cards can be a convenient way to manage your finances, they can also be risky. 
Credit card fraud is the unauthorized use of someone else's credit card or credit card information to make purchases or withdraw cash.
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. 
The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
We have to build a classification model to predict whether a transaction is fraudulent or not.


## Features

The dataset contains 30 numerical features:
- **Time:** Seconds elapsed between each transaction and the first transaction.
- **V1 to V28:** Principal components obtained via PCA (to protect sensitive information).
- **Amount:** Transaction amount.
- **Class:** Target variable (0 = Legitimate, 1 = Fraudulent).

## Objective
The primary goal is to build a robust classification model capable of accurately predicting whether a transaction is fraudulent. The focus includes:
1. **Handling Imbalanced Data:** Developing strategies to deal with the skewed class distribution.
2. **Evaluation Metrics:** Prioritizing metrics like precision, recall, and F1-score over accuracy, given the imbalanced dataset.
3. **Model Performance:** Ensuring high performance to minimize false negatives (fraudulent transactions misclassified as legitimate).

## Approach
1. **Data Preprocessing:**
   - Normalize the `Amount` feature.
   - Handle the imbalanced dataset using techniques like undersampling, oversampling (e.g., SMOTE), or ensemble methods.
   
2. **Exploratory Data Analysis (EDA):**
   - Understand the distribution of legitimate and fraudulent transactions.
   - Analyze feature correlations and their importance.

3. **Model Selection:**
   - Train multiple models (e.g., Logistic Regression, Random Forest, Gradient Boosting) and compare performance.
   - Optimize hyperparameters for the best-performing model.

4. **Evaluation Metrics:**
   - Precision
   - Recall
   - F1-score
   - Area Under the ROC Curve (AUC-ROC)

5. ## Dependencies
    The following libraries are required:
    - Python 3.x
    - Pandas
    - NumPy
    - Scikit-learn
    - Matplotlib
    - Seaborn
    - Imbalanced-learn (for handling imbalanced datasets)

6. ## Requirement.txt
   The above dependencies libraries version mentioned in the Requirement.txt file

6. ## Results
    The final model will be evaluated on:
    - Its ability to detect fraudulent transactions.
    - Balancing false positives and false negatives.

7. ## Installation

    Explain the steps required to install the project. You may also include prerequisites and dependencies.
    ```bash

    # Clone the repository
    git clone https://github.com/jagbhomrah2006/Prediction-of-Credit-Card-fraud.git

    # Change to the project directory
    cd projectname
8. ## Usage // Will be add