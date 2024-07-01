# prophet-challenge

Step 1: Collect the Data
Google Search Data: Use the pytrends library to collect search traffic data for the keyword "MercadoLibre" from Google Trends.
Stock Price Data: Obtain stock price data for MercadoLibre from a reliable source such as Yahoo Finance.
Step 2: Mine the Search Traffic Data for Seasonality
Plot the Search Traffic Data: Visualize the search traffic data to identify patterns and seasonality.
Decompose the Data: Use time series decomposition to break down the search traffic data into trend, seasonal, and residual components.
Step 3: Relate the Search Traffic to Stock Price Patterns
Read and Plot Stock Price Data: Import the stock price data and visualize it.
Concatenate Data: Combine the search traffic data and stock price data into a single DataFrame.
Create Lagged Search Trends: Create a new column that shifts the search traffic data by one hour to explore lagged effects.
Calculate Stock Volatility: Add a column for stock volatility, using a four-hour rolling average of stock price returns.
Calculate Hourly Stock Return: Add a column for hourly stock returns.
Step 4: Analyze Correlations
Correlation Table: Construct a correlation table to identify relationships between search traffic, stock volatility, and stock returns.
Time Series Correlation: Visualize the time series correlation to further analyze the relationships.
Step 5: Forecast with Prophet
Prepare Data for Prophet: Set up the search traffic data for use with the Prophet forecasting model.
Fit the Model: Train the Prophet model on the search traffic data.
Make Predictions: Use the model to predict future search traffic trends.
Visualize Predictions: Plot the forecast results and the individual components (trend, weekly, yearly, daily).
Results and Interpretation
Correlation Analysis
There is a notable correlation between search traffic and stock price returns, suggesting that changes in search traffic may predict stock price movements.
Stock volatility shows significant spikes during periods of high search traffic, indicating that search trends can influence market behavior.
Forecasting Analysis
Near-Term Forecast: The model predicts an increase in search traffic for MercadoLibre in the near term.
Time of Day Popularity: Search traffic is highest during the late afternoon and early evening hours.
Day of Week Popularity: Search traffic peaks on Mondays and decreases towards the weekend.
Lowest Search Traffic Point: The lowest search traffic occurs in early January, likely due to post-holiday season effects.
