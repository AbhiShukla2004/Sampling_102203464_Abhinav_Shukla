# Overview

Detecting fraudulent transactions in credit card data is a complex challenge due to the significant class imbalance present in transaction datasets. Such imbalances can adversely impact the performance of machine learning models. This project aims to address these challenges by:

1. Mitigating class imbalance using the Synthetic Minority Oversampling Technique (SMOTE).
2. Creating five samples of different sizes through various sampling strategies.
3. Training and testing five machine learning algorithms on the sampled datasets.
4. Evaluating and comparing the performance of these models to identify the most suitable sampling technique for each.

# Dataset

The dataset, Creditcard_data.csv (provided for this project), contains the following attributes:

1. Features (V1 to V28): Principal components derived from the original transaction data.
2. Time: The time elapsed in seconds between consecutive transactions.
3. Amount: The value of the transaction.
4. Class: The target variable, where 0 denotes legitimate transactions and 1 indicates fraudulent ones.

## Class Imbalance

The dataset exhibits a significant class imbalance, with the following distribution:

1. Class 0 (Legitimate Transactions): Constituting 98.83% of the dataset.
2. Class 1 (Fraudulent Transactions): Making up only 1.17% of the dataset.

# Sampling Techniques

To address the class imbalance, the following sampling methods were applied:

1. Random Sampling: Arbitrarily selects a subset of records.

2. Stratified Sampling: Ensures the class proportions are maintained in the sampled dataset.

3. Systematic Sampling: Selects every nth record from the dataset.

4. Cluster Sampling: Divides the dataset into clusters and uses entire clusters for analysis.
5. Oversampling: Balances the dataset by increasing the representation of the minority class.

# Machine Learning Models

The project evaluated the following machine learning algorithms:

1. Logistic Regression

2. Gradient Boosting Classifier

3. Random Forest Classifier

4. Support Vector Machine (SVM)

5. K-Nearest Neighbors (KNN)

# Observations

Logistic Regression: Performed optimally with data generated through Stratified Sampling and Oversampling.

Gradient Boosting: Delivered the highest accuracy when trained on Stratified Sampling data.

Random Forest: Achieved its best performance using Oversampled datasets.

SVM: Showed superior results with Oversampled datasets.

K-Nearest Neighbors: Demonstrated optimal performance with Stratified Sampling.
