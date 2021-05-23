# Bangalore_Home_Price
This project's aim is to predict home price in Bangalore and identify key driving features which have an impact on the decidng price of a home in Bangalore.

## Table of Content
 
  * [Problem_Definition](#Problem_Definition)
  * [Dataset_Description](#Dataset_Description)
  * [Data_Preprocessing](#Data_Preprocessing)
  * [Model_Building](#Model_Building)
  * [Result](#Result)
  * [Credit](#Credit)
  
## Problem_Definition
Bangalore is a well-known IT hub. It's very crucial for a newcomer who starts his/her career in Bangalore to know the price of a home/flat at a particular location with certain types of facilities in the home. Apart from this, for those who already lived in this city, the model will use to predict the price of a flat.
 
 
 ## Dataset_Description
 The dataset consists of the following attributes:

* SL.NO.
* Area Type
* Availability   - Wether able to move or not
* Location   
* Size  - 1 BHK / 2 BHK / 3 BHK
* Society  - Type of Society
* total_sqft  - the area of the home
* bath - number of baths
* balcony - number of balconies
* Target Variable - Price

 

## Data_Preprocessing
* Null Values dropped due to 1% NA's values
* Dropping  features  - 'area_type','society','balcony','availability' due to high cardinality
* Applying mean of max and min value for the range value of total Area Feature
* Created new feature - Price per square feet
* Applying dimensionality reduction technique on 'Location' feature to reduce the number of locations.
* Outlier removal with the use of +/- 3 standard deviation
* Applying one-hot encoding for location feature


## Model_Building
* Created X & Y data frame where X - features, Y - Target  Variable 
* Applying GridSearchCV hyperparameter tuning on - linear regression, Lasso, decision Tree.




## Result
* Linear Regression Algorithms perform better than other models.
* linear regression algorithm gives accuracy - 84.78%
* The key deciding features of a home price is 'total Square feet', 'no. of BHK', 'location'.

## Credit
 This project has been done as a course project.

