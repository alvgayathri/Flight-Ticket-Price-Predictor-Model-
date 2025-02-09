# Flight-Ticket-Price-Predictor-Model-

Overview
This project aims to predict flight ticket prices using machine learning techniques. The dataset used in this project contains various features related to flights, such as the airline, date of journey, source, destination, route, departure time, arrival time, duration, total stops, and additional information. The goal is to build a model that can accurately predict the price of a flight ticket based on these features.

Dataset
The dataset used in this project is stored in an Excel file named Data_Train.xlsx. The dataset contains the following columns:

Airline: The name of the airline.
Date_of_Journey: The date of the flight.
Source: The departure city.
Destination: The arrival city.
Route: The route taken by the flight.
Dep_Time: The departure time of the flight.
Arrival_Time: The arrival time of the flight.
Duration: The duration of the flight.
Total_Stops: The total number of stops during the flight.
Additional_Info: Additional information about the flight.
Price: The price of the flight ticket (target variable).

Data Preprocessing
The dataset undergoes several preprocessing steps to prepare it for modeling:

1. Handling Missing Values: The dataset is checked for missing values, and any rows with missing values are dropped.
2. Feature Engineering:
  -Duration: The duration of the flight is converted from a string format (e.g., "2h 50m") to total minutes.
  -Departure and Arrival Time: The departure and arrival times are converted to datetime objects, and then the hour and minute components are 
   extracted as separate features.
  -Date of Journey: The date of the journey is converted to a datetime object, and the day and month are extracted as separate features.
  -Total Stops: The total stops are mapped to numerical values (e.g., "non-stop" → 0, "1 stop" → 1, etc.).
  -Additional Info: This column is dropped as it contains mostly "No info" values.
3. Encoding Categorical Variables: Categorical variables such as Airline, Source, Destination, and Route are encoded using appropriate techniques (e.g., one-hot encoding).

Exploratory Data Analysis (EDA)
The dataset is analyzed to understand the distribution of the features and their relationship with the target variable (Price). Key insights from the EDA include:
-The distribution of flight prices.
-The relationship between the number of stops and flight prices.
-The impact of the airline on flight prices.
-The effect of the duration of the flight on the price.

Model Building
Several machine learning models are trained and evaluated to predict flight ticket prices. The models used include:

-Linear Regression
-Random Forest Regressor
-Gradient Boosting Regressor
-XGBoost Regressor
The performance of each model is evaluated using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²).

Results
The best-performing model is selected based on the evaluation metrics. The results are visualized using plots such as:

-Actual vs Predicted Prices: A scatter plot comparing the actual and predicted flight prices.
-Feature Importance: A bar plot showing the importance of each feature in the model.

Usage
To use this project, follow these steps:

Clone the Repository:
git clone https://github.com/yourusername/flight-ticket-price-predictor.git
cd flight-ticket-price-predictor

Install Dependencies:
pip install -r requirements.txt

Run the Jupyter Notebook:
Open the Jupyter notebook Flight_Ticket_Price_Predictor.ipynb and run the cells to preprocess the data, train the models, and evaluate the results.

Predict Flight Prices:
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
