# Credit_Risk_Analysis

## Overview

The purpose of this project is to user machine learning to predict credit risk. To achieve this, we will be using the following six machine learning models:

- Oversampling (Random Oversampler and SMOTE)
- Undersampling (Cluster Centroids)
- Combination (Over and Under) Sampling
- Balanced Random Forest Classifier
- Easy Ensemble Classifier


## Results

Our analysis produced the following results:

### Oversampling

#### Random Oversampler

Accuracy Score: 0.648072305476572

Confusion Matrix

![random_over_cm](/resources/random_over_cm.PNG)

Imbalanced Classification Report

![random_over](/resources/random_over.PNG)

#### SMOTE

Accuracy Score: 0.6625695222702812

Confusion Matrix

![smote_cm](/resources/smote_cm.PNG)

Imbalanced Classification Report

![smote_over](/resources/smote_over.PNG)

### Undersampling

#### Cluster Centroids

Accuracy Score: 0.5442661782548694

Confusion Matrix

![under_cm](/resources/under_cm.PNG)

Imbalanced Classification Report

![under](/resources/under.PNG)

### Combination (Over and Under) Sampling

Accuracy Score: 0.6639481008437607

Confusion Matrix

![combo_cm](/resources/combo_cm.PNG)

Imbalanced Classification Report

![combo](/resources/combo.PNG)

### Balanced Random Forest Classifier

Accuracy Score: 0.7885466545953005

Confusion Matrix

![brf_cm](/resources/brf_cm.PNG)

Imbalanced Classification Report

![brf](/resources/brf.PNG)

### Easy Ensemble Classifier

Confusion Matrix

Accuracy Score: 0.9316600714093861

![ee_cm](/resources/ee_cm.PNG)

Imbalanced Classification Report

![ee](/resources/ee.PNG)

## Summary

Of the six models, the Easy Ensemble Classifier option produced the highest accuracy score. This model also has a perfect precision score for low risk applications, along with high recall and F1 scores. However, we have significantly low precision and F1 scores, and a high recall score, which means that this model will have a large number of false positives and a low number of false negatives. 

Since nearly all applications that are actually high risk are being classified as high risk, additional testing will be required to address the large amount of large positives in this class. If resources are available to perform additional testing, then I would recommend  going forward with the Easy Ensemble Classifier model.
