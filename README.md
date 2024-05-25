# Sector-Analyis
**Overview**
This project aims to predict future values of Nifty indices using macroeconomic variables such as GDP and inflation. We utilize the SARIMAX (Seasonal AutoRegressive Integrated Moving Average with eXogenous regressors) model for time series forecasting. The focus is on predicting the Nifty Auto index, but the approach can be extended to other indices as well.

**Data Sources**
The data used in this project include:

Nifty Indices Data: Historical data for various Nifty indices obtained from Yahoo Finance.
Macroeconomic Data: GDP and inflation data.
Nifty Indices
**The Nifty indices considered in this project are:**

NIFTY FIFTY
Nifty Auto
Nifty FMCG
Nifty IT
Nifty Media
Nifty Metal
Nifty Realty
**Macroeconomic Variables**
GDP (Billions of US $)
Inflation Rate (%)
Steps
Data Collection:

Fetch historical data for Nifty indices using Yahoo Finance.
Load GDP and inflation data from CSV files.
Data Preprocessing:

Convert the 'Date' columns to datetime format.
Ensure all datasets have a consistent time format.
Resample the Nifty indices data to yearly frequency to match the macroeconomic data.
Shift macroeconomic data by one year to use the previous year's data for prediction.
Data Merging:

Merge Nifty indices data with macroeconomic data on the 'Date' column.
Ensure all necessary columns are numeric and handle missing values.
Model Training and Prediction:

**Use the SARIMAX model to predict the Nifty Auto index.**
Split the data into training and test sets.
Fit the SARIMAX model on the training data.
Make predictions on the test data.
Model Evaluation:

Calculate the mean squared error (MSE) of the predictions.
Plot the actual vs. predicted values.
**Issues and Considerations**
Data Alignment: Ensure that the Nifty indices and macroeconomic data are aligned correctly on the date.
Missing Values: Handle missing values appropriately to avoid issues during model training.
