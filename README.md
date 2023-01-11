# Credit_Risk_Analysis


## Overview of the analysis: 

It is a challenging problem to segregate good loans from risky/bad loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results: 

Naive Random Oversampling results: Our balanced accuracy test it 67%, the precision for the high_risk has a very low positivity at 1% and the recall is 74%

![ScreenShot](https://github.com/LIPSASHARMA/Credit_Risk_Analysis/blob/main/Starter_Code/Starter_Code/images/naive_random_sampling.png)

SMOTE oversampling results: the accuracy score is 66.2%, the precision for the high_risk loans has a low positvity again at 1% and recall is 69% overall

![ScreenShot](https://github.com/LIPSASHARMA/Credit_Risk_Analysis/blob/main/Starter_Code/Starter_Code/images/smote_over_sampling.png)

Undersampling results: balanced accuracy score is 66.2% overall, the precision is at 99% and the recall is 41%

![ScreenShot](https://github.com/LIPSASHARMA/Credit_Risk_Analysis/blob/main/Starter_Code/Starter_Code/images/under_sampling.png)

Combination(over and undersampling) results: balanced accuracy score is 54.7% the precision is 99% and the recall is 57% overall

![ScreenShot](https://github.com/LIPSASHARMA/Credit_Risk_Analysis/blob/main/Starter_Code/Starter_Code/images/combination_over_under_sampling.png)

Balanced Random Forest Classifier results: the accuracy score is 77.2% the precision is 99% and the recall is 88%

![ScreenShot](https://github.com/LIPSASHARMA/Credit_Risk_Analysis/blob/main/Starter_Code/Starter_Code/images/balanced_random_forest_classifier.png)

Easy Ensemble AdaBoost Classifier results: the accuracy score is 91.7% the precision is 99% and the recall is 94%

![ScreenShot](https://github.com/LIPSASHARMA/Credit_Risk_Analysis/blob/main/Starter_Code/Starter_Code/images/easy_ensemble_classifier.png)



## Summary: 

We tried to predict credit risk of various types of loans. We had a low accuracy score in the first 4 models when we compare it with the ensamble classifiers. There is a low score in oversampling and mixed models as well. Hence, we observe that Ensemble classifiers give better accuracy scores during the first 4 models. 