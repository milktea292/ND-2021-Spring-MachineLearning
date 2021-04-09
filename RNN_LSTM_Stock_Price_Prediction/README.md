## Deploy a RNN-LSTM model for predicting the NVDA stock price from 1999-2021

This work focused on deploying a RNN-LSTM model for predicting the NVDA stock price from 1999-2021.
For the dataset, I downloaded the csv file from https://finance.yahoo.com/quote/NVDA/history/. To make this mini-project simple, I only used 'Adj Close Price' as my datapoints. Here is the visualization of the dataset I used. This work splited the dataset into 60:20:20 for train:val:test, and used the n-prior days technique to deal with time-series regression problems.
<div style="text-align:center"><img src="./images/NVDA_dataset.jpg" width="500">

Here I used my 7-40-1 ANN model as an experiment, and explored different activation functions at hidden layers while setting activation function at output layer as relu.
<div style="text-align:center"><img src="./images/MSE_performance_ANN_diff_activation_functions_with_minmax_scalor.jpg" width="500">

## Data-Processing MinMax-Scaler are all applied in following results

### MSE performances of 7-40-1 ANN architectures on test dataset with different activation functions at the hidden layer
<div style="text-align:center"><img src="./images/MSE_performance_ANN_diff_activation_functions_with_minmax_scalor.jpg" width="500">
  
### MSE prediction performance of using RNN-LSTM architectures on test dataset 
<div style="text-align:center"><img src="./images/LSTM_MSE_performance_testing_with_minmax_scalor.jpg" width="500">

### Prediction on test dataset using ANN architectures with different activation functions at hidden layer 
<div style="text-align:center"><img src="./images/ANN_prediction_with_diff_activation_functions_with_minmax_scalor.jpg" width="500">
  
### Prediction on test dataset using RNN-LSTM architectures with different input layers
 <div style="text-align:center"><img src="./images/LSTM_Predictions_vs_GroundTruth_with_minmax_scaler.jpg" width="500">
  
here I just list 10-prior days' performances. For more info, feel free to check on my ipynb file
