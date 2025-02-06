# INF6027_Microsoft-Stock-Price-Analysis-Using-R Project


This repository contains an analysis of Microsoft stock prices using historical financial data and machine learning techniques. The primary objective is to predict Microsoft's future stock prices (closing price) using a Random Forest model. Additionally, comparisons with a Multiple Linear Regression model are made to assess prediction performance.


## Project Title: Enhancing Stock Price Prediction Using Machine Learning: A Comparative Analysis of Random Forest and Linear Regression Models on Microsoft's Financial Data 

### Research Aim
The primary aim of this research was to explore the historical stock price data of Microsoft Corporation, uncover patterns and relationships between financial 

indicators, and evaluate the effectiveness of machine learning models in predicting stock prices. 

The specific objectives were to:

1. Investigate the influence of financial indicators, such as High, Low, Open, and Volume on Microsoft’s closing price.

2. Develop predictive models, including Random Forest and Linear Regression, to forecast accuracy of future stock price.


## Research Questions

1. How do financial indicators, such as High, Low, and Volume, influence Microsoft’s closing price?

2. Can machine learning models, including Random Forest and Linear Regression, predict Microsoft’s future stock price with accuracy?

## Machine Learning Models (Predictive Modelling)
1. Random Forest Model
2. Linear Regression Model


## Key Findings  
-Key Finding 1: The predictors of Microsoft’s closing price which proved most influential were High and Low prices, having strong positive correlations over 0.95.

-Key Finding 2: Random Forest model exhibits excellent predictive accuracy with an R² = 0.9999 and good error metrics (MAE = 0.2499, RMSE = 0.6839).

-Key Finding 3: Linear Regression did relatively well, with identical R² values, but on the lower end of RMSE, that showed its inability to deal with complex interactions compared to Random Forest.

-Key Finding 4: The direct correlation of Volume indicator against price movements was weak and therefore the indicator has a very weak standalone predictive power.

-Key Finding 5: A paired t-test showed no statistically significant difference in prediction accuracy of Random Forest model from that of Linear Regression model (p = 0.1252).




## Repository Contents

- **MSFT.csv**: This file contains historical stock market data for Microsoft (MSFT), including columns such as Date, Low, Open, Volume, High, Close, and Adjusted Close.
- **Microsoft Stock Price Analysis Using R.R**: The R script that implements the data preprocessing, exploratory analysis, Random Forest model, hyperparameter tuning, and model evaluation.
- **Visualization Outputs**: 

## Requirements

Before running the code, ensure that you have the following R packages installed: 


install.packages(c("tidyverse", "caret", "randomForest", "ranger", "ggplot2", "lubridate", "gridExtra", "forecast", "zoo"))

tidyverse: Data manipulation and visualization.

caret: Machine learning package for building models and tuning parameters.

randomForest: Implementation of the Random Forest algorithm.

ggplot2: Visualization package for creating high-quality plots.

lubridate: Handling date-time data efficiently.

gridExtra: For arranging multiple plots

forecast: For Time Series Analysis

zoo: Ensure this is included for moving averages


## Steps for Running the Code
Follow these steps to run the code on your local machine:

## Download or Clone the Repository

You can either clone the repository using Git or download it as a ZIP file.

To clone the repository, run the following command in your terminal or Git Bash
git clone https://github.com/Richiealx/INF6027_Microsoft-Stock-Price-Analysis-Using-R.git

### 2. Load the Data and Script

Open RStudio or your preferred R environment.

Load the script Microsoft Stock Price Analysis Using R.R by either opening it directly from your file explorer or using the following command in R:

source("path/to/Microsoft Stock Price Analysis Using R.R")

### 3. Running the Analysis

Make sure the dataset MSFT.csv is in the same directory as the R script.

Run the entire script step by step or use source() to execute all commands in one go.


### 4. Results

The script will preprocess the data, generate visualizations, train the Random Forest model, perform hyperparameter tuning, and output performance metrics such as RMSE, R², and MAE.

The final model will be evaluated using residual analysis, and the results of a paired t-test will show if the Random Forest model outperforms the Linear Regression model.

### 5.Visualizations

High-quality visualizations of feature importance, residuals, and model performance are generated using ggplot2.

## Model Description

### Step-by-Step Breakdown

Data Preprocessing: The data is cleaned and prepared for model training by handling missing values and creating new features such as moving averages and daily returns.

Random Forest Model: A Random Forest model is trained to predict the closing stock price of Microsoft.

Feature Selection: Recursive Feature Elimination (RFE) is used to select the most relevant features for model prediction.

Hyperparameter Tuning: The model's hyperparameters are fine-tuned using grid search to improve performance.

Model Evaluation: Model performance is evaluated using various metrics (RMSE, R², MAE) and residual analysis.





