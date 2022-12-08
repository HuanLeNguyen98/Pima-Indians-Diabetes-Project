# Pima Indian Diabetes Analysis

## Introduction
<img align="right" width="350" src="Img/Pima Indian Pic.jpg">
Diabetes is one of the most frequent diseases worldwide and the number of diabetic patients are growing over the years. The main cause of diabetes remains unknown, yet scientists believe that both genetic factors and environmental lifestyle play a major role in diabetes.
A few years ago research was done on a tribe in America which is called the Pima tribe (also known as the Pima Indians). The Pima Indians, a Native American population, pose a unique opportunity for diabetes researchers due to their limited European admixture. This posits the greatest opportunity to study diabetes with the uncontrollable genetic factor playing the smallest possible role. In this tribe, it was found that the ladies are prone to diabetes very early. Several constraints were placed on the selection of these instances from a larger database. In particular, all patients were females at least 21 years old of Pima Indian heritage.

## Objective
This project is to  analyze different aspects of Diabetes in the Pima Indians tribe by doing Exploratory Data Analysis, and then using Statistical screening from Logistic Regression to validate the model and predict the diabetes from a given dataset.

## Data Dictionary
The dataset has the following information:
Pregnancies: Number of times pregnant
Glucose: Plasma glucose concentration over 2 hours in an oral glucose tolerance test
BloodPressure: Diastolic blood pressure (mm Hg)
SkinThickness: Triceps skin fold thickness (mm)
Insulin: 2-Hour serum insulin (mu U/ml)
BMI: Body mass index (weight in kg/(height in m)^2)
DiabetesPedigreeFunction: A function that scores the likelihood of diabetes based on family history.
Age: Age in years
Outcome: Class variable (0: a person is not diabetic or 1: a person is diabetic)

## Exploratory Data Analysis
The detail of data analysis is in Jupiter file in Github. Below is the heat map to check for the multic-collinearity.
The correlation matrix above uses Pearson’s correlation coefficient to illustrate the relationship between variables.
<img align="center" width="350" src="Img/Pima Indian Heat Map.jpg">
From the figure, a significant correlation can be observed between Pregnancies and Age (0.54), BMI and Skin Thickness (0.53). By the rule of thumb, in the case of the correlation coefficient is above 0.70, multi-collinearity is expected. Hence, no significant case of multi-collinearity is observed.
 
## Building Model
A logistic regression is used from the dependent variable is binary, ordinal or nominal and the independent variables are either continuous or discrete
In this scenario, a Logit Model has been used to fit the data
In this case an event is defined as occurance of ‘1’ in outcome
Basically logistic regression uses the odds ratio to build the model

## Summary
The accuracy of the Logistic Regression model is 76% means that this model can explain 76% of the variation in dependent variables
The result from confusion_matrix indicates that 442+139 = 481 are correct predictions and 129+58 = 187 are incorrect predictions in the total 768 cases.
 
Note: The model has been improved recently the accuracy is above 90% vs. 76% currently. Results will be uploaded soon.

