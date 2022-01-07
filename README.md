# google_trend_sarima
A set of analytical model to smooth trends, determine seasonality and predict future search frequency of specific keywords

The model main steps:
- Pull the time-series data with Google Trend API 
- Use STL decomposition to break down to trend and seasonality component of the time-series
- Check the stationarity of the residuals by Augmented Dickey-Fuller test
- Grid search to find the optimal order for the SARIMA model
- Predict the future outcome
