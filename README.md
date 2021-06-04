# KingCountyPredictions
---


# Overview

This project, we took a look at the King County Housing Data. King County is the greater Seattle area, to build a model that predicts house prices for homes in the area.
So I will build a linear regression model to predict the housing price to help accurately price homes they represent.
An overview of the average home in the dataset... 3 bedrooms, 2 bathrooms, $540,000, ⅓ acre yard, 3 condition (Average), 1 floor, Built in 1971

---

# Data

King County housing dataset contained data from May 2014-2015. I am looking to identify and predict housing sales prices based on features with a RMSE of less than $200,000.

---

# EDA
Initial columns provided in the data set include:


- id - unique ID for a house
- date - Date day house was sold
- price - Price is prediction target
- bedrooms - Number of bedrooms
- bathrooms - Number of bathrooms
- sqft_living - square footage of the home
- sqft_lot - square footage of the lot
- floors - Total floors (levels) in house
- waterfront - Whether house has a view to a waterfront
- view - view rating of house
- condition - How good the condition is (overall)
- grade - overall grade given to the housing unit, based on King County grading system
- sqft_above - square footage of house (apart from basement)
- sqft_basement - square footage of the basement
- yr_built - Year when house was built
- yr_renovated - Year when house was renovated
- zipcode - zip code in which house is located
- lat - Latitude coordinate
- long - Longitude coordinate
- sqft_living15 - The square footage of interior housing living space for the nearest 15 neighbors
- sqft_lot15 - The square footage of the land lots of the nearest 15 neighbors 

I examined the correlation between price and the other variables for multicollinearity. 
![image](https://user-images.githubusercontent.com/76975163/111123827-2c28ac00-8546-11eb-9b40-6cc1983685d2.png)

After handling the extra variables I looked for outliers that may be in the data, which included a bedrooms with a large amount of bedrooms.
![image](https://user-images.githubusercontent.com/76975163/111124089-76119200-8546-11eb-80b8-40ed2924d968.png)

I continued my exploratory research by looking tot see if there was a relationship between the amount of houses sold by yr built in 25 year increments. 
![image](https://user-images.githubusercontent.com/76975163/111124394-db658300-8546-11eb-8a21-9daadbb8b01e.png)

Through my exploratory data, I was able to start creating a model to that would best predict the price.
I ran a test train split and tried two different feature selections in the KBest and RFECV for the best possible model.

The RFECV gives a underfitted model.

<img width="761" alt="Screen Shot 2021-03-15 at 4 33 02 AM" src="https://user-images.githubusercontent.com/76975163/111125028-88d89680-8547-11eb-8de8-5655863eb86d.png">

<img width="743" alt="Screen Shot 2021-03-15 at 4 36 15 AM" src="https://user-images.githubusercontent.com/76975163/111125452-fd133a00-8547-11eb-8ca7-2046987355d4.png">
<img width="478" alt="Screen Shot 2021-03-15 at 4 36 52 AM" src="https://user-images.githubusercontent.com/76975163/111125530-12886400-8548-11eb-9d68-c690c4f94b9c.png">


---


# Conclusion
I repeated multiple linear regression models to get the best possible model for prediction as well as used the
KBest and RFECV feature. The original model gives me a RMSEof 156,729. I would look forward to trying to get an even lower RMSE model with a more accurate prediction. 


My github folder includes the CSVs for the Kings County Housing Data, Kings County Holdout Data.

