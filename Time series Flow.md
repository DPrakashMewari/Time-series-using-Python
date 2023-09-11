Time Series : 
A sequence of data point collected over time often used for analysis , forecasting and understanding Trends 

Here things will happen extrapolition way : To Find out the value out of the range 

Time Series Components :

Trend
Seasonality 
Cyclic
Noise 

---- Data Preprocessing Requires --- :

Handling Missing Values 
Handling outlier 
Handling TimeZone 

---- Exploratory Data Analysis ---- 

Linear Chart
Area Chart
Seasonal check
Ouliteranalysis 
lag plot 
rolling stats 

----- Stationery Check -----
Visual Inspection 
Summary Statistics : If not constant mean and variance  Not Stationery 
ADFTEST

IF WE FIND OUT NO STATIONERY 
----- Data Transformation ------ 
Will Do 
Differening 
Log Transformation 
Box-cox Transform 

* Remember iterative process it is ---

*----- Decomposition to check :---- 
Trend 
Seasonality
Resid

--- ACF AND PACF -- TO IDENTIFY POTENTIAL ORDERS  -- For All Models ----

Autocorrelation - How correlated a time series is with its past values, if positive at Lag-1 then AR if
negative then MA

Partial Autocorrelation - The correlation between 2 variables controlling for the values of another set of
variables. If the partial autocorrelation drops of quickly then AR terms, if it slowly decays then MA

-----

Model Selection on different modedls

SIMPLE MOVING AVG : SMOOTHING OF TIME SERIES DATA 
Cummalative Moving Avg : Find out avg of all data point d1+d2/2 ...
Exponential Moving Avg : Give More Weightto recent datapoint and less to old 

Arima Model :  ARIMA models are displayed in the terms (p,d,q) which stand for p - periods to lag for, d -
number of transformations used to make the data stationary, q - lags of the error component

Seasonal SARIMA (Seasonal AutoRegressive Integrated Moving Average) is a time series forecasting model that extends ARIMA to handle seasonality in the data.
# Fit a Seasonal SARIMA model
order = (1, 1, 1)  # Non-seasonal order (p, d, q)
seasonal_order = (1, 1, 1, 7)  # Seasonal order (P, D, Q, S)


Vector AutoRegressive (VAR) is a time series forecasting model that considers the relationship between multiple time series variables.
model = VAR(df[['data1', 'data2']])

-------Model Training and testing happen on test data -----

Split data into train and test
Selected model used to predict for test data 

----
Later we have Stage: Model Evaluation 

MAE 
MSE 
RMSE
AIC (Akaike Information Criterion) or BIC (Bayesian Information Criterion): Information criteria that balance model complexity and goodness of fit. Lower values indicate better models.

Ljung-Box Test: A statistical test to check if the residuals (forecast errors) are white noise, indicating a well-fitted model.

Cross-Validation: Techniques like k-fold cross-validation or time series cross-validation are used to assess a model's performance on multiple test sets.

-------
Interpret Model : 
Plot and check 

------

Refinement and Imporvement







