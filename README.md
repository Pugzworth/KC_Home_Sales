# Module 2 Modeling Project

### Repository
Readme
- The readme file contains a brief explanation of our project goals, findings, metrics used, a comparison of our final model versus our baseline, and our recommendations. 

Tim's Notebook (Project_2_Modeling_Tim_Notebook)
- Tim's jupyter notebook. It runs through his entire modeling process with explanations for each step.
(Lenaya's Notebook)
-
Jesus' Notebook
- For the branch named (Jesus), contains the notebook regarding a Ridge regression model.
- The base model for the notebook contains the raw dated fed to the model.
- After normalizations where made to the data and got a better score after normalizing my data.
kc_house_data.csv
- The csv file containing the data that we used for the project.

### Project Goals
* The goal of our project was to take data for sales of homes in King County, Washington and determine which features of home sales best predict the sales price. Our goal was to run a multivariate linear regression to determine which factors from our dataset influenced the sales price of houses the most in order to make a business based recommendation on how to build homes in order to increase profitability.

### Error Metrics
* Our main error metric was Mean Absolute Error. We also routinely used r^2, the coefficient of determination, in our notebooks, but we decided to use Mean Absolute Error as our primary metric. 
  The Mean Absolute Error is the average of the absolute differences between the predicted and actual values. We used this metric because we felt it was the most easily explainable to an audience without a statistics background. We also used it over the coefficient of determination because it is better at detecting bias in the data. 

### Findings
* The model that we ultimately used was a Scaled Ridge Linear Regression. We also did some feature selection. The features that we selected were the square footage of the house, square footage of the lot, the square footage of nearby lots, number of bathrooms, number of bedrooms, number of floors, latitude, longitude, zip code, waterfront location, view, and grade. We found that the most significant feature was waterfront view, followed by square footage, latitude, and year built (negative relationship).

### Final Model vs Baseline
* Our model that we used had a Mean Absolute Error of $125,105, versus our baseline model which had a Mean Absolute Error of $129,993. We were unable to improve the linear model by a significant degree.

### Recommendations
* Get information on the cost of building each house. By doing this we could run a similar multivariate linear regression to determine which home features contribute the most in cost. By doing this we could then compare the increase to the sale price of each house with the increase in the cost of each house associated with each feature to determine which house features were the most profitable.
* It would also be useful to use a model were we could link latitude and longitude. While this is possible using a GAM model with tensoring, we were unable to understand how to implement the model sufficiently to be used. This relational approach could be investigated with other features as well. For example, is adding on another bathroom more or less significant when the bathroom is paired with another bedroom?
* Obtaining more data would also be useful. Our data set stops at 2015 and it would probably be useful to have data closer to the present.
