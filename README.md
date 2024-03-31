Stock Price Prediction Model
Overview
This project aims to predict the closing price of a stock using historical stock price data and machine learning techniques. The model utilizes features such as open, high, low, close prices, volume, 50-day moving average, and 200-day moving average to predict the closing price of a stock for the next day.

Dependencies

Pandas: For data manipulation and analysis.

yfinance: For fetching historical stock price data.

scikit-learn: For implementing machine learning models and evaluating performance metrics.

datetime: For handling date and time operations.

Dataset The historical stock price data is fetched using the yfinance library for a specified ticker symbol and time period. Features such as open, high, low, close prices, volume, 50-day moving average, and 200-day moving average are extracted from the dataset.

Feature Engineering
Moving averages (50-day and 200-day) are calculated as additional features to provide trend information. Missing values are filled using the forward-fill method.

Model Training
The dataset is split into training and testing sets using the train_test_split function from scikit-learn. A Linear Regression model is trained on the training data to learn the relationship between the input features and the target variable (closing price).

Model Evaluation
The trained model is evaluated on the testing set using various performance metrics such as R-squared score, Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE). These metrics provide insights into the accuracy and reliability of the model's predictions.

Usage To use the model, follow these steps:
Install the required dependencies listed in the Dependencies section. Run the provided Python script to train the model and make predictions. Adjust the parameters such as ticker symbol, start date, and end date as needed. Evaluate the model's performance metrics to assess its accuracy.
​
