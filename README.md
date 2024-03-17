# Solar Irradiance Prediction

This project focuses on predicting solar irradiance using meteorological data collected at the HI-SEAS weather station over a four-month period from September to December 2016. Solar irradiance is a critical parameter for various applications, including solar energy generation, climate modeling, and atmospheric science.

![Python](https://img.shields.io/badge/made%20with-Python-blue.svg) ![Machine Learning](https://img.shields.io/badge/-Machine%20Learning-orange) ![Data Science](https://img.shields.io/badge/-Data%20Science-lightgrey) ![Prediction](https://img.shields.io/badge/-Prediction-brightgreen)

## Overview

The goal of this project is to predict solar radiation (measured in watts per square meter) based on environmental factors such as temperature, humidity, barometric pressure, wind direction, and wind speed. By leveraging machine learning techniques, this project aims to provide accurate forecasts of solar irradiance, which is beneficial for optimizing solar energy production and understanding atmospheric conditions.

## Dataset

The dataset consists of meteorological observations collected at the HI-SEAS weather station during the interval between Mission IV and Mission V. It includes:

- Sequential row number for dataset ordering
- UNIX time_t value for alignment with other datasets
- Date and local time (24-hour format)
- Measurements of solar radiation, temperature, humidity, barometric pressure, wind direction, and wind speed
- Sunrise and sunset times in Hawaii local time

## Data Preprocessing

The dataset underwent several preprocessing steps, including:
- Parsing dates and times to extract meaningful features such as month, day, hour, minute, and second
- Handling missing values (if any)
- Transforming categorical data and normalizing numerical features for optimal machine learning model performance

## Feature Engineering

We performed feature engineering to improve model accuracy, which included:
- Extracting time components from sunrise and sunset times
- Applying transformations like Box-Cox, Log, Min-Max, and Standard scaling to various features

## Machine Learning Model

The project employs several machine learning models, including:
- **XGBoost Regression Model**: Predicts solar irradiance as a continuous variable
- **MultiLayer Perceptron (Neural Network)**: A deep learning approach to predict solar irradiance

Model performance was evaluated using metrics such as Root Mean Squared Error (RMSE) and R-squared (R2).

## Usage

To replicate or explore this project:

1. Clone the repository: git clone https://github.com/your-username/solar-irradiance-prediction.git
2. Navigate to the project directory
3. Install required libraries (preferably in a virtual environment)
4. Run the Jupyter notebooks to explore data analysis and model training steps
