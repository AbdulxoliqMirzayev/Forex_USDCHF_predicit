# Forex_USDCHF_predicit

# USD/CHF Price Prediction Model

## Project Overview
This project develops a machine learning model to predict the future prices of the USD/CHF currency pair. Using historical data from 2020 to 2024, we employ the RandomForestRegressor, a robust ensemble learning method, to forecast future price movements based on observed trends. The model is designed to assist traders and financial analysts in making informed decisions by predicting the direction of the currency exchange rate.

## Technical Details
### Data Preparation
The dataset comprises daily price movements (open, high, low, close) and percentage changes. Initial steps involve cleaning the data by removing unnecessary columns and converting data types for analysis. We also create new features, such as moving averages (10-day and 50-day), which are commonly used in trading to detect price trends.

### Model Development
We use the RandomForestRegressor due to its effectiveness in handling non-linear data and its ability to provide a high level of accuracy without extensive hyperparameter tuning. The model is trained on features including daily prices, moving averages, and changes in percentages to predict the next day's closing price.

### Training Process
The data is split into training and testing sets, with 80% used for training and 20% for testing to evaluate the model's performance. The model is trained using historical data, and its performance is validated on unseen test data to ensure it generalizes well to new data.

## Results and Accuracy
The model's accuracy is evaluated using the Mean Squared Error (MSE) metric, which measures the average of the squares of the errors—that is, the average squared difference between the estimated values and the actual value. A lower MSE value indicates a model with higher accuracy. Additionally, we plot both the actual and predicted prices to visually assess the model's performance. These plots provide a clear comparison between the model's predictions and the real market prices, highlighting the effectiveness of the model in forecasting price trends.

## Conclusion
The RandomForestRegressor model has proven to be highly effective in predicting the USD/CHF currency pair's future prices. This model serves as a valuable tool for traders who need accurate and timely predictions to make strategic trading decisions. Future enhancements can include integrating more complex features and exploring more advanced machine learning techniques to further improve the model's accuracy.

## Usage
To run the model and see the predictions, execute the Python scripts included in the repository following the instructions in the Installation section. Ensure all dependencies are installed, and use the provided datasets.

For further inquiries or contributions to the project, please refer to the contributing guidelines or contact the repository maintainers.
