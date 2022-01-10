# Flight-Fare-Prediction

### Abstract
Someone who purchase flight tickets frequently would be able to predict the right time and fare of ticket to obtain the best deal. Airlines change ticket prices for revenue management. To estimate the minimum airfare, data for a specific air route has been collected including features like departure time, arrival time and airways over a period. Features are extracted from the collected data to apply Machine Learning(ML) models. This case study gives the machine learning regression methods to predict flight prices at the given time.

### Problem Statement:
This is a Machine learning project. In this project I am trying to predict the fare of flights by training the dataset which contain data for one year.

![image](https://user-images.githubusercontent.com/84588705/148721074-2c275888-c375-4a62-b7ba-7d20ca02c453.png)

### Approach:
## Data Preprocessing:
In this section I am doing all the Data cleaning and analysis. Most of the data is in categorical form which should get converted into numerical form.

I did some feature engineering in it and created columns of day and months. There are many columns which I created from the existing column which you can see in the notebook.

I dropped the additional info and route columns as most of the values were missing or of no use.

Here is the comparision graph of Airline vs the price.

![image](https://user-images.githubusercontent.com/84588705/148720694-0a89482a-8b4b-4780-8433-851c7638fbd6.png)


This all the process I followed for test dataset as well and made a training and test dataset to feed in the Machine learning algorithm.

### Feature Selection:
Finding out the best feature which will contribute and have good relation with target variable. Following are some of the feature selection methods.

(1) Heat Map

![image](https://user-images.githubusercontent.com/84588705/148721774-d6228565-c9a1-4293-8732-4cdc6e553259.png)


(2) ExtraTreesRegressor

![image](https://user-images.githubusercontent.com/84588705/148721785-0523256c-a773-47d5-8daf-1867023ae3f8.png)


### Model Implementation:
I used Multiple models to fit the dataset. Below are the best metrics which I got

1) Linear Regression :       R2 score = 0.614           RMSE = 2731.67
2) Decision Tree Regressor : R2 score = 0.731           RMSE = 2370.05
3) Random Forest Regressor : R2 score = 0.827           RMSE = 1897.45
4) XGBoost Regressor :       R2 score = 0.845           RMSE = 1797.82


