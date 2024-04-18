# dsan5550-final-project
# Predicting Parent Company Stock Prices Based on Facility Carbon Emissions and Local Climate Data

## Project Overview

This project explores the complex relationship between regional climate conditions around factories and the daily stock prices of their parent companies. We hypothesize that local climate variables can serve as indicators of factory operational efficiency and affect production efficiency, business performance, and ultimately stock prices.

## Objective

To provide a nuanced understanding of how environmental conditions affect corporate operations and financial outcomes using advanced statistical and machine learning techniques.

## Data Sources

- **Climate Data**: Obtained from the Global Historical Climatology Network - Daily (GHCN-Daily), Version 3, provided by NOAA's National Centers for Environmental Information (NCEI).
- **Carbon Emissions Data**: Sourced from the Environmental Protection Agency's Greenhouse Gas Reporting Program (GHGRP).
- **Stock Price Data**: Collected from Yahoo Finance, covering 3,751 facilities and 423 U.S.-based companies.

## Methodology

1. **Data Collection and Refinement**: Align climate, emissions, and stock price data for comprehensive analysis.
2. **Statistical Analysis**: Explore correlations and decompose time series to understand stock price trends.
3. **Machine Learning Models**: Implement regression, ARIMA, and LSTM models for forecasting using key environmental predictors.
4. **Data Visualization**: Employ plots, heatmaps, and correlation matrices to represent the data relationships visually.

## Evaluation Metrics

- **Correlation Coefficients**
- **Mean Absolute Error (MAE)**
- **Root Mean Square Error (RMSE)**
- **R-squared (R²)**
- **Feature Importance Scores**

## Sustainability Commitment

We are mindful of our carbon footprint and will quantify the carbon impact of our computational models using CodeCarbon.

## Installation

```bash
# Clone this repository
git clone https://github.com/your-username/your-repo-name.git

# Navigate to the project directory
cd your-repo-name

# Install required dependencies
pip install -r requirements.txt
