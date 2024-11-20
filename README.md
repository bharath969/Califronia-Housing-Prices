# California Housing Prices Prediction

## Problem Statement

The goal is to `predict the median house value` of a property in `California` based on various attributes such as geographical location, size, and economic factors.

The dataset includes the following features:
- **Longitude:** The geographic coordinate representing the house's location.
- **Latitude:** The geographic coordinate representing the house's location.
- **Housing Median Age:** The age of the house.
- **Total Rooms:** The total number of rooms in the house.
- **Total Bedrooms:** The total number of bedrooms in the house.
- **Population:** The population of the area where the house is located.
- **Households:** The number of households in the area.
- **Median Income:** The median income of households in the area.
- **Ocean Proximity:** A categorical feature indicating the proximity of the house to the ocean (e.g., "NEAR OCEAN", "INLAND", etc.).

The task is to develop a machine learning model that can accurately predict the median house value based on these features.

---

## Solution Overview

This project involves a systematic approach to analyze the dataset and build a predictive model for house prices. The following steps were undertaken:

1. **Data Understanding**: 
   - Investigated the dataset to understand the features and the target variable (`median_house_value`).
   - Explored relationships between variables such as `ocean_proximity`, income levels, and house prices.

2. **Data Preprocessing**:
   - Handled missing values to ensure data consistency.
   - Encoded categorical variables, including `ocean_proximity`, using techniques like one-hot encoding.
   - Scaled numerical features to prepare them for machine learning models.

3. **Exploratory Data Analysis (EDA)**:
   - Visualized patterns and correlations between features and house prices.
   - Identified key factors affecting housing prices, such as proximity to the ocean and average income levels.

4. **Model Development**:
   - Built and trained a regression model using deep learning techniques with TensorFlow and Keras.
   - Used Ensemble method to group different regressors for the better outcome
   - Evaluated the model's performance using metrics such as **Mean Absolute Error (MAE)** and **R^2**.
   - Used GridSearch to predict the best model and its parameters
5. **Predictions**:
   - Used the trained model to predict house prices for unseen data.
   - Validated the model's reliability by comparing predicted values to actual prices.

---

## Key Highlights
- #### Model Performance Comparison

The table below summarizes the performance of various regression models used for predicting California housing prices:

| Model                         | Mean Absolute Error (MAE) | Score (R²)      |
|-------------------------------|---------------------------|-----------------|
| `LinearRegression()`          | 50,976.30                | 0.6201          |
| `SVR()`                       | 86,797.11                | -0.0400         |
| `RandomForestRegressor()`     | 43,122.17                | 0.7045          |
| `VotingRegressor()`           | 45,088.27                | 0.6917          |
| `ANN`                         | 47,434.75 (Validation)   | N/A             |

---

## Observations
- As the **RandomForestRegressor** achieved the best performance with the lowest MAE (43,122.17) and the highest R² score (0.7045), we used this model to predict our future prices

---


