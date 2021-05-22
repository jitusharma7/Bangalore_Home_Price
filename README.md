# Bangalore_Home_Price
This project aim is to predict home price in Bangalore and identify key driving  features which have impact on decidng price of home in Bangalore.

## Table of Content
 
  * [Problem_Definition](#Problem_Definition)
  * [Dataset_Description](#Dataset_Description)
  * [Data_Preprocessing](#Data_Preprocessing)
  * [Model_Building](#Model_Building)
  * [Result](#Result)
  * [Business_Recommendation](#Business_Recommendation)
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
* Dropping three features 'SLNO','Candidate Ref' and 'Location' dueto high cardinality
* Applying Label Encoding to'offered band' ordinal feature.
* Applying one hot encoding to restof the categorical features
* Used drop_first feature of one hotencoding to avoidmulticollinearity
* Checked for multicollinearity using correlation mapand variance Inflation factor,Two features 'Pecent hike expected in CTC' and'Percent hike offered in CTC' has been removed

    <img src="/VIF.PNG" width="400">


## Model_Building
* XG Boost performs better thanother models
* Hyperparameters tuning isdone by RandomizedSearchCV for xgboost
* It has a higher accuracy of83.24%
* True Negative is almost doublethan false negative
* Rest of the models have verypoor performance in terms ofpredicting true negative values
* True negative values are crucialbecause it is important to knowwho will not join theorganization


     <img src="/ModelComparison.PNG" width="400">

## Result
* XG Boost classifieroutperforms here among all model with 83.24% accuracy
* Feature importance score from XGBoost classifier
* Top 3 important features = 'Percent difference CTC', 'Duration to accept offer', 'Age'
* Least 3 important features = 'Joining Bonus_Yes', 'LOB_EAS', 'LOB_Healthcare'

## Business_Recommendation
* Firm should focus on 3 important features 'Percent difference CTC', 'Duration to accept offer'& 'Age'
* Firm should introduce new offering/schemes  based on these 3 features combination so that attrition rate can reduce.

## Credit
[dare2Compete](https://https://dare2compete.com/) - This project has been done on this competitive platform.

