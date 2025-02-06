# INF6027_Microsoft-Stock-Price-Analysis-Using-R

# Microsoft Stock Price Analysis Using R

This repository contains an analysis of Microsoft stock prices using historical financial data and machine learning techniques. The primary objective is to predict Microsoft's future stock prices (closing price) using a Random Forest model. Additionally, comparisons with a Multiple Linear Regression model are made to assess prediction performance.

## Repository Contents

- **MSFT.csv**: This file contains historical stock market data for Microsoft (MSFT), including columns such as Date, Low, Open, Volume, High, Close, and Adjusted Close.
- **Microsoft Stock Price Analysis Using R.R**: The R script that implements the data preprocessing, exploratory analysis, Random Forest model, hyperparameter tuning, and model evaluation.

## Requirements

Before running the code, ensure that you have the following R packages installed: 


```r
install.packages(c("tidyverse", "caret", "randomForest", "ranger", "ggplot2", "lubridate", "gridExtra", "forecast", "zoo"))

tidyverse: Data manipulation and visualization.

caret: Machine learning package for building models and tuning parameters.

randomForest: Implementation of the Random Forest algorithm.

ggplot2: Visualization package for creating high-quality plots.

lubridate: Handling date-time data efficiently.

gridExtra: For arranging multiple plots

forecast: For Time Series Analysis

zoo: Ensure this is included for moving averages


## Running the Code
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
Results

The script will preprocess the data, generate visualizations, train the Random Forest model, perform hyperparameter tuning, and output performance metrics such as RMSE, R², and MAE.

The final model will be evaluated using residual analysis, and the results of a paired t-test will show if the Random Forest model outperforms the Linear Regression model.

### **4.Visualizations**

High-quality visualizations of feature importance, residuals, and model performance are generated using ggplot2.

## Model Description

### Step-by-Step Breakdown

Data Preprocessing: The data is cleaned and prepared for model training by handling missing values and creating new features such as moving averages and daily returns.

Random Forest Model: A Random Forest model is trained to predict the closing stock price of Microsoft.

Feature Selection: Recursive Feature Elimination (RFE) is used to select the most relevant features for model prediction.

Hyperparameter Tuning: The model's hyperparameters are fine-tuned using grid search to improve performance.

Model Evaluation: Model performance is evaluated using various metrics (RMSE, R², MAE) and residual analysis.

### License

This repository is provided under the MIT License. See the LICENSE file for more information.




