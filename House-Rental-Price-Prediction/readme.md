# House Rental Price Prediction Using Regression
This project was assigned for completing Junior Data Scientist Course by [Narasio Data](https://narasiodata.com/)

## Information
The case study uses data containing: 

the dependent variable (Y) = rent

the independent variable (X)
  * Bedroom
  * Bathrooms
  * Area
  * Floor_number_gate_community
  * Light bill
  * Maintenance_amt
  * Deposit_amt

## Problem
* Determine the effect of variable X on variable Y
* Analysis and prediction of house rental prices

## Used Technologies
* Jupyter Notebook
* Library Sklearn
* Library Statsmodel
* Library Pandas, Numpy, and Matplotlib

## Development Steps
* Data Cleansing (checking missing values, duplicates, and data types)
* Data Pre-Processing (Normality test and Multicollinearity test)
* Feature Engineering
    Scaling. The data will be scaled to reduce the gaps between the columns in the data, this process does not change the distribution of the data, it only changes the data scale.
* Modelling
* Analysis

## Conclusion
Based on the loaded train data, 5-column data are taken, namely bedroom, bathrooms, area, floor_number, and deposit_amt.

In the multicollinearity test, it was found that the bedroom and bathroom values have the same correlation so it can be concluded that the two columns have the same values, causing the regression model to have multicollinearity problems. It has also been shown that the percentage of bedroom and bathroom data similarity is 88.1%. To make a model suitable for use, drop one of the columns, namely bathrooms because it has a large correlation.

Then the P-value test was carried out and it was found that the four variables significantly influenced the Rent (Y) variable.

It is also obtained, the p-value <0.05 so that H0 is rejected. It can be concluded that the regression model of the four independent variables and the dependent variable rent is feasible to use.
