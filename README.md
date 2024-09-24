# Ethereum to Great British Pounds (GBP) Price Prediction

This repository contains the code and methodology for predicting the price of Ethereum (ETH) in Great British Pounds (GBP) using Long Short-Term Memory (LSTM) networks. The project focuses on analysing historical price data to forecast future Ethereum prices, providing valuable insights for cryptocurrency traders and financial analysts.

## Project Overview

Cryptocurrency prices, particularly Ethereum, are notoriously volatile and influenced by a myriad of factors. This project applies deep learning techniques, specifically LSTM, to predict Ethereum's closing price against GBP. The model captures the temporal dependencies in the data, enabling more accurate predictions based on historical price trends.

### Key Features:
- **Data Preprocessing**: Includes data cleaning, normalisation, and splitting into training and testing sets.
- **LSTM Model**: Uses PyTorch to implement an LSTM model, which is particularly suited for time-series data.
- **Model Evaluation**: The model is evaluated using key metrics such as Mean Absolute Percentage Error (MAPE) and R-squared (R²).
- **Visualisations**: Plots the training and testing performance, alongside predicted vs. actual prices.

## Methods and Model

The dataset used spans from **November 2017 to April 2024**, obtained from **Yahoo Finance**. The historical data includes Ethereum prices in GBP, with features such as:
- **Open**: Opening price
- **High**: Highest price during the day
- **Low**: Lowest price during the day
- **Close**: Closing price
- **Volume**: Total trading volume

The LSTM model processes sequential data, predicting future prices based on the preceding days' closing prices. The model uses the following architecture:
- **Input Size**: Single feature (Closing Price)
- **Hidden Size**: Configurable, with a default of 4
- **Layers**: Single stacked LSTM layer
- **Optimizer**: Adam optimiser

### Performance Metrics:
- **MAPE** (Mean Absolute Percentage Error)
- **R² Score** (Explained variance)

The model achieved the following performance:
- **MAPE on Test Data**: 2.18%
- **R² Score on Test Data**: 0.9845

## Visualisation

The notebook includes visualisations of both training and test performance, showing how well the model predicts Ethereum's price. It also provides a comparison between predicted and actual values, offering insights into the model's accuracy.

## Conclusion

The LSTM model demonstrated excellent performance in predicting Ethereum prices with a low MAPE and high R² score, making it a reliable tool for forecasting cryptocurrency prices. Future improvements could involve exploring more complex models or incorporating additional features like trading volume and market sentiment.

### License

This project is licensed under the MIT License.
