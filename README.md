# Stock_Price_prediction_LSTM

# Objective
This project aims to build an Multivariate time series prediction LSTM model to predict the stock price.
![image](https://github.com/ritikdhame/Stockprice_prediction_LSTM/assets/7029092/3e27c534-3d82-465c-9408-a20f60272e74)

# About the data
The code requires the following dataset from : https://finance.yahoo.com/quote/TSLA/history?period1=1528502400&period2=1686268800&interval=1d&filter=history&frequency=1d&includeAdjustedClose=true
The dataset contains :  Last 5 years of Tesla Share price on a daily basis with 1244 data points.

#  Requirements
To run the code, you need to install the following libraries:
- Plotly
- tendsorflow.Keras.layers
- Scikitlearn
-keras.optimizers 
- keras.model

# Algorithm 
- Stacked LSTM model

# Methodology
The code consists of 4 main parts:
- Data loading and exploration: invloves loading the data set using pandas and saving it in the dataset
- Preprocessing: Involves seperating dates for future prediction, and buidling a data frame with only relavant parameters : 'Open', 'High', 'Low', 'Close', 'Adj Close', followed by splitting the training data.
- Model building and training: This part using the keras libraries to build a single LSTM model with only 64 units followed by Stacked LSTM model with a hidden LSTM with 32 units and a dropout layer and using optimizer adam. We then track the loss function at every epoch and finally compare the loss function of both the training and validation loss.
- Prediction : Performing inverse transformation to rescale back to original range,Since we used 5 variables for transform and then plotting the stock price for the next 15 days.
![image](https://github.com/ritikdhame/Stockprice_prediction_LSTM/assets/7029092/ab5ebcd0-83d3-42eb-bdde-77e63d444b6a)

# Procedure
You can install them using pip or conda commands.
To run the code, you need to execute the following steps:

1. Import the required libraries.
2. Load and view the text and explore the data 
3. Define the layers of the LSTM model 
4. Building and fitting the model with keras package.
5. Predicting the stock price 
6. Evaluating and visualize the model performance using metrics and plots.

The code is commented and documented for better understanding and readability.
