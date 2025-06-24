# Financial-Data-Analysis-4

## Questions 1-5 are concerned with Value at Risk and Expected Shortfall. Assume that the tail probability of interest is 1%. The daily Amazon (AMZN) and Coca Cola (KO) prices from January 2, 2003 to April 30, 2015 can be downloaded from Yahoo via the quantmod package. Use the adjusted closing prices to compute the daily log returns. Assume that you hold both stocks valued at $1 million each.

### 1- Consider the Amazon stock only.

A. Calculate the VaR of your position for the next trading day using the RiskMetrics method on April 30, 2015. Write down the model based on which you calculate VaR. What is the associated expected shortfall? Also, what is the VaR for the next 10 trading days? 

B. Build a GARCH(1,1) model for the log return series with Gaussian innovations. What is the VaR based on the fitted model for the next trading day? What is the corresponding expected shortfall? 

C. Build a GARCH(1,1) model with Student-t innovations for the log return series. What is the VaR for the next trading day based on the fitted model? What is the corresponding expected shortfall?

### 2- Again, consider the daily log-returns of Amazon stock. The goal here is to use EVT to estimate risk. Using blocks of size 21, fit a generalized extreme value distribution to a proper return series. Write down the estimates and their standard errors.  How can you compute the 1% VaR? (Formula). Compute the 1% VaR of your financial position based on the fitted parameters. What is the 1% VaR of your financial position for the next 10 trading days?

### 3- Again, consider the log returns of the Amazon stock. Fit a generalized Pareto distribution to the return series with threshold 3.5%. Based on the fitted model, what is the 1% VaR of your position? What is the associated expected shortfall? Repeat the analysis using threshold 4.5%. Are the results sensitive to the choice of thresholds?

### 4- Consider the log returns of KO stock. 

A. Calculate the VaR using the RiskMetrics method for the next trading day on April 30, 2015. 

B. What is the VaR for the combined position of AMZN and KO stocks for the next trading day on April 30, 2015? (Using RiskMetrics method) 

C. Consider a new portfolio that holds a short position of $1 million in AMZN stock, but a long position of $1 million in KO stock. Obtain the VaR of the portfolio for the next trading day on April 30, 2015 if (a) RiskMetrics is used and (b) GARCH(1,1) models with standardized Student-t innovations are used. 

D. What is the VaR for the combined position of AMZN and KO (both long), for the next trading day on April 30, 2015, if we entertain time-varying correlations between the two stocks.

### 5- The goal is to study the daily log return and the volatility of Apple stock. Focus on the period from January 3, 2007 to April 30, 2015. You may download the daily open, high, low, close prices and related information from Yahoo via the quantmod package. The tick symbol is AAPL.Focus on the volatility of the daily log-returns. Use the data and n = 63 to compute the Yang and Zhang (2000) variance estimate 𝜎 of Section (3.15.2) of the textbook. Obtain a time plot of the annualized estimated volatility series. Build a linear time series model (ARMA) for the log-volatility series. Use the fitted model to produce 1-step to 5-step ahead forecasts of log-volatility at the forecast origin April 30, 2015. 

