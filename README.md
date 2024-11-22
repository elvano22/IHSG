# IHSG

## Project Overview
This repository contains the final project for a time series analysis on the Indonesia Stock Exchange (IHSG). The primary goal of this analysis is to explore and predict movements in the IHSG (Indeks Harga Saham Gabungan), which represents the composite stock index in Indonesia. The repository includes code, data, and a detailed explanation of different predictive models used for time series forecasting.

## Repository Structure
- **Dataset IHSG.csv**: This dataset contains historical data of the IHSG, which will be used to build and test prediction models.
- **Other Prediction Model.Rmd**: This R markdown file contains scripts for analyzing the time series using different approaches. It provides a detailed and reproducible workflow to preprocess the data, train models, and evaluate their performance.
- **Manual Prediction Model.xlsx**: This Excel file outlines a manual approach to making predictions. It contains various sheets and calculations that help illustrate different prediction techniques step-by-step.
- **Other Prediction Model.html**: This file is an HTML document generated from the R markdown, offering a comprehensive report of the models used, their assumptions, and the overall findings of the analysis.

## Analysis Summary
The analysis focused on the prediction of the IHSG index, a crucial indicator for investors and economists. The methods used in this study included:

1. **Time Series Decomposition**: The data was decomposed into trend, seasonality, and residuals. This allowed the team to understand the fundamental structure of the IHSG data, highlighting long-term movements and regular patterns.

2. **ARIMA Model**: The Auto-Regressive Integrated Moving Average (ARIMA) model was used to forecast the future values of the IHSG index. ARIMA is particularly useful for handling data with trends and seasonality, and it performed well when tested against the historical data.

3. **Exponential Smoothing**: Another model applied was Exponential Smoothing, which is effective for capturing trends and seasonal variations in time series data. This method was also tested and evaluated for accuracy.

4. **Performance Evaluation**: Each model was evaluated using metrics like **Mean Absolute Error (MAE)**, **Root Mean Squared Error (RMSE)**, and **Mean Absolute Percentage Error (MAPE)**. The comparison showed that ARIMA produced the lowest RMSE, indicating better predictive performance compared to other models used.

5. **Manual Calculations**: The Excel file provides step-by-step manual calculations of different prediction models. These calculations serve as a validation tool and help in understanding the model mechanics.

## Key Findings
- The **ARIMA model** was found to be the most suitable for predicting IHSG, owing to its capability to handle trends and noise in financial data.
- Seasonal trends were identified in the IHSG dataset, and the models captured these variations effectively, contributing to more accurate forecasts.
- The **manual predictions** in the Excel file aligned well with the outputs from the automated models, providing an additional layer of validation.

## Conclusion
The paper concluded that the ARIMA model is a robust tool for predicting the IHSG index due to its effective handling of both trend and noise components inherent in financial time series data. The inclusion of seasonal trends further improved prediction accuracy, highlighting the importance of capturing periodic behaviors in financial markets. Overall, the models demonstrated reliable forecasting capabilities, providing valuable insights for investors and economic analysts regarding future movements in the IHSG.

## How to Use This Repository
1. **Data Exploration**: Start by exploring the dataset (Dataset IHSG.csv) to understand its structure and key variables.
2. **Run Analysis**: Use `Other Prediction Model.Rmd` to run the analysis and create visualizations. This R markdown file contains all the steps, from data cleaning to model training and evaluation.
4. **Traditional Method**: Use `Manual Prediction Model.xlsx` to calculate the time series prediction with traditional method.

## Dependencies
- R with the following libraries: **forecast**, **ggplot2**, **tseries**, and **dplyr**.
- A spreadsheet editor like Microsoft Excel or Google Sheets.

For further questions, suggestions, or contributions, feel free to open an issue or create a pull request.
