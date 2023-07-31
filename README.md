# Stock-price-Prediction
Predict the stock value using machine learning models 


Amazon Stock Price Prediction using Machine Learning Techniques

Technologies: Machine Learning and Deep Learning
Methods: Linear Regression, Decision Tree Regression, Random Forest Regression, XGBoost Regression, Long-Short term Memory

Data and Sources:
We used historical stock price data of Amazon.com (AMZN) for ten years. The data have been scrapped from S&P 500 using an appropriate scrapping method. The imported data includes records of all registered 500 companies from 2010 – 2020. Out of which the Amazon records have been selected. The description of each variable in the data set that we are going to use is as below.

Variable Name	Names in the Dataset	Variable Type
Date	Date	Datetime
High	High	Continuous
Low	Low	Continuous
Open	Open	Continuous
Close	Close	Continuous
Volume	Volume	Continuous
Adjusted Close	Adj_Close	Continuous
Moving Averages	Moving_avg	Continuous
Increase in Volume	Increase_in_Vol	Continuous
Increase in Adjusted Close	Increase_in_adj_close	Continuous
Year	Year	Datetime


For the current study, we added three new variables: 
(1) moving averages
(2) increase in volume
(3) increase in the adjusted close. 

These variables will help us to check the variability of the stock prices. We also added “Year” column by extracting year from the “Date” column. 
Moving averages has been calculated by taking mean of the adjusted close. 
Increase in Volume has been calculated by subtracting the volume from 2020 to 2019. 
It will explain the yearly change in the volume. Similarly, we checked the increase in adjusted close by subtracting the
adjusted close from year 2020 to 2019. These calculations will explain the actual fluctuations. 
The final dataset which we are going to use contains 2635 rows and 9 columns.
