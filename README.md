# Credit_Risk_Analysis

## Project Purpose

Determining credit risk presents a challenge because it is an unbalanced classification problem.  The number of good loans highly outnumber risky loads and therefore results may be skewed if the correct algorithm is not used.  

The purpose of this project is to evaluate 6 different machine learning models to determine which, if any, can be used to reliably and accurately predict credit risk.  These include resampling models, SMOTEEN algorithm, and ensemble classifiers.

## Results

### Resampling Models

_Oversampling with RandomOverSampler 

In random oversampling, instances of the minority class are randomly selected and added to the training set until the majority and minority classes are balanced. 

Accuracy Score:

<img width="331" alt="2021-10-16 (2)" src="https://user-images.githubusercontent.com/84471904/137592243-a261fe65-b285-4f25-995d-f5936d829dac.png">

Imbalanced classification Report

<img width="374" alt="2021-10-16 (3)" src="https://user-images.githubusercontent.com/84471904/137592297-e82c3d82-143b-4e07-ad8e-ec8212d13579.png">

