# Air-Pollution-Forecasting
An LSTM model to predict the pollution levels in the next hour using the weather conditions and pollution levels in the current hour. I have trained the model using multi-variate(when we consider multiple features for prediction).

## Dataset
In this, I have used the Air Quality dataset. This is a dataset that reports on the weather and the level of pollution each hour for five years at the US embassy in Beijing, China. The data includes the date-time, pollution called PM2.5 concentration, and the weather information including dew point, temperature, pressure, wind direction, wind speed and the cumulative number of hours of snow and rain. 

## Steps followed
- Data preparation
- Data visualization
- LSTM data preparation
- Fit the model 
- Evaluate the model

### Data preparation
- Replaced NA values
- Parsed date-time into pandas dataframe index
- Specified clear names for each columns

### LSTM data preparation
- Normalized data
- Transformed dataset into supervised learning problem by using slicing window method/lag method.

### Model Fitting
- Splited data into train and test
- Reshaped into 3D
- Defined LSTM with 50 neurons in the first hidden layer and 1 neuron in the output layer for predicting pollution
- Added dropout at 20% after every layer

### Evaluate model
- Make prediction
- Invert scaling
- Ploted the loss graph.
- Ploted the line graph between actual vs predicted values
- Calculated RMSE(root mean squared errot) and MAPE(mean absolute percentage error)
