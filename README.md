# Stock Price Prediction 
A minor project where I utilized two models - Liear Regression and LSTM for predicting closing price of stocks. 

## Dataset Description :

**Open** - The price the stock opened at.<br/>
**High** - The highest price during the day.</br>
**Low** - The lowest price during the day.</br>
**Close** - The closing price on the trading day.</br>
**Adj Close** - The price of the stock after paying off the dividends.</br>
**Volume** - How many shares were traded.</br>

## Data Preparation 
Data Preparing for Linear Regression is pretty straightforward , I set my target as close column and rest other were used as features . I also derived few other features like Day, Month etc which I beleived 
were relevant for this dataset

## Splitting the Dataset 
Splitting a time series data is different in the sense that we cannot randomly split the time series data as it can break the time series and can cause future values to be known by our model while trainig. 
That's why I used sequential splitting.

## Results
The mae for linear Regression was : **137.64** , proving that it isn't the best model for predicting something like stock market <br>

The mae for LSTM model was : **22.22** , which is not very decent but way better than our Linear Regression Model 

## Conclusion 
The LSTM model in its bare state was able to capture the trend quite decently. 

## Future Updates 
In future my plan is testing out other models like ARIMA , AutoReg,GARCH etc to see how they compare with the previous result

