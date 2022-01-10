# Flight-Fare-Prediction

### Table of Contents
Problem Statement
Approach
Data Preprocessing
Feature Selection
Model Implementation
Hyperparameter Tuning

### Problem Statement:
This is a Machine learning project. In this project I am trying to predict the fare of flights by training the dataset which contain data for one year.

### Approach:
## Data Preprocessing:
In this section I am doing all the Data cleaning and analysis. Most of the data is in categorical form which should get converted into numerical form.

I did some feature engineering in it and created columns of day and months. There are many columns which i created from the existing column which you can see in the notebook.

I dropped the additional info and route columns as most of the values were missing or of no use.

Here is the comparision graph of Airline vs the price.

![image](https://user-images.githubusercontent.com/84588705/148720694-0a89482a-8b4b-4780-8433-851c7638fbd6.png)



This all the process i followed for test dataset as well and made a training and test dataset to feed in the Machine learning algorithm.

Feature Selection:
Finding out the best feature which will contribute and have good relation with target variable. Following are some of the feature selection methods.

(1) Heatmap

image

(2) ExtraTreesRegressor

image

Model Implementation:
I used Random Forest model to fit the dataset.Below are the metrics which i got

MAE: 1172.5455945373583

MSE: 4347276.1614450775

RMSE: 2085.0122688955757

The R2 square values which i got is 0.7983

Hyperparameter Tuning:
After hyperparameter tuning the best parameters which i got are as follows:

{'n_estimators': 700, 'min_samples_split': 15, 'min_samples_leaf': 1, 'max_features': 'auto', 'max_depth': 20}

The metrics with these parameters are as:

MAE: 1165.606162629916

MSE: 4062650.6911608884

RMSE: 2015.6018186042818

The R2 square i got after hyperparameter tuning I am getting the same score as the previous one.
