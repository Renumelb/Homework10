# Homework10
In this notebook, you will load historical Dollar-Yen exchange rate futures data and apply time series analysis and modeling to determine whether there is any predictable behavior.

Using futures Settle Returns, estimate an ARMA model

ARMA: Create an ARMA model and fit it to the returns data. Note: Set the AR and MA ("p" and "q") parameters to p=2 and q=1: order=(2, 1).
Output the ARMA summary table and take note of the p-values of the lags. Based on the p-values, is the model a good fit (p < 0.05)?
Answer: Based on the p-values below, it appears that model is not a good fit as the p values are greater than 0.05.
Plot the 5-day forecast of the forecasted returns (the results forecast from ARMA model)

Forecasting the Settle Price using an ARIMA Model
Using the raw Yen Settle Price, estimate an ARIMA model.
Set P=5, D=1, and Q=1 in the model (e.g., ARIMA(df, order=(5,1,1))
P= # of Auto-Regressive Lags, D= # of Differences (this is usually =1), Q= # of Moving Average Lags
Output the ARIMA summary table and take note of the p-values of the lags. Based on the p-values, is the model a good fit (p < 0.05)?
Construct a 5 day forecast for the Settle Price. What does the model forecast will happen to the Japanese Yen in the near term?

Using futures Settle Returns, estimate an ARMA model

ARMA: Create an ARMA model and fit it to the returns data. Note: Set the AR and MA ("p" and "q") parameters to p=2 and q=1: order=(2, 1).
Output the ARMA summary table and take note of the p-values of the lags. Based on the p-values, is the model a good fit (p < 0.05)?
Plot the 5-day forecast of the forecasted returns (the results forecast from ARMA model)

Second notebook:
In this notebook, you will build a SKLearn linear regression model to predict Yen futures ("settle") returns with lagged Yen futures returns.