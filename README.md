# Time Series Model Forecasting of Real Estate Data from Zillow.com
## **TOP FIVE BROOKLYN ZIPCODES TO INVEST IN** 

Author:  David R. Torres

The Model 4 project task was to create models for time series forecasting.  The project consisted of acting as a consultant for a real estate firm and they asked me to provide analysis and recommendations of the 5 best zipcodes in Brooklyn to invest in.  The top zipcodes would be based on the highest Return on Investment and risk vs. profitability. The investment firm was looking for short-term investments with the highest returns over a 3 year period. The investment firm wasn't interested in long term investments which require purchasing property and keeping them to increase in value.

### **Data**
I worked with real estate sales data from Zillow.com which covered the time period 4-1-1996 to 4-1-2018.  I created models for a univariate Series.  I did not include categories other than the monthly mean sales prices for each zipcode. 

### **Methods**
Preprocessing of data involved using the .melt() function because the columns included date columns which needed to be set up so they could be used as the index.  
The data was split into train and test sets.
I used an auto_arima model as a gridsearch to find the lowest AIC scores and corresponding p,d,qs.  
I then created a statsmodel summary for each zipcode and sliced this data to create a dataframe of all the p,d,qs and lowest AIC for each zipcode.
Created a SARIMA model to make predictions regarding the test data.  The auto-arima model identified the set of parameters that produces the best fitting model for   each zipcodes and I included these optiml parameters into the SARIMA model.  

## **Business Problem**
The investment firm has asked to provide an analysis and recommendations regarding the top 5 zipcodes in Brooklyn to investment in. 

## **Recommendations**


