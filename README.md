# telemetry_servers

## Dataset

[[microsoft-azure-predictive-maintenance](https://www.kaggle.com/datasets/arnabbiswas1/microsoft-azure-predictive-maintenance)](https://www.kaggle.com/datasets/arnabbiswas1/microsoft-azure-predictive-maintenance)

Objective:
To predict the date on which a given server may fail, having as input the periodic (time series) telemetry information available from Azure cloud servers and failures recorded on given dates.

Development:
After exploring the data and according to the reviewed documentation, recurrent neural network models are chosen, which are the most suitable to develop the problem. The reasons for choosing this type of neural network model are because the data are periodically given in fixed time, time series, and the predictors are very unbalanced, which can be a big problem when using a predictor layer at the end of our neural network. our neural network.

Deep learning models: 
A function is defined to provide a neural network model, the function provides one of the 3 common types of neural networks used in time series: SimpleRNN, LSTM and GRU. The data were evaluated with these 3 types of neural networks varying the backward observation times from 1 to 5. For each combination the RMSE performance metric is obtained to determine which combination is the best.




