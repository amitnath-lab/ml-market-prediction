It will be interesting to see how machine learning can predict forex markets based on fundamental and sentiment data.

# Download training data
The training data were exported using MT4 software. This data is uploaded and hosted in GCP

# Feature Engineering
Involves generating technical analysis and different indicator data from values using TA lib http://ta-lib.org/. TA lib has wrapper for python and includes methods for 200+ indicators such as ADX, MACD, RSI, Stochastic, Bollinger Bands etc...

# Generate Performance Targets
Targets are genearted as trading signal. If the price is 200 pips higher after 5 periods then a trading signal is generated.

# Generate Training and Validation Examples
Determine Training/Test data
Since we are doing time series analysis, our training and test data have to be continuous in date, otherwise we will not be able to evaluate our trading strategy. I decided to use market data from 01/01/2018 to 12/31/2018 as our training set, and data from 01/01/2016 to 12/31/2017 as our test set.

# Model Trainings
We will experiment with different methods here like logistic regression.

# Model Deployment
Will use joblib to dump model here.
