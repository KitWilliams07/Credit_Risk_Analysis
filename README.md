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

Naive Over-Sampling + Logisitic Regression: <br/>
Accuracy: 67.9% <br/>
Confusion Matrix: <br/>
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cm_naive.png)

Classification Report: <br/>
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cr_naive.png)

Precision: 99% <br/>
Recall: 68%


SMOTE Over-Sampling + Logistic Regression: <br/>
Accuracy: 65.6% <br/>
Confusion Matrix: <br/>
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cm_smote.png)

Classifiction Report: <br/>
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cr_smote.png)

Precision: 99% <br/>
Recall: 66%


Centroid Clusters Under-Sampling + Logistic Regression: <br/>
Accuracy: 45% <br/>
Confusion Matrix: <br/>
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cm_centroid.png)

Classification Report: <br/>
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cr_centroid.png)

Precision: 99% <br/>
Recall: 45%



SMOTEENN Over and Under Sampling + Logistic Regression: <br/>
Accuracy: 57.1% <br/>
Confusion Matrix: <br/>
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cm_smoteenn.png)

Classification Report: <br/>
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cr_smoteenn.png)

Precision: 99% <br/>
Recall: 57%



PART 2:

Balanced Random Forest Classifier: <br/>
Accuracy: 80.1% <br/>
Confusion Matrix: <br/>
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cm_brf.png)

Classification Report: <br/>
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cr_brf.png)

Precision: 99% <br/>
Recall: 90%



Easy Ensemble AdaBoost Classifier: <br/>
Accuracy: 92.6% <br/>
Confusion Matrix: <br/>
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cm_easy.png)

Classification Report: <br/>
![alt text](https://raw.githubusercontent.com/KitWilliams07/Credit_Risk_Analysis/main/Resources/cr_easy.png)

Precision: 99% <br/>
Recall: 94%


## Summary

From the results, the most glaring outcomes are the success of the ensemble learning algorithms. The Balanced Random Forest had an accuracy of 80.1% and Recall of 90% while the Easy Ensemble had an accuracy of 92.6% and Recall of 94%.

The other algorithms that resampled the data and applied the Logistic Regression model preformed much worse. Their accuracies ranged from 45% to 67.9% and recalls that ranged from 45% to 68%. Since these models preformed significantly worse than the ensemble algorithms I would not recommend any of these.

With that being said I still would NOT recommend the ensemble algorithms either. The glaring issue with these models is best seen in the confusion matrices. The Balanced Random Forest Classifier had 1694 False Negatives and the Easy Ensemble Model had 957 False Negatives. False Negatives means that the algorithm predicted the credit loan was low risk when in reality it was high risk. Considering this data set is out 17,205 that means that a large portion of these credit card loans would be given to "high risk" accounts on the basis that the model thinks they are actually "low risk" accounts. Credit Card Companies would want to avoid this scenario which is why I wouldn't recommend any of these models. 

