# Bangalore_Home_Price
This project aim is to predict home price in Bangalore and identify key driving  features which have impact on decidng price of home in Bangalore.

## Table of Content
 
  * [Problem_Definition](#Problem_Definition)
  * [Dataset_Description](#Dataset_Description)
  * [Data_Preprocessing](#Data_Preprocessing)
  * [Model_Building](#Model_Building)
  * [Result](#Result)
  * [Credit](#Credit)
  
## Problem_Definition
Bangalore is a well known IT hub. Its very crucial for a newcomer who starts his/her carrer in Bangalore to know price of home/flat at a particular location with certain types of facility in home.Aprat for this, for those who already lived in this city , model will useful to predict price of flat.
 
 
 ## Dataset_Description
 The dataset consists of the following attributes:

* SL.NO.
* Area Type
* Availability   - Wether able to move or not
* Location   
* Size  - 1 BHK / 2 BHK / 3 BHK
* Society  - Type of Society
* total_sqft  - area of home
* bath - number of bath
* balcony - number of balcony
* Target Variable - Price

 

## Data_Preprocessing
* Null Values drpped due to 1% NA's values
* Dropping  features  - 'area_type','society','balcony','availability' due to high cardinality
* Applying mean of max and min value for the range value of total Area Feature
* Creaetd new feature - Price per square feet
* Applying dimensoality reduction technique on 'Location' feature to reduce number of locations.
* Outlier removal with the use of +/- 3 standard deviation
* Applying one hot encoding for location feature


## Model_Building
* Created X & Y datafraem wehre X - features , Y - Target  Variable 
* Applying GridSearchCV hyperparameter tuning on - linear regression , Lasso , decision Tree .
* 



## Result
* Linear Regression Algorithms perform bettern than other models.
* linear regression algorith gives accuracy - 84.78%
* The key deciding  features of a home price are  'toal Square feet','no. of BHK','location' .

## Credit
 This project has been done as a course project .

