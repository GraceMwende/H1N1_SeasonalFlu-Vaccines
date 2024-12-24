# Predict H1N1 and Seasonal Flu Vaccines
## Overview
predict whether people got H1N1 and seasonal flu using information they shared about their backgrounds, opinions and behaviours

## Problem statement
The goal of this study is to predict  how likely individuals are to recieve their H1N1 and seasonal flu vaccines,whether individuals received the H1N1 and seasonal vaccines based on information about their backgrounds,opinions and health behaviours.
Understanding the factors influencing vaccination decisions can inform strategies to improve vaccine uptake in future public initiaves.
The study involves analyzing this survey data to uncover relationships between individual characteristics and vaccination patterns altimately develop predictive models to classify 

## Data Understanding
This data is colected from a phone survey in the United States.This phone survey asked respondents whether they had received the H1N1 and seasonal flu vaccines, in conjunction with questions about themselves. These additional questions covered their social, economic, and demographic background, opinions on risks of illness and vaccine effectiveness, and behaviors towards mitigating transmission. 

### Data Analysis
This project uses descriptive analysis, including checking tthe behaviours/opinions that had the most numbers. This provides an overview of the behaviours that influence the H1N1 vaccine or sesonal flu vaccine.
The data was cleaned by filling categorical columns with mode and numeric data with median. Columns with more than 50 % missing values were dropped.
One hot encoding was done for categorical columns since modelling doesnt allow objects.


### Results
Since this is a binary classification , I used logistic regression and Decision Tree for modelling.
On model evaluation the average AUC of 81. MSE for training set and test data was close showing no sign of overfitting or underfitting.

On hyperparameter tuning using grid search Cv i compared Logistic Regression and the best model chosen was logistic regression with thw following parameters:
`C=100, class_weight='balanced',random_state=42, solver='liblinear'`

### Repository Structure
```
├── data
├── h1n1_seasonal_flu_Vaccinepredictions.csv
├── H1N1_SeasonalFlu Vaccines.ipynb
├── test_set_features.csv
├── training_set_features.csv
├── training_set_labels.csv
├── README.md
├── H1N1_SeasonalFlu Vaccines - Jupyter Notebook.pdf
└── H1N1_SeasonalFlu Vaccines.pdf.pdf
```

