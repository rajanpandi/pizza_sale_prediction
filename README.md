# pizza_sale_prediction

This project forecasts pizza sales by employing various time-series forecasting techniques. The primary purpose is to:

Predict future sales based on historical data.
Optimize ingredient stock levels to meet expected demand, based on the prediction results.
Project Structure
Data: Contains raw sales and ingredient data.
Models: Scripts or saved model files for ARIMA, SARIMAX, and LSTM.
Results: Predictions and evaluations.
Data Preparation
Data Collection: Gathered historical sales data and ingredients data for each type of pizza.
Data Cleaning: Processed data by:
Handling missing values.
Removing outliers and inconsistencies.
Formatting dates for time-series compatibility.
Feature Engineering:
Generated time-related features (e.g., day of the week, month).
Created features based on sales trends and seasonality.
Modeling
Three main models were evaluated for forecasting future sales:

ARIMA:

Applied for univariate time-series analysis.
Optimized using grid search for best-fit parameters.
SARIMAX:

Integrated external features to capture seasonality and exogenous factors.
Tuned seasonal parameters to improve forecasting accuracy.
LSTM (Long Short-Term Memory):

Implemented a deep learning approach to capture complex patterns in data.
Scaled and reshaped data to fit into the LSTM model.
Set up a sequential LSTM model with an output layer for future sales prediction.
Prediction and Inventory Planning
After obtaining the forecasted sales data, we utilized the predictions to:

Estimate Ingredient Requirements:
Mapped each predicted sale to the ingredient data to calculate the expected usage for each ingredient type.
Plan Inventory for Future Production:
Based on the projected demand, optimized ingredient stocking for efficient resource management.
