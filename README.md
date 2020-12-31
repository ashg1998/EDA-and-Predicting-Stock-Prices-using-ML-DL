# EDA-and-Predicting-Stock-Prices-using-ML-DL
** In this project we will train a Ridge Regression Model  and Deep Neural Network Model to predict the future Stock Price.
** By accurately predicting stock price , the investor can maximize returns and know when buy/sell securities.
** The AI/ML model will be trained using historic stock price data , along with the volume of transactions.
** We will use a type of Neural Network known as LSTM(Long Short Term Memory).

First Visualizing the dataset:
Stock Prize:
![alt text](https://github.com/ashg1998/EDA-and-Predicting-Stock-Prices-using-ML-DL/blob/main/Capture1.JPG)
Stock Volume Prize:
![alt text](https://github.com/ashg1998/EDA-and-Predicting-Stock-Prices-using-ML-DL/blob/main/images/Capture2.JPG)

 Preparing the Dataset:
 step 1: individual_stock()
 This function returns a new dataset containing closing price and volume of the given Company
 step 2: trading_window()
 This function add a new column target , which contains the next day price. This target column is used as output or y_train for X training data.
 step 3:We remove the last row which contains Nan values in target Column.
 step 4: We use MinMaxScalar() to scale down all the values from 0 to 1 range.
 step 5: We keep stock price and volume in X and target in y.
 step 6: We split the data in X_train ,y_train, X_test,y_test in 65% : 35%.
 
 Training the Model:
 1. We used Ridge model to predict the future stock price.
 Result for Apple Company Stocks.
![alt text](https://github.com/ashg1998/EDA-and-Predicting-Stock-Prices-using-ML-DL/blob/main/images/Capture3AAPL.JPG)
2. We switched LSTM Model.
LSTM Model:
![alt text](https://github.com/ashg1998/EDA-and-Predicting-Stock-Prices-using-ML-DL/blob/main/images/Model_Summary.jpg)
 Result for SP500 Company Stocks.
![alt text](https://github.com/ashg1998/EDA-and-Predicting-Stock-Prices-using-ML-DL/blob/main/images/Capture4LSTMSP500.JPG)
Result for Amazon Company Stocks.
![alt text](https://github.com/ashg1998/EDA-and-Predicting-Stock-Prices-using-ML-DL/blob/main/images/Capture5LSTMAmazon.JPG)

