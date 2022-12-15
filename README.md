# Credit_Risk_Analysis

## Overview of the analysis: 

In this analysis we are using machine learning to evaluate credit risk based on a series of data provided. We rely on multiple methods to produce our models. We address issues of oversampling and under sampling to ensure that we get our most accurate results. For this analysis we find that having a precise search is a safer bet as a bank because having too many defaults could lead to bankruptcy of the bank if too many bad loans are given out. We used six different under sample and oversampling algorithms to reduce as much bias as possible. We used RandomOverSampler and SMOTE to oversample the data, and ClusterCentroids to undersample the data. SMOTEENN was then later used to combine both. To combat bias we used BalancedRandomForestClassifier and EastEnsembleClassifier.

## Results:

### RandomOverSampler:
  - accuracy score: 0.64
  - precision score: 1.0
  - recall score: 0.66
  
![Oversampling](https://github.com/Hamza97anh/Credit_Risk_Analysis/blob/c10c627a96d3ca71231e6668bde4644419afc079/Images/Oversampling.PNG)

### SMOTE:
  - accuracy score: 0.615
  - precision score: 1.0
  - recall score: 0.59
  
![SMOTE](https://github.com/Hamza97anh/Credit_Risk_Analysis/blob/c10c627a96d3ca71231e6668bde4644419afc079/Images/SMOTE.PNG)

### Undersampling:
  - accuracy score: 0.52
  - precision score: 1.0
  - recall score: 0.43
  
![Undersampling](https://github.com/Hamza97anh/Credit_Risk_Analysis/blob/c10c627a96d3ca71231e6668bde4644419afc079/Images/Undersampling.PNG)


### SMOTEENN:
  - accuracy score: 0.65
  - precision score: 1.0
  - recall score: 0.59
  
![Combination Sampling.](https://github.com/Hamza97anh/Credit_Risk_Analysis/blob/c10c627a96d3ca71231e6668bde4644419afc079/Images/Undersampling.PNG)

### BalancedRandomForestClassifier:
  - accuracy score: 0.795
  - precision score: 1.0
  - recall score: 0.9
  
![Ensemble Learners](https://github.com/Hamza97anh/Credit_Risk_Analysis/blob/c10c627a96d3ca71231e6668bde4644419afc079/Images/Ensemble%20Learners.PNG)

### EasyEnsembleClassifier:
  - accuracy score: 0.925
  - precision score: 1.0
  - recall score: 0.94
  
![Easy Ensemble AdaBoost Classifier](https://github.com/Hamza97anh/Credit_Risk_Analysis/blob/c10c627a96d3ca71231e6668bde4644419afc079/Images/Easy%20Ensemble%20AdaBoost%20Classifier.PNG)

## Summary
Based on our results we see that every model has a precision scroe of 1. However our highest scorers were  Easy Ensemble Classifier at 0.925 and Balanced Random Forest Classifier at 0.795. Our lowest score was 0.52 when we used our undersampling method which is not a surprise as undersampling trims the data down to where almost both outcomes are equal in the data. The highest outcomes were the ones that are designed to reduce bias. I would air on the side of caution and avoid using Easy Ensemble Classifier at that 0.925 accuracy as it can be harder to interpert and since it's so much higher than the other results. Balanced Random Forest Classifier is easier to interpert and brings a more beliveable result at 0.795 and it still has a very comparable recall score to Easy Ensemble Classifier at 0.9 vs the 0.94. It's also the easiest to interpret.  



