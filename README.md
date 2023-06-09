# Credit-Risk-Analysis

## Purpose

The purpose of this assignment is to apply machine learning techniques to solve a real-world problem, which is credit card risk. The credit risk is an inherently unbalanced classification problem because the good loans easily outnumber risky loans. Therefore, I will employ different techniques to train and evaluate models with unbalanced classes. We were required to use the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

I will use the credit card credit dataset from LendingClub, a peer-to-peer lending services company. I will oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I will use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I will compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Summary of Results

The random forest classifiers, with and without AdaBoost, were not able to produce accurate results in predicting bad loan applications. Similarly, oversampling and undersampling techniques did not yield a satisfactory model. The precision scores ranged from 0.01 to 0.09, indicating that only a small portion of flagged bad loan applications were actually bad, and the recall scores ranged from 0.61 to 0.92, indicating that the models could only detect a portion of the bad loans. The F1 scores were also low, ranging from 0.01 to 0.16, reflecting the trade-off between precision and recall. Despite using combination sampling, which resulted in a slightly higher recall score of 0.70, the overall performance of the models was inadequate for commercial use. Therefore, these models are not recommended for predicting bad loan applications.
