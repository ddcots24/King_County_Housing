# King_County_Housing
Analysis of Housing Data in King County, Washington
 
## Overview
I have been tasked with analyzing the data on houses in King County, Washington. The goal is to help prospective buyers near Amazon HQ understand the housing market better. I did this by creating a predictive model of the sale price of houses, in King County, based on different features. After building and assesing the linear regression model, I determined that the features with the largest weight, and the strongest correlation to price, were square feet of living space and number of bathrooms.

## Business Problem
King County is the most populous county in the state of Washington and the thirteenth most popular in the United States of America. In Kings County, the largest populated city is Seattle with a total of over 700,000 people. Recently, Seattle has made itself a home to new innovations. Starbucks, Costco, and Microsoft are just a few of the titans of the industry located within. Additionally, the largest employer of the county is Amazon with over 75,000 employees in Washington alone. The new influx of business created a pipeline for new prospective workers. These workers are searching for employment and housing options near Amazon HQ. However, the process of resettling is more complex than expected. Questions begin to compound and answers are seldom found. 

## Data
I utilized a few different data sources for our model so that we could obtain a comprehensive and accurate prediction of home prices.
King County House Data:
A data source that provided the following information; date, number of floors, waterfront property, greenbelt property, nuisance, view, condition, long, lat, grade, heat_source, sewer_system, sqft_garage, sqft_patio, yr_built,y r_renovated, address, price, bedrooms, bathrooms, sqft_living, sqft_lot, sqft_above, and sqft_basement. 

## Methods
The majority of the dataset pertained to houses sold in King County, Washington, but there were several outliers that needed to be addressed. After focusing on just King County I performed a heatmap to show any correlations between the independent features in my model. 

![image](https://github.com/ddcots24/King_County_Housing/assets/131708046/12a18675-31a1-46ab-8738-668929bd4a88)



From the following graphic we were able to identify square feet above and square feet of living have a very high correlation of 90%. I took out square feet of living to prevent from overfitting my model.


![image](https://github.com/ddcots24/King_County_Housing/assets/131708046/d81ec703-d1df-4f41-961f-cf2b8d33743a)


I further narrowed the scope of our research to focus on the technology hub in downtown Seattle. In particular, I identified Amazon as the largest employer and point of interest to wanna-be buyers. The range was focused to be a 3-mile radius around Amazon Center. What was discovered was a strong correlation between the price of houses with the sqft_living. I was able to form a regression line to model the relationship. 

After focusing on the correlation between square feet of living and price, I turned my attention to the number of bathrooms.  What was observed was that the number of bathrooms has a strong posotive correlation with the price of the house. However, the data is slightly skewed by the limited data points with houses beyond six bathrooms. 

![image](https://github.com/ddcots24/King_County_Housing/assets/131708046/6b8f1996-f6ca-4305-9424-88c21f9214b0)



## Results
I fit the following data into a multivariable linear regression model to establish a fairly accurate price guage, based upon features represented within the data. I achieved an R-square score of .63 indicating that the predicted value will fall with 63 percent accuracy. The following visual further shows the effectiveness of predicting price by fitting a regression line between the actual and predicted price value. 

![image](https://github.com/ddcots24/King_County_Housing/assets/131708046/328104c5-e0c5-4a91-a6f8-473ef03c7ee2)


## Analysis of Model
The model includes aspects of all numerical, ordinal, and nominal categories from our data frame and the influence of each category on our predicted price. About 63% of the variability observed in the sale price is explained by the regression model. The model is a predictor of house prices based on certain features in King County. Some coefficients to note that have an increase in house sale price include bathrooms, sqft_living, sqft_above, sqft_basement, sqft_patio, grade, condition, and view. 

## Recommendations

Recommendations are as follows:
1) Increase the square footage of living space by adding an extension to an existing house
2) Purchase a less expensive home and then add bathrooms to add value to the house
