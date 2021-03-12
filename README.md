PROJECT 2

#Overview
This project, we took a look at the King County Housing Data. King County is the greater Seattle area, to build a model that predicts house prices for homes in the area.
So I will build a linear regression model to predict the housing price to help accurately price homes they represent.
An overview of the average home in the dataset... 3 bedrooms, 2 bathrooms, $540,000, ⅓ acre yard, 3 condition (Average), 1 floor, Built in 1971

#Data
King County housing dataset contained data from May 2014-2015.

#EDA
Initial columns provided in the data set include:


id - unique ID for a house
date - Date day house was sold
price - Price is prediction target
bedrooms - Number of bedrooms
bathrooms - Number of bathrooms
sqft_living - square footage of the home
sqft_lot - square footage of the lot
floors - Total floors (levels) in house
waterfront - Whether house has a view to a waterfront
view - view rating of house
condition - How good the condition is (overall)
grade - overall grade given to the housing unit, based on King County grading system
sqft_above - square footage of house (apart from basement)
sqft_basement - square footage of the basement
yr_built - Year when house was built
yr_renovated - Year when house was renovated
zipcode - zip code in which house is located
lat - Latitude coordinate
long - Longitude coordinate
sqft_living15 - The square footage of interior housing living space for the nearest 15 neighbors
sqft_lot15 - The square footage of the land lots of the nearest 15 neighbors 

#Conclusion
I repeated multiple linear regression models to get the best possible model for predictions.Using
KBest and RFECV.

My github folder includes the CSVs for the Kings County Housing Data, Kings County Holdout Data.

