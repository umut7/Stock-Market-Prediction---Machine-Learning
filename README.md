# S&P 500 Financial Time Series Prediction
This project demonstrates the process of predicting future stock price trends using historical data from the S&P 500 index. The data is sourced using the yfinance library, and a machine learning model is applied to predict whether the stock price will rise or fall.

## Project Overview
Data Collection: Historical data for the S&P 500 index is downloaded using yfinance. This includes features such as opening price, closing price, highest price, lowest price, volume, and more.

Data Preprocessing: The dataset is cleaned and prepared by removing irrelevant columns (e.g., dividends, stock splits). Additional features are created for prediction, such as rolling averages over different time horizons and trends.

Modeling: A Random Forest Classifier is trained to predict the direction of the stock price movement (up or down) based on a set of predictors such as Close, Open, High, Low, and Volume.

Evaluation: The model's performance is evaluated using metrics like precision score. Additionally, a custom backtesting function is implemented to assess the model’s performance over time.

Feature Engineering: Rolling averages and trends for various horizons (2, 5, 60, 250, and 1000 days) are calculated and added as new predictors to improve the model's performance.

## Results
The Random Forest Classifier was able to predict the stock price movements with a precision score of approximately 57% in the test set. Feature engineering with rolling averages and trends improved the overall model performance.

## Technologies
pandas
yfinance
scikit-learn
matplotlib
