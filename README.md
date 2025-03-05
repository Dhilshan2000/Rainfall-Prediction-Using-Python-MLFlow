# Rainfall Prediction Web App

This repository contains a web application that predicts whether there will be rainfall based on weather-related features. The app uses a machine learning model to make the prediction based on the following features:

1. Pressure
2. Dewpoint
3. Humidity
4. Cloud
5. Sunshine
6. Wind Direction
7. Wind Speed

## Files in the Repository

1. app.py
   
This is the main Python file that runs the Flask web application. It performs the following functions:

Initializes the Flask App: It sets up the basic web framework and routes.
Loads the Model: It connects to MLflow to load the production version of the rainfall prediction model.
Handles Predictions: It captures input data from the user, formats it into a DataFrame, and uses the model to predict whether there will be rainfall.
Prediction Result Display: It shows the result ("Rainfall" or "No Rainfall") to the user on the web page.

2. Rainfall_Prediction.ipynb
   
This Jupyter notebook contains the code and logic to train the machine learning model that predicts rainfall. It involves:

Data Exploration: Analyzing the provided dataset.
Model Training: Using machine learning algorithms to build a model that can predict rainfall based on the provided features.
Model Evaluation: Evaluating the model's performance and saving the trained model for later use.

3. Rainfall.csv
   
This CSV file contains the dataset used for training the machine learning model. The dataset includes multiple weather features like pressure, humidity, and wind speed, along with the target variable (whether there was rainfall).

5. index.html
   
This is the HTML file that provides the frontend interface for the user. The web page allows the user to input the following weather features:

Pressure
Dewpoint
Humidity
Cloud
Sunshine
Wind Direction
Wind Speed
Once the user submits the form, the app sends the data to the backend, which processes it and returns the prediction.

How to Run

01. Ensure that the machine learning model is correctly saved and loaded using MLflow. The model should be available at models:/rainfall-prediction-production@champion.

02. Run the app.py file to start the web server: "python app.py"

03. Open a browser and navigate to http://127.0.0.1:8080/ to access the web application.

04. Enter the weather features in the form and click Predict to get the prediction result.

![Screenshot 2025-03-05 222339](https://github.com/user-attachments/assets/2a0562a3-62a9-4014-b039-635f3dbde17a)

![Screenshot 2025-03-05 222323](https://github.com/user-attachments/assets/e120ca18-34e3-4414-b55e-cb382a13340f)

![Screenshot 2025-03-05 221306](https://github.com/user-attachments/assets/5895e99a-383c-458d-a0a4-fafc2f439101)

![Screenshot 2025-03-05 221242](https://github.com/user-attachments/assets/ad8a6487-e10e-4fb2-b963-552c8fb5cda3)

![Screenshot 2025-03-05 221222](https://github.com/user-attachments/assets/1bf37362-11d3-4eb6-8b36-8a905f9540ee)

![Screenshot 2025-03-05 221155](https://github.com/user-attachments/assets/e7d2dfd5-1436-4567-85be-1c6f3a5cb6f1)



