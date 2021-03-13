# Credit_Risk_Analysis

## Overview of the Analysis

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, an analysis is performed to predict credit card risk using machine learning methods. The following techniques to train and evaluate models are used:

* Imbalanced-learn and scikit-learn libraries in order to build and evaluate models using resampling.
* Oversampling the data using the RandomOverSampler and SMOTE algorithms.
* Undersampling the data using the ClusterCentroids algorithm.
* Combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
* Comparing two machine learning models, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risks.

## Results
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

### Model 1: Naive Random Oversampling

![naive_random_oversampling](https://github.com/Lora-Borja/Credit_Risk_Analysis/blob/main/images/naive_random_oversampling.PNG)

* Using the naive random oversampling model resulted in a balanced accuracy score of 0.64
* High risk credit applications resulted in a precision score of 0.01 and a recall score of 0.62
* Low risk credit applications resulted in a precision score of 1.00 and a recall score of 0.67

### Model 2: SMOTE Oversampling

![SMOTE_oversampling](https://github.com/Lora-Borja/Credit_Risk_Analysis/blob/main/images/SMOTE_oversampling.PNG)

* Using the SMOTE model resulted in a balanced accuracy score of 0.65
* High risk credit applications resulted in a precision score of 0.01 and a recall score of 0.66
* Low risk credit applications resulted in a precision score of 1.00 and a recall score of 0.64

### Model 3: Undersampling via Cluster Centroids Algorithm

![clustercentroids_undersampling](https://github.com/Lora-Borja/Credit_Risk_Analysis/blob/main/images/clustercentroids_undersampling.PNG)

* Using the Undersampling model resulted in a balanced accuracy score of 0.51
* High risk credit applications resulted in a precision score of 0.01 and a recall score of 0.60
* Low risk credit applications resulted in a precision score of 1.00 and a recall score of 0.43

### Model 4: SMOTEENN Combo Sampling

![SMOTEENN_combosampling](https://github.com/Lora-Borja/Credit_Risk_Analysis/blob/main/images/SMOTEENN_combosampling.PNG)

* Using the SMOTEENN model resulted in a balanced accuracy score of 0.62
* High risk credit applications resulted in a precision score of 0.01 and a recall score of 0.71
* Low risk credit applications resulted in a precision score of 1.00 and a recall score of 0.55

### Model 5: Balanced Random Forest Classifier

![BRF_classifier](https://github.com/Lora-Borja/Credit_Risk_Analysis/blob/main/images/BRF_classifier.PNG)

* Using the Balanced Random Forest Classifier model resulted in a balanced accuracy score of 0.78
* High risk credit applications resulted in a precision score of 0.03 and a recall score of 0.70
* Low risk credit applications resulted in a precision score of 1.00 and a recall score of 0.87

### Model 6: Easy Ensemble AdaBoost Classifier

![EE_classifier](https://github.com/Lora-Borja/Credit_Risk_Analysis/blob/main/images/EE_classifier.PNG)

* Using the Easy Ensemble Classifier model resulted in a balanced accuracy score of 0.93
* High risk credit applications resulted in a precision score of 0.09 and a recall score of 0.92
* Low risk credit applications resulted in a precision score of 1.00 and a recall score of 0.94


## Summary
Based on the analysis results of the various models, the recommendation is to use the Easy Ensemble AdaBoost Classifier as it seems to be the best method to predict credit risks having the highest accuracy score of 0.93. It is somewhat concerning that both high and low risk applications also have a high recall score. Therefore, it may mean that the applications will need further investigations before approving them.
