# Part A Time_series_analysis
In this notebook, you will load historical Dollar-Yen exchange rate futures data and apply time series analysis and modeling to determine whether there is any predictable behavior. Decompose the Yen Settle price using the Hodrick-Prescott Filter to understand Trend and Noise. Then calculate future Settle Returns, estimate an ARMA model for these Settle returns, an ARIMA model for Yen Settle prices and a GARCH model to understand Yen volatility to provide answers to the below questions.

## Based on your time series analysis, would you buy the yen now?
Per ARMA Returns model (though p value is greater than .05 for ARMA and ARIMA), the return associated with yen is forecasted to fall sharply and then rise marginally and stabilise. But from the ARIMA model, it appears that the forecasted settle prices will go up. From the GARCH model it appears that the volatility associated with yen will increase. Therefore if you have a yen for "risk", suggest that you buy the yen after considering other factors else wait for the volatility to subside.

## Is the risk of the yen expected to increase or decrease?
To increase- From the GARCH model it appears that the volatility associated with yen will increase.

## Based on the model evaluation, would you feel confident in using these models for trading?
Based on the results of the above models, not sure if these models are a good fit as the p > 0.05. Other factors that are not included in these models will also impact how the yen will perform. Therefore I believe that these models may help but are not the only factors to determine trading strategy.

## Part B- Regression_analysis:
In this notebook, you will build a SKLearn linear regression model to predict Yen futures ("settle") returns with lagged Yen futures returns. 
## Conclusions
The ideal RMSE should be as close to 0 implying little deviation from expected. It is interesting to note that the train  RMSE (in sample) is much higher- generally this is lower- than the test RMSE (out of sample) implying some kind of mismatch.