# Flight-Database_EDA_project
This project aims to predict flight prices using a dataset containing various features related to flights.

## Dataset

The dataset used in this project is `flight_price.xlsx`. It contains the following features:

- **Airline:** The name of the airline company.
- **Flight:** The plane's flight code.
- **Source City:** The city from which the flight takes off.
- **Departure Time:** The time of departure (categorized into time periods).
- **Stops:** The number of stops between the source and destination cities.
- **Arrival Time:** The time of arrival (categorized into time periods).
- **Destination City:** The city where the flight will land.
- **Class:** The seat class (Business or Economy).
- **Duration:** The total time taken to travel between cities (in hours).
- **Days Left:** The number of days left until the trip date.
- **Price:** The target variable, representing the ticket price.

## Project Steps

The project involves the following steps:

1. **Data Loading and Initial Exploration:** The dataset is loaded using pandas, and initial exploration is performed to understand the data structure, summary statistics, and data types.
2. **Data Cleaning and Preprocessing:**
    - Handling missing values (if any).
    - Converting date and time features into numerical format.
    - Extracting relevant information from date and time features (e.g., day, month, hour, minute).
    - Dropping irrelevant columns.
    - Mapping categorical features like 'Total_Stops' to numerical values.
3. **Feature Engineering:** Creating new features from existing ones to potentially improve the model's performance. In this project, date and time components were extracted as new features.
4. **Exploratory Data Analysis (EDA):** Visualizing the distribution of the target variable (Price) and exploring relationships between different features.
5. **Model Building:** Selecting and training a suitable machine learning model for price prediction. (This step is not fully implemented in the provided code but would be the next logical step).
6. **Model Evaluation:** Evaluating the trained model's performance using appropriate metrics. (This step is not fully implemented in the provided code).
7. **Prediction:** Using the trained model to predict flight prices on new data. (This step is not fully implemented in the provided code).

## Code Overview

The provided code snippet demonstrates the initial steps of the project, including data loading, exploration, and some data preprocessing and feature engineering.

- **Loading Data:** The dataset is loaded using `pd.read_excel()`.
- **Basic Exploration:** `df.head()`, `df.info()`, and `df.describe()` are used to get a glimpse of the data.
- **Answering Basic Questions:** The code includes examples of how to answer simple questions about the data, such as the average price, unique airlines, and the airline with the most flights.
- **Visualizing Price Distribution:** A histogram is plotted to visualize the distribution of flight prices.
- **Feature Engineering:**
    - 'Date_of_Journey' is split into 'Date', 'Month', and 'Year'.
    - 'Arrival_Time' is processed to extract 'Arrival_hour' and 'Arrival_min'.
    - 'Dep_Time' is processed to extract 'Departure_hour' and 'Departure_min'.
- **Data Type Conversion:** Extracted date and time components are converted to integer types.
- **Dropping Columns:** Irrelevant columns like 'Date_of_Journey', 'Arrival_Time', 'Dep_Time', and 'Route' are dropped.
- **Mapping 'Total_Stops':** The categorical 'Total_Stops' feature is mapped to numerical values.

## How to Run the Code

1. Ensure you have the `flight_price.xlsx` file in the same directory as your notebook or provide the correct path.
2. Run the code cells sequentially in a Jupyter Notebook or Google Colab environment.
3. You will need to install the necessary libraries: pandas, matplotlib, and numpy. You can install them using pip:
Use code with caution
bash pip install pandas matplotlib numpy openpyxl

library_add

content_copy
## Future Work

- Implement the model building, evaluation, and prediction steps.
- Explore different machine learning algorithms for price prediction.
- Perform more in-depth EDA to uncover further insights.
- Handle outliers and other data inconsistencies.
- Fine-tune model hyperparameters for better performance.
- Create a user interface for predicting flight prices.
