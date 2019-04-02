# Global Land Temperature Forecast

Summary

This project is done as part of Advanced Data Science with IBM specialization https://www.coursera.org/specializations/advanced-data-science-ibm

You can also look at this youtube video I made for the project.
https://www.youtube.com/watch?v=gJ3AFoDxMf4&feature=youtu.be

In this project I perform forecasting of global land temperature for the next 1-month and for next 12-months given history of 1-month and 12-months respectively. I use one deep learning algorithm (Single layer LSTM neural network) and one supervised learning algorithm (Gradient Boosted Regressor). I used two performance metrics to judge the forecast results, namely root mean squared error and mean absolute error. Finally, according to my analysis 1-month forecast is better done by using single layer-LSTM model and 12-month forecast is better done by Gradient Boosted Regressor. But, in both cases the forecast was done to a decent agreement level.

Note: I found the feature scaling (Max-Min Scaler) is needed to get the best results.
https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.MinMaxScaler.html 

For step-by-step detailed description please follow the python notebooks in this repository. I have also added an Architecture Design Document (ADD) to describe the workflow in this project.

1. Data Cleaning: Data_cleaning.ipynb

2. Data Visualisation: Data Visualisation.ipynb

3. Supervised Learning Model, Gradient Boosted Regressor: 

i. No feature scaling: Gradient_boost_forecasting.ipynb

ii. Max-Min feature scaling: Gradient_boost_forecasting_MaxMinScaled.ipynb

4. Deep Learning Model, LSTM (Long Short-term Memory Neural Network): 

i. No feature scaling: LSTM_forecasting.ipynb

ii. Max-Min feature scaling: LSTM_forecasting_MaxMinScaled.ipynb

### Data Source: Berkeley earth 
url: http://berkeleyearth.lbl.gov/auto/Global/Complete_TAVG_complete.txt
