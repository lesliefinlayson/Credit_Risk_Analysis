# Credit_Risk_Analysis

## Project Purpose

Determining credit risk presents a challenge because it is an unbalanced classification problem: the number of good loans highly outnumber the number of risky loans.  The results, therefore, may be skewed and using standard metrics can lead to classification errors and misleading conclusions.

The purpose of this project is to evaluate 6 different machine learning models to determine which, if any, can be used to predict credit risk.  These include resampling models, combination sampling, and ensemble classifiers.

## Results

### Resampling Models

_Oversampling with RandomOverSampler_ 

In random oversampling, instances of the minority class are randomly selected and added to the training set until the majority and minority classes are balanced. 

Balanced Accuracy Score:

<img width="331" alt="2021-10-16 (2)" src="https://user-images.githubusercontent.com/84471904/137592243-a261fe65-b285-4f25-995d-f5936d829dac.png">

Imbalanced classification Report:

<img width="374" alt="2021-10-16 (3)" src="https://user-images.githubusercontent.com/84471904/137592297-e82c3d82-143b-4e07-ad8e-ec8212d13579.png">

_Oversampling with SMOTE_ 

With SMOTE, new instances of the minority class are interpolated and added to the training set until the majority and minority classes are balanced. 

Balanced Accuracy Score:

<img width="238" alt="2021-10-16 (4)" src="https://user-images.githubusercontent.com/84471904/137593307-e819a34b-5b5c-46cf-b00d-1f78c0cfad47.png">

Imbalanced classification Report:

<img width="383" alt="2021-10-16 (5)" src="https://user-images.githubusercontent.com/84471904/137593386-a2fad91f-cf98-446d-ab10-2687d8c1c783.png">

_Undersampling with the ClusterCentroids resampler_ 

This algorithm identifies clusters of the majority class then generates synthetic data points that are representiatve of the clusters.  The majority class is then undersampled down to the size of the minority class.   

Balanced Accuracy Score:

<img width="246" alt="2021-10-16 (7)" src="https://user-images.githubusercontent.com/84471904/137594773-2dde37db-ee67-48e9-aeb7-3076a7824564.png">

Imbalanced classification Report:

<img width="374" alt="2021-10-16 (8)" src="https://user-images.githubusercontent.com/84471904/137594806-0735645e-f0db-453c-ab12-46a3f141b7bb.png">

### Combination Sampling

_Combination Sampling with SMOTEEN_ 

This sampling strategy combines oversampling the minority class with SMOTE and undersampling by dropping data points that have neighbors belonging to two different classes.

Balanced Accuracy Score:

<img width="256" alt="2021-10-16 (10)" src="https://user-images.githubusercontent.com/84471904/137595116-cd6e8f99-67c5-45f9-b1ea-fbfc1a22a176.png">

Imbalanced classification Report:

<img width="370" alt="2021-10-16 (11)" src="https://user-images.githubusercontent.com/84471904/137595174-f68e8091-b479-401d-bd9a-4d342e9cd9e2.png">

### Ensemble Learners

_Balanced Random Forest Classifier_ 

This supervised learning algorith builds a "forest" - where for each tree two bootstrapped sets of the same size, equal to the size of the minority class, are constructed:  one for the minority class, the other for the majority class.      

Balanced Accuracy Score:

<img width="150" alt="2021-10-16 (14)" src="https://user-images.githubusercontent.com/84471904/137604014-44ac9709-d2e7-4f48-9a43-0cb709ca7f4f.png">

Imbalanced classification Report:

<img width="372" alt="2021-10-16 (15)" src="https://user-images.githubusercontent.com/84471904/137604030-fac9c1a0-99f1-41b2-aefd-825a0d72f5e7.png">

_Easy Ensemble AdaBoost Classifier_ 

The classifier is an ensemble of AdaBoost learners trained on different balanced boostrapsamples, with balancing achieved by random under-sampling.

Balanced Accuracy Score:

<img width="122" alt="2021-10-16 (17)" src="https://user-images.githubusercontent.com/84471904/137604173-4b2d691e-ecd3-4d08-9d8f-d4a5e0dbb23d.png">

Imbalanced classification Report:

<img width="393" alt="2021-10-16 (18)" src="https://user-images.githubusercontent.com/84471904/137604186-9d25a2c8-990c-4110-a71d-cb208d80234a.png">


## Results

Balanced Accuracy:  metric used to evalualte how good a binary classifier is; especially useful when classes are imbalanced. 

The classification report is about key metrics in a classification problem.

You'll have precision, recall, f1-score and support for each class you're trying to find.

The recall means "how many of this class you find over the whole number of element of this class"

The precision will be "how many are correctly classified among that class"

The f1-score is the harmonic mean between precision & recall

The support is the number of occurence of the given class in your dataset (so you have 37.5K of class 0 and 37.5K of class 1, which is a really well balanced dataset.




