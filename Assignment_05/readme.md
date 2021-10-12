**Regression Modelling and exploratory analysis of Used cars selling prices**

**Business Objective:** To identify trends in the sales of used cars segment by exploring the dataset and predicting their market value (price) by their respective attributes. For first-time car buyers, COVID-19 has fueled the demand for the sale of used cars. This analysis helps one to understand the trends in the prices of the segment of the used cars and able to identify drivers that determine the car prices and able to predict the car prices to check one's affordability.

**Inferences from Exploratory Analysis**

1) Most of the car prices are in the range of 300000 to 1500000
2) Most of the cars sold are 5-seaters
3) Most of the cars sold has mileage in the range of 18-22 km/liter
4) Most of the cars sold has an engine capacity of 1200 to 1300 cc
5) The cars bought during 2017 & 2016 are sold mostly
6) The cars that are manufactured by Maruti, Hyundai, & Mahindra are sold the most
7) Lexus, BMW, Volvo have the most automatic cars sold rather than manual cars. Force & Fiat has the most manual cars sold than the automatic ones.
8) The columns year & mileage, and year & kilometers driven has the highest correlation.
9) Test drive cars and first owners cars the highest sold cars
10) Diesel and petrol variant cars are the most sold cars.
11) The Volvo car manufactured in 2017 has the highest selling price, and the prices of the cars have increased significantly over the years.


**Inferences from Regression Analysis**

1) In our Regression model, we could explain about 47% of the variation in selling prices.
2) A simple OLS regression model is appropriate for our model rather than a model with increasing or decreasing the regularization strengths.
3) Number of miles/kilometers driven and seating capacity are the primary factors influencing the selling prices of the cars.
4) Since there are interdependent features, we should handle the issue of multicollinearity.
5) As we could explain only 47% of the variance in selling prices, we need to consider other features to improve the model performance.
