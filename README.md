# Flight Ticket Price Predictor Model

## Overview
This project aims to predict flight ticket prices using machine learning techniques.

## Dataset
The dataset contains the following columns:
- **Airline**: The name of the airline.
- **Date_of_Journey**: The date of the flight.
- **Source**: The departure city.

## Data Preprocessing
1. **Handling Missing Values**: Any rows with missing values are dropped.
2. **Feature Engineering**:
   - Duration is converted to total minutes.
   - Date of journey is converted to a datetime object.

## Model Building
Several machine learning models are trained and evaluated, including:
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor

## Results
The best-performing model is selected based on evaluation metrics.
