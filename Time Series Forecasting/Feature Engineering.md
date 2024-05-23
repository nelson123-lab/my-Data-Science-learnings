1. **Data Related Features**: These features are derived from the original data itself, such as values of the time series at each time step. They often include transformations or decompositions of the original data, like seasonality and trend components.

2. **Time Based Features**: These features are extracted from the timestamp of the data points, such as the hour, minute, day, month, or day of the week. They help capture the periodic patterns and seasonality effects in the data.

3. **Lag Features**: Lag features are past values of the time series used as predictors for future values. For example, the value of a time series at time \( t-1 \) or \( t-2 \) can be used to predict the value at time \( t \).

4. **Rolling Features**: These features are computed using a rolling window over the time series, such as the moving average or moving standard deviation over a specified window size. They capture the local trends and variability in the data over time.

5. **Expanding Window Features**: These features are calculated using all data points up to the current time step, such as the cumulative mean or cumulative sum. They provide insights into the overall trend and long-term patterns of the series.

6. **Domain Specific Features**: These are features that are specific to the domain or context of the time series data, such as holidays, promotional events, or weather conditions in sales forecasting. They capture external factors that can influence the time series beyond its historical patterns.
