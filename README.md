Employee Salary Classification Project
This project focuses on building a machine learning model to predict whether an individual's income is greater than $50K or less than or equal to $50K based on demographic and employment information.

Dataset
The project utilizes the Adult dataset, which contains various attributes about individuals, including:

Age
Workclass
Education and Educational Number
Marital Status
Occupation
Relationship
Race
Gender
Capital Gain
Capital Loss
Hours per Week
Native Country
Income (the target variable: >50K or <=50K)
Project Goals
The main goals of this project are:

To preprocess the Adult dataset to make it suitable for machine learning.
To train and evaluate several classification models to predict income level.
To select the best-performing model.
To deploy the model as a user-friendly web application for making predictions.
Project Steps
Data Loading and Initial Exploration: Load the dataset and perform initial checks for its structure, content, and missing values.
Data Cleaning and Preprocessing: Handle missing values (specifically the '?' entries), remove unnecessary columns, and address outliers in numerical features. Categorical features are encoded into numerical formats, and numerical features are scaled.
Model Selection and Training: Split the data into training and testing sets. Train various classification models including:
K-Nearest Neighbors (KNN)
Logistic Regression
Support Vector Classifier (SVC)
Random Forest Classifier
Gradient Boosting Classifier
MLP Classifier (Neural Network)
Model Evaluation: Evaluate the performance of each trained model using metrics such as accuracy and the classification report (precision, recall, F1-score).
Best Model Selection: Identify the model with the highest accuracy on the test set. The Gradient Boosting Classifier was found to be the best-performing model in this project.
Model Saving: Save the trained best model (retrained_best_model.pkl) and the scaler (scaler_retrained.pkl) to disk for later use in the web application.
Streamlit Web Application Development: Create an interactive web application (app.py) using Streamlit. This application allows users to input employee details and get a salary class prediction. It also includes functionality for batch predictions via CSV upload.
Deployment using ngrok: Use ngrok to create a public tunnel to the local Streamlit application, making it accessible from anywhere with an internet connection.
Results
The evaluation of the models showed that the Gradient Boosting Classifier achieved the highest accuracy of approximately 0.8722 on the test set.
Run the Streamlit App : https://e61718c1b6c6.ngrok-free.app
