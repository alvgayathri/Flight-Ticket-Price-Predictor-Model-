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

Run the Jupyter Notebook
Open the Jupyter notebook Flight_Ticket_Price_Predictor.ipynb and run the cells to preprocess the data, train the models, and evaluate the results.

Predict Flight Prices
Use the trained model to predict flight prices by providing the necessary input features.

Dataset Files
The dataset used in this project is stored in the data directory:

Data_Train.xlsx: The main dataset containing flight information.
Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
The dataset used in this project is sourced from Kaggle.

Special thanks to the open-source community for providing valuable resources and libraries.
