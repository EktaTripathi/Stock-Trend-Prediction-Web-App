# Stock-Trend-Prediction-Web-App
This project utilizes Long Short-Term Memory (LSTM) networks to predict stock trends based on historical stock price data. It includes two main components: a Jupyter notebook for model training and a Streamlit web application for interactive stock trend prediction.

# Jupyter Notebook (stock_trend.ipynb)
- Data Collection: Uses the Yahoo Finance API to retrieve historical stock price data for a specified stock (e.g., AAPL) from 2010 to 2023.
- Data Preprocessing: Cleans the data, calculates moving averages (100-day and 200-day), and scales the data using MinMaxScaler.
- Model Building: Constructs an LSTM neural network model using Keras, with four LSTM layers (50, 60, 80, and 120 units), dropout layers for regularization, and a Dense output layer.
- Model Training: Trains the LSTM model on the training data (70% of the dataset) for 50 epochs.
- Model Evaluation: Evaluates the model's performance on the test data (30% of the dataset) and scales back the predictions for comparison with the original prices.
- Model Saving: Saves the trained LSTM model as a .h5 file for later use.

# Streamlit Web Application (app.py)
- User Input: Allows users to input a stock ticker symbol to retrieve and analyze its historical stock price data.
- Data Visualization: Displays descriptive statistics of the data and visualizes the closing price over time, along with the 100-day and 200-day moving averages.
- Model Loading: Loads the pre-trained LSTM model to make predictions on future stock prices.
- Prediction Visualization: Shows the predicted stock prices compared to the original prices, allowing users to assess the model's accuracy.

# Dependencies
- NumPy
- Pandas
- Matplotlib
- Pandas Datareader
- yfinance
- TensorFlow
- Streamlit
  
# Usage
1. Run stock_prediction.ipynb to train the LSTM model and save it.
2. Run stock_prediction_app.py to start the Streamlit web application.
3. Enter the desired stock ticker to view historical data, moving averages, and predicted vs. actual prices.

# Output
## Enter Stock Prediction

The Enter Stock Prediction" feature allows users to input a stock ticker symbol of their choice. Once entered, the application retrieves historical data for the specified stock and utilizes a pre-trained LSTM neural network model to predict future stock prices.

![stock trend(1)](https://github.com/EktaTripathi/Stock-Trend-Prediction-Web-App/assets/94041887/b637c4c7-6d61-4f6d-bab9-ae13cea09545)

## Closing Price vs Time Chart
The "Closing Price vs Time Chart" feature provides users with a graphical representation of the closing prices of a selected stock over time. This visualization allows users to observe the trend and fluctuations in the stock's closing prices throughout the specified historical period.
![stock trend(2)](https://github.com/EktaTripathi/Stock-Trend-Prediction-Web-App/assets/94041887/4d3c2090-c8dc-4649-8c9d-7f01d43ba8cc)

# Predictions vs Original
The "Predictions vs Original" feature offers a comparative visualization of predicted and actual stock prices. This side-by-side comparison allows users to evaluate the accuracy and reliability of the LSTM neural network model used for predicting future stock prices based on historical data.

![stock trend(5)](https://github.com/EktaTripathi/Stock-Trend-Prediction-Web-App/assets/94041887/d6b7a3fb-412e-413b-9946-4e1058213ff8)
