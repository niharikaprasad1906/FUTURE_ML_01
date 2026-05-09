Sales Forecasting with Linear Regression

Overview
This project demonstrates a simple sales forecasting solution using a Linear Regression model. It involves loading sales data, performing essential data preprocessing, feature engineering, training a linear regression model, and visualizing the actual, predicted, and forecasted sales.

Data Source
The project utilizes a 'Sample - Superstore.csv' dataset, which contains sales and order information.

Methodology
The forecasting process involves the following steps:

Data Loading: The dataset is loaded into a pandas DataFrame, with 'Order Date' parsed as datetime objects. 

Data Cleaning: Missing values are handled by dropping rows, and the data is sorted by 'Order Date' to prepare for time-series analysis.

Feature Engineering: New time-based features (year, month, day, day of week) are extracted from the 'Order Date'. Monthly sales are aggregated using resample('ME').

Model Training: A LinearRegression model from sklearn is trained on the monthly sales data, using a time index as the independent variable.

Prediction and Forecasting: The trained model generates predictions for a test set and forecasts sales for future periods.

Visualization: The actual sales, test set predictions, and future forecasts are plotted to provide a clear overview of the model's performance and future outlook.

Model
The core of the forecasting is a LinearRegression model, chosen for its simplicity and interpretability in demonstrating basic time-series forecasting concepts.

How to Run
To run this notebook and replicate the analysis:

Upload Data: Ensure you have a Sample - Superstore.csv file in your Colab environment or update the file path in the 'Reading file' cell.
Execute Cells: Run all the cells in the notebook sequentially. The notebook is designed to be executed from top to bottom.
Review Output: Observe the printed outputs and visualizations to understand the data, model performance, and sales forecasts.
Libraries Used:
pandas for data manipulation.
matplotlib.pyplot for data visualization.
sklearn for machine learning models (Linear Regression and train_test_split).
