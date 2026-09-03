# Bengaluru House Price Prediction using Keras

## Overview
This repository contains an end-to-end Deep Learning regression project aimed at predicting house prices in Bengaluru. The model is built using a Fully Connected Neural Network (FCNN) via TensorFlow and Keras, focusing on robust data preprocessing and accurate continuous value prediction.

## Dataset
The project utilizes the `bengaluru_house_prices.csv` dataset, which includes real estate features such as:
* **Location:** Neighborhood in Bengaluru.
* **Size (BHK):** Number of bedrooms, hall, and kitchen.
* **Total Sqft:** Total area of the property.
* **Bath:** Number of bathrooms.
* **Target Variable:** `Price` (in Lakhs).

## Project Workflow
1. **Data Cleaning:** Handled missing values, standardized string formats, and converted square footage ranges into numerical averages.
2. **Outlier Removal:** Applied the Interquartile Range (IQR) method mathematically to remove illogical property sizes and prices.
3. **Feature Engineering:** Grouped rare locations into an 'other' category and applied One-Hot Encoding.
4. **Data Scaling:** Standardized the features using `StandardScaler` to ensure optimal neural network convergence.
5. **Model Architecture:** Built a Sequential FCNN with three hidden layers (256, 128, 64 neurons) using ReLU activations and Dropout for regularization.

## Model Evaluation
The regression model was trained using the Adam optimizer and Mean Squared Error (MSE) loss function, alongside callbacks like `EarlyStopping` and `ReduceLROnPlateau`.
* **Mean Absolute Error (MAE):** ~15.97
* **R-squared (R2 Score):** ~0.62

## Technologies Used
* Python
* TensorFlow / Keras
* Scikit-Learn
* Pandas & NumPy
* Matplotlib

## Author
**Rana Magdy**
