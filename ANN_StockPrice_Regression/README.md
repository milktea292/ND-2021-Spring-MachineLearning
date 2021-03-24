## Design an ANN model for predicting stock price

This work focused on designing an ANN model to predict NVDA stock price. 
For the dataset, I download the csv file from https://finance.yahoo.com/quote/NVDA/history/. To make this mini-project simple, I only use 'Adj Close Price' as my datapoints. Here is the visualization of the dataset. This work splited this dataset into 60:20:20 for train:val:test, and used n-prior days technique to deal with time-series regression problems.
<div style="text-align:center"><img src="./images/NVDA_dataset.jpg" width="500">

### Using Principal Component 1 and Principal Component 2 for Analysis
(distinguished by population)
<div style="text-align:center"><img src="./Images/pic1.png" width="500">

### Using Principal Component 1 and Principal Component 3 for Analysis 
(distinguished by gender 1 = male / 2 = female)

<div style="text-align:center"><img src="./Images/pic2.png" width="500">

### Using Principal Component 1 and Principal Component 4 for Analysis 
(distinguished by population)

<div style="text-align:center"><img src="./Images/pic3.png" width="500">

For more details feel free to check the .ipynb file.
