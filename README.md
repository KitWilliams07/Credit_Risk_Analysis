# Credit_Risk_Analysis


## Overview of the Analysis

The purpose of this Analysis is to take credit card data and apply various Supervised Machine Learning algorithms and techniques in order to determine credit card fraud. A few metrics for each algorithm will be calculated (accuracy, confusion matrix, classification report) in order to determine which algorithm serves as the best predictor for credit card fraud.

Credit Card Fraud data is an inherently unbalanced classification problem, as good loans far out number risky ones. As a result, need to apply different techniques in order to solve credit fraud using machine learning. These include using unbalanced ML libraries or resampling the data, by oversampling, undersampling, or SMOTEENN algorithm. For this analysis we will use resampling in order to train and evaluate our models. 


PART 1: 
The following resamplings were preformed on the credit card data...

Naive Over-Sampling (Random Over Sampling)
SMOTE Over-Sampling 
Centroid Clusters Under-Sampling
SMOTEENN (Combination of Over and Under Sampling)

Each resampled data was then used to train a Logistic Regression Supervised ML algorithm. The algorithm was then used to make predictions on credit card fraud. The accuracy, confusion matrix, and classification report were displayed for each resampling. 


PART 2:
The credit card data was then applied to a few ensemble learning ML algorithms...

Balanced Random Forest Classifier
Easy Ensemble AdaBoost Classifier 

These algorithms were then used to make predictions on credit card fraud. The accuracy, confusion matrix, and classification report were displayed for both. 

## Results

The metrics for all 6 Machine Learning Models are displayed below...


PART 1:

Naive Over-Sampling + Logisitic Regression:
Accuracy: 67.9%
Confusion Matrix:
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cm_naive.png)

Classification Report:
![alt text](https://raw.githubusercontent.com/KitWilliams07/Amazon_Vine_Analysis/main/Challenge/y.png)

Precision: 99%
Recall: 68%


SMOTE Over-Sampling + Logistic Regression:
Accuracy: 65.6%
Confusion Matrix:
![alt text](https://raw.githubusercontent.com/KitWilliams07/Amazon_Vine_Analysis/main/Challenge/y.png)

Classifiction Report:
![alt text](https://raw.githubusercontent.com/KitWilliams07/Amazon_Vine_Analysis/main/Challenge/y.png)

Precision: 99%
Recall: 66%


Centroid Clusters Under-Sampling + Logistic Regression:
Accuracy: 45%
Confusion Matrix:
![alt text](https://raw.githubusercontent.com/KitWilliams07/Amazon_Vine_Analysis/main/Challenge/y.png)

Classification Report:
![alt text](https://raw.githubusercontent.com/KitWilliams07/Amazon_Vine_Analysis/main/Challenge/y.png)

Precision: 99%
Recall: 45%



SMOTEEN Over and Under Sampling + Logistic Regression:
Accuracy: 57.1%
Confusion Matrix: 
![alt text](https://raw.githubusercontent.com/KitWilliams07/Amazon_Vine_Analysis/main/Challenge/y.png)

Classification Report:
![alt text](https://raw.githubusercontent.com/KitWilliams07/Amazon_Vine_Analysis/main/Challenge/y.png)

Precision: 99%
Recall: 57%



PART 2:

Balanced Random Forest Classifier:
Accuracy: 80.1%
Confusion Matrix: 
![alt text](https://raw.githubusercontent.com/KitWilliams07/Amazon_Vine_Analysis/main/Challenge/y.png)

Classification Report: 
![alt text](https://raw.githubusercontent.com/KitWilliams07/Amazon_Vine_Analysis/main/Challenge/y.png)

Precision: 99%
Recall: 90%



Easy Ensemble AdaBoost Classifier:
Accuracy: 92.6%
Confusion Matrix:
![alt text](https://raw.githubusercontent.com/KitWilliams07/Amazon_Vine_Analysis/main/Challenge/y.png)

Classification Report:
![alt text](https://raw.githubusercontent.com/KitWilliams07/Amazon_Vine_Analysis/main/Challenge/y.png)

Precision: 99%
Recall: 94%


## Summary

