# solar_panel_prediction
Prediction of next-minute solar generation using 3 different models.

Given a year's worth of minute-by-minute solar generation data from a solar panel system, I tested the accuracy of three different models for predicting the solar generation at the next minute. The three models were:
1. **Persistence**: predict the same value as the last seen value.
2. **Linear regression**: determine the line of best fit for the last *w* (w = window size) data points and use that line to predict the next value. Different window sizes were tested to determine the best option.
3. **Autoregressive Integrated Moving Average (ARIMA)**: uses combinations of historical data to explain variations and predict the next value.

After testing the models on the original data, I then grouped the data into differnet resolutions to test the effect of that on accruacy for the three models.
