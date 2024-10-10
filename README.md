# HeartScope: A Data-Driven Approach to Cardiac Health

## Project Overview

This project analyzes a heart disease dataset to predict exercise-induced angina, a common symptom of Congenital Heart Disease (CHD). We explore various machine learning models to determine the most effective approach for early detection of this condition.

Heart Disease Analysis

## Background

Heart disease is a leading cause of death worldwide, with an estimated 12 million deaths annually. Early detection is crucial for managing the condition and reducing mortality rates. This study focuses on predicting exercise-induced angina using non-fatal attributes.

## Dataset

The dataset used in this study is from the UCI Machine Learning Repository, specifically the Cleveland Clinic Foundation database. It contains 303 observations with 14 attributes related to heart disease diagnosis.

## Research Question

Can we predict exercise-induced angina among patients diagnosed with some degree of heart disease in Cleveland? Which model is most suitable for detecting this condition with high accuracy?

## Methods

We employed two main machine learning approaches:

1. K-Nearest Neighbors (KNN)
2. Support Vector Machines (SVM) with Linear and Radial kernels

### Data Preprocessing

- Normalization of data
- Removal of binary values and diagnosis column
- 5-fold cross-validation for KNN
- 80:20 train-test split for SVM

## Results

### KNN Performance

KNN Error vs K

- Accuracy: 86.44%
- Error Rate: 13.56%
- Precision: 72.22%
- Sensitivity: 81.25%
- Specificity: 88.37%

### SVM Performance

#### Linear Kernel
SVM Linear ROC

- Accuracy: 80.33%
- Error Rate: 19.67%
- Precision: 57.69%
- Sensitivity: 93.75%
- Specificity: 75.56%

#### Radial Kernel
SVM Radial ROC

- Accuracy: 81.97%
- Error Rate: 18.03%
- Precision: 64.71%
- Sensitivity: 68.75%
- Specificity: 86.67%

## Model Comparison

| Model | Accuracy | Error Rate | Precision | Sensitivity | Specificity |
|-------|----------|------------|-----------|-------------|-------------|
| KNN   | 86.44%   | 13.56%     | 72.22%    | 81.25%      | 88.37%      |
| SVM - Linear | 80.33% | 19.67% | 57.69%   | 93.75%      | 75.56%      |
| SVM - Radial | 81.97% | 18.03% | 64.71%   | 68.75%      | 86.67%      |

## Conclusion

The KNN model demonstrated the best overall performance in predicting exercise-induced angina, with high accuracy and balanced precision and sensitivity. This approach shows promise for early detection of potential heart disease cases.

## Limitations

The main limitation observed was in precision across all models, likely due to the number of false positives. Future work could focus on improving the threshold to balance true positives and false positives more effectively.

## References

- UCI Machine Learning Repository: Heart Disease Data Set
- Bradley Boehmke's Hands-On Machine Learning with R
- R Documentation for ROSE package
- Penn State Quantitative Developmental Systems Methodology Core
