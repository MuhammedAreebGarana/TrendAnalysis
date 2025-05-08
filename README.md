This project analyzes historical U.S. baby name data using time series forecasting, clustering, and change point detection techniques. The goal is to understand naming trends and forecast future popularity patterns using statistical and machine learning methods.

🧠 Technical Overview
1. Gender-Specific ARIMA Forecasting
Time series were grouped by gender and aggregated by year.

Stationarity was checked using the Augmented Dickey-Fuller test.

ARIMA (AutoRegressive Integrated Moving Average) models were trained separately for boys and girls to forecast name frequency.

Model selection was based on AIC and residual diagnostics.

2. Prophet Forecasting for Individual Names
For selected popular names, Meta’s Prophet was used to model trends and seasonality.

Prophet handled yearly seasonality and changepoints automatically.

Forecasts included uncertainty intervals and visual diagnostics.

3. Clustering of Name Trends
Time series data was transformed into feature vectors using trend-based summaries or raw counts over years.

K-Means clustering was applied to identify groups of names with similar temporal patterns.

PCA was optionally used for dimensionality reduction before clustering.

4. Changepoint Detection
Applied Ruptures to detect structural changes in name popularity trends.

Techniques such as Pelt and Binseg algorithms were used for identifying change points in selected name series.

Helps highlight cultural or societal shifts affecting naming preferences.
