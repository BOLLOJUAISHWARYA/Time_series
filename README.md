# Air-Pollution-Forecasting
To predict the pollution levels in the next hour using the weather conditions and pollution levels in the current hour. 

## Dataset
In this, I have used the Air Quality dataset. This is a dataset that reports on the weather and the level of pollution each hour for five years at the US embassy in Beijing, China. The data includes the date-time, pollution called PM2.5 concentration, and the weather information including dew point, temperature, pressure, wind direction, wind speed and the cumulative number of hours of snow and rain. 

## Steps followed
- Data preparation
- Data visualization
- Model Building 
- Forecasting

### Data preparation
- Replaced NA values
- Parsed date-time into pandas dataframe index
- Specified clear names for each columns
- Normalized data
- Transformed dataset into supervised learning problem by using slicing window method/lag method.

### Model Building
- Splited data into train and test
- Reshaped into 3D
- Defined LSTM with 50 neurons in the first hidden layer and 1 neuron in the output layer for predicting pollution
- Added dropout at 20% after every layer

- Defined GRU with 50 neurons in the first hidden layer and 1 neuron in the output layer for predicting pollution

### Forecasting
- Make prediction
- Invert scaling
- Ploted the loss graph.
- Ploted the line graph between actual vs predicted values
- Calculated RMSE(root mean squared errot) and MAPE(mean absolute percentage error)
