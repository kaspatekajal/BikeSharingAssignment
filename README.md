# Bike Sharing Assignment
In this case assignment we are building a multiple regression model to predict the count of bikes shared based on season, weather, date etc.
We will be using below steps to create regression model here.
  a. Reading and Understanding dataset
  b. Visualise data
  c. Prepare data for modelling
  d. Split data in training and test dataset
  e. Build linear model
  f. Analysis of Residuals
  g. Make predictions using final model on test data set
  h. Evaluate model.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
US-based bike sharing company 'BoomBikes' has recently suffered dip in their revenue during pandemic and they would like to know factors driving bike sharing numbers before the pandemic is over so they could get back to previous revenue levels. In the data set we have been provided with the bike sharing data for years 2018 and 2019 along with the external factors like weather, temperature, humidity, windspeed etc. We have also been provided with the counts of registered users and casual users. Factors that may be affecting them like holiday, workingday are also shared with the data.
This dataset was transformed for categorical variables and a normalised scaling was performed using MinMaxScaler. With iterative approach, we have built a linear regression model using statsmodels. For feature selection, we have used RFE function from sklearn.


## Conclusions
Based on the final model, I see below features contribute the most towards explaining demand of the shared bike
a.	Temperature – Coefficient for the temperature is 0.45 and this is the max for all the predictors combined.  Correlation coefficient for this is 0.63 based on corr function. This can explain the increase in bike rentals as the higher temperatures could drive people to go out much and enjoy the bike rides or also rides to parks etc on holidays.
b.	Weather – Second most important predictor is weather. If the weather is bad with thunderstorms, no bikes are rented as we see from the data set. Also, from data visualization we saw that ‘Dry’ weather accounted for more bike rentals. In the final model, we have negative 0.29 as coefficient for ‘Wet’ weather. This is the lowest coefficient we have amongst all predictors. This could also mean, when there is light rain/snow – count of rented bikes falls. So, when the weather is Dry, we should have increase in the bikes rented.
c.	Year – year has a coefficient as 0.23. This is significant in saying that demand for bike sharing is going up from the time it was introduced.  



## Technologies Used
- Numpy 1.24.3
- Pandas 1.5.3
- Seaborn 0.12.2
- statsmodels 0.14.0
- sklearn 1.3.0


## Acknowledgements
- This assignment is part of curriculum for postgraduate program by IIIT-B in Artificial Intelligence and Machine Learning.
- This project uses concepts learned from below modules
  1. Simple Linear Regression
  2. Multiple Linear Regression


## Contact
Created by [@kaspatekajal] - feel free to contact me!
