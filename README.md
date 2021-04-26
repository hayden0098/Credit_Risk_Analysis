# Credit_Risk_Analysis

## Overview of the analysis
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Also Personal lending is growing faster than credit card, auto, mortgage, and even student debt. With such incredible growth, FinTech firms are storming ahead of traditional loan processes. We'll need to employ different tenchnique to train and evaluate models with unbalanced classes, using imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. By using the latest machine learning techniques, these FinTech firms can continuously analyze large amounts of data and predict trends to optimize lending.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Each algotirhm will fit in logistic regression to evaulate the balanced accuracy score, generate the confusion matrix and classication report.

## Results:
Each Algorithms below fit in Logistic Regression model to train

Resampling Models Oversampling RandomOverSampler algorithms:
  * balanced accuracy scores = 0.6461
  * precision scores for high_risk = 0.01, low_risk = 1.00
  * recall scores for high_risk = 0.63, low_risk = 0.66

![RandomOverSampler](https://github.com/hayden0098/Credit_Risk_Analysis/blob/main/screen%20shot/RandomOverSampler.jpg)

Resampling Models Synthetic Minority Oversampling Technique(SMOTE) algorithm:
  * balanced accuracy scores = 0.6289
  * precision scores for high_risk = 0.01, low_risk = 1.00
  * recall scores for high_risk = 0.60, low_risk = 0.66

![SMOTE](https://github.com/hayden0098/Credit_Risk_Analysis/blob/main/screen%20shot/SMOTE.jpg)

Resampling Models Undersampling ClusterCentroids algorithms:
  * balanced accuracy scores = 0.5160
  * precision scores for high_risk = 0.01, low_risk = 1.00 
  * recall scores for high_risk = 0.60, low_risk = 0.43

![ClusterCentroids](https://github.com/hayden0098/Credit_Risk_Analysis/blob/main/screen%20shot/ClusterCentroids.jpg)

combinatorial approach of over- and undersampling SMOTEENN algorithms:
  * balanced accuracy scores = 0.6292
  * precision scores for high_risk = 0.01, low_risk = 1.00 
  * recall scores for high_risk = 0.72, low_risk = 0.53

![SMOTEENN](https://github.com/hayden0098/Credit_Risk_Analysis/blob/main/screen%20shot/SMOTEENN.jpg)

Ensemble Classifiers Balanced Random Forest Classifier algorithms:
  * balanced accuracy scores = 0.7871
  * precision scores for high_risk = 0.04, low_risk = 1.00 
  * recall scores for high_risk = 0.67, low_risk = 0.91 

![Balanced Random Forest Classifier](https://github.com/hayden0098/Credit_Risk_Analysis/blob/main/screen%20shot/Balanced%20Random%20Forest%20Classifier.jpg)

Ensemble Classifiers EasyEnsembleClassifier algorithms:
  * balanced accuracy scores = 0.9255
  * precision scores for high_risk = 0.07, low_risk = 1.00 
  * recall scores for high_risk = 0.91, low_risk = 0.94 

![EasyEnsembleClassifier](https://github.com/hayden0098/Credit_Risk_Analysis/blob/main/screen%20shot/EasyEnsembleClasskifier.jpg)

## Summary:
As the result, we run through all 6 machine learning models, the highest balanced accuracy scores is the Easy Ensemble Classifier algorithms, which gives us 0.9255 high score of accuracy. On the other hand the precision score that correctly predicted the high risk loan is 0.07, low risk loan is 1.00, the recall(sensitive) scores that correctly detect potential high rick loan is 0.91, low risk loan is 0.94. 

I would recommend to use the Easy Ensemble Classifier algorithms machine learning models. Although all 6 machine learning models can correctly predict the low credit risk loan, EasyEnsembleClassifier got the highest score overall at 0.07. Also other than it's come with the highest balanced accuracy scores, high recall(sensitive) scores tend to be more important when a person with high risk credit applying a loan and most of them were detacted correctly. 
