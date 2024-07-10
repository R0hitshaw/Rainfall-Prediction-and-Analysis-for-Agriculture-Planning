Rainfall Prediction and Agricultural Planning
Project Overview

This project aims to predict monthly rainfall using Long Short-Term Memory (LSTM) neural networks and provide agricultural planning recommendations based on the predictions. The focus is on the state of Sikkim, India, considering its unique geographical and climatic characteristics.
Table of Contents

    Introduction
    Dataset
    Data Preprocessing
    Model
    Evaluation
    Agricultural Planning
    Results
    Installation
    Usage
    Contributing
    License

Introduction

Accurate rainfall prediction is crucial for effective agricultural planning, especially in regions with diverse climatic conditions like Sikkim. This project leverages LSTM neural networks to predict monthly rainfall and provides actionable recommendations for farmers and stakeholders based on these predictions.
Dataset

The dataset used in this project contains monthly rainfall data for various districts in Sikkim over several years. It includes the following columns:

    Year: Year of the record
    Month: Month of the record
    District: District name
    Rainfall: Monthly rainfall value in millimeters

Data Preprocessing

Data preprocessing steps include:

    Handling Missing Values: Imputing or removing missing values.
    Categorical Encoding: Converting categorical variables (e.g., Month, District) into numerical representations.
    Scaling: Normalizing the rainfall values using MinMaxScaler.
    Reshaping for LSTM: Reshaping the data to fit the input requirements of LSTM models.

Model

The model architecture includes:

    Two LSTM layers with 50 units each and ReLU activation.
    A Dense output layer with one unit to predict the rainfall.
    The model is compiled with Adam optimizer and Mean Squared Error (MSE) loss function.

Model Training

The model is trained on the preprocessed dataset with the following parameters:

    Epochs: 100
    Batch Size: 32
    Validation Split: 20% of the data

Evaluation

The model performance is evaluated using the following metrics:

    Mean Absolute Error (MAE)
    Root Mean Squared Error (RMSE)
    R-Squared (R²)

Agricultural Planning

Based on the rainfall predictions, the project provides recommendations for agricultural planning:

    Low Rainfall (< 50 mm): Consider drought-resistant crops.
    Moderate Rainfall (50 - 100 mm): Regular irrigation schedule advised.
    High Rainfall (> 100 mm): Prepare for potential flooding, manage drainage systems.

Results

The model achieved the following performance metrics:

    R-Squared (R²): 0.81
    Mean Absolute Error (MAE): 0.07
    Root Mean Squared Error (RMSE): 0.10

Installation

To run this project, clone the repository and install the required dependencies:

bash

git clone https://github.com/your-username/rainfall-prediction-agriculture-planning.git
cd rainfall-prediction-agriculture-planning
pip install -r requirements.txt

Usage

    Preprocess the Data: Prepare the dataset by running the preprocessing script.
    Train the Model: Train the LSTM model using the training script.
    Make Predictions: Use the trained model to make rainfall predictions.
    Get Recommendations: Obtain agricultural planning recommendations based on the predictions.
