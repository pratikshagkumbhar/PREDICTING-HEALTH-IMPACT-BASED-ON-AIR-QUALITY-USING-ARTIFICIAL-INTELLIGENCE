# PREDICTING-HEALTH-IMPACT-BASED-ON-AIR-QUALITY-USING-ARTIFICIAL-INTELLIGENCE
This project uses AI and machine learning to predict health impacts based on air quality data. It combines pollutant levels, weather conditions, and health factors to classify risk levels. Models like XGBoost and Random Forest improve accuracy, enabling early detection and better environmental health analysis.

📌 Overview

This project proposes an AI-based machine learning framework to classify health impact classes (0–3) based on air pollution severity.
The model integrates air pollutants, weather factors, and health-related data to capture real-world impact on human health.
Unlike existing approaches that focus mainly on AQI classification, this work directly predicts health impact levels.

📊 Dataset
https://www.kaggle.com/datasets/rabieelkharoua/air-quality-and-health-impact-dataset

⚙️ Methodology

🔹 Data Preprocessing
-Binning: Converted AQI, temperature, and humidity into categorical levels

-One-Hot Encoding: Converted categorical data into numerical format

-SMOTE: Used to balance minority classes

-Standard Scaling: Applied for better model performance


🔹 Feature Engineering

New features were created to capture combined effects:

-PM2.5 × Temperature → captures effect of heat on pollutant activity

-PM2.5 × Humidity → shows particle suspension in air

-AQI / (Wind Speed + 1) → inverse relation with wind speed

-PM2.5 / (PM10 + 1) → fine particle ratio for respiratory risk

-Total Pollution → sum of all pollutants

-Total Health Cases (R + C) → combined health impact

-Admission Rate → severity indicator


🤖 Machine Learning Models

The following models were implemented with hyperparameter tuning and 5-fold GridSearchCV:

-K-Nearest Neighbors (KNN)

-Decision Tree

-Random Forest

-XGBoost

-AdaBoost


📈 Results

<img width="650" height="123" alt="image" src="https://github.com/user-attachments/assets/1d9e68ce-73bc-44de-b97e-a929d5d4b0aa" />

