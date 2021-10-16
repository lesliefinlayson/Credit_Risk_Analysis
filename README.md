# Credit_Risk_Analysis

## Project Purpose

Determining credit risk presents a challenge because it is an unbalanced classification problem.  The number of good loans highly outnumber risky loads and therefore results may be skewed if the correct algorithm is not used.  

The purpose of this project is to evaluate 6 different machine learning models to determine which, if any, can be used to reliably and accurately predict credit risk.  These include resampling models, SMOTEEN algorithm, and ensemble classifiers.

## Results

### Resampling Models

_Oversampling with RandomOverSampler_ 

In random oversampling, instances of the minority class are randomly selected and added to the training set until the majority and minority classes are balanced. 

Accuracy Score:

<img width="331" alt="2021-10-16 (2)" src="https://user-images.githubusercontent.com/84471904/137592243-a261fe65-b285-4f25-995d-f5936d829dac.png">

Imbalanced classification Report:

<img width="374" alt="2021-10-16 (3)" src="https://user-images.githubusercontent.com/84471904/137592297-e82c3d82-143b-4e07-ad8e-ec8212d13579.png">

_Oversampling with Synthetic Minority Oversampling Technique (SMOTE) _ 

With SMOTE, new instances of the minority class are interpolated and added to the training set until the majority and minority classes are balanced. 

Accuracy Score:

<img width="238" alt="2021-10-16 (4)" src="https://user-images.githubusercontent.com/84471904/137593307-e819a34b-5b5c-46cf-b00d-1f78c0cfad47.png">

Imbalanced classification Report:

<img width="383" alt="2021-10-16 (5)" src="https://user-images.githubusercontent.com/84471904/137593386-a2fad91f-cf98-446d-ab10-2687d8c1c783.png">












