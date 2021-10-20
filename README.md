The financial departments of large companies often deal with foreign currency transactions while doing international business. As a result, they are always looking for anything that can help them better understand the future direction and risk of various currencies.In this assignment, you will test the many time-series tools that you have learned in order to predict future movements in the value of the Japanese yen versus the U.S. dollar.

# Part A Time_series_analysis
In this notebook, you will load historical Dollar-Yen exchange rate futures data and apply time series analysis and modeling to determine whether there is any predictable behavior. Decompose the Yen Settle price using the Hodrick-Prescott Filter to understand Trend and Noise. Then calculate future Settle Returns, estimate an ARMA model for these Settle returns, an ARIMA model for Yen Settle prices and a GARCH model to understand Yen volatility to provide answers to the below questions.

# Based on your time series analysis, would you buy the yen now?
Per ARMA Returns model (though p value is greater than .05 for ARMA and ARIMA), the return associated with yen is forecasted to fall sharply and then rise marginally and stabilise. But from the ARIMA model, it appears that the forecasted settle prices will go up. From the GARCH model it appears that the volatility associated with yen will increase. Therefore if you have a yen for "risk", suggest that you buy the yen after considering other factors else wait for the volatility to subside.

# Is the risk of the yen expected to increase or decrease?
To increase- From the GARCH model it appears that the volatility associated with yen will increase.

# Based on the model evaluation, would you feel confident in using these models for trading?
Based on the results of the above models, not sure if these models are a good fit as the p > 0.05. Other factors that are not included in these models will also impact how the yen will perform. Therefore I believe that these models may help but are not the only factors to determine trading strategy.

## Part B- Regression_analysis:
In this notebook, you will build a SKLearn linear regression model to predict Yen futures ("settle") returns with lagged Yen futures returns. 

# Conclusions
The ideal RMSE should be as close to 0 implying little deviation from expected. The out of sample (test data) is lower than the in the sample (train data) which ideally should have been the other way around i.e. the RMSE of train data should have been lower. Additionally the RMSE values are significantly different. Suggest that the train data be revisited.