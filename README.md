# Automobile (Car) Price Prediction Using Linear Regression

## Project Overview

This project explores the relationship between vehicle weight and vehicle price using a dataset of vehicle specs.
The goal of this project was to determine is curb weight can be used to predict vehicle price using a regression model.

The workflow looked like this:

-cleaning the dataset
-performing EDA
-building a regression model
-evaluating model performance

## Dataset

The car dataset contained a variety of cars and their specifications including:

-make/model/manufacturer
-turbocharged vs naturally aspirated
-two door/four door
-amount of seats (coupe vs sedan)
-engine size/displacement
-fuel system
-amount of cylinders

The dataset included 205 vehicles with 26 variables for each.

## Project Workflow

The project was organized into 3 notebooks:

### 1. Data Cleaning (clean.ipynb)
-handled missing values
-assigned column names
-exported a cleaned dataset

### 2. Exploratory Data Analysis (explore.ipynb)
-visualized relationships between variables
-identified curb weight as a strong predictor of price

### 3. Modeling (model.ipynb)
-built a linear regression model
-split the data into training and testing sets
evaluated performance using R2, MSE, RMSE

## Model 

A simple linear regression model was used to predict automobile price based on curb weight.
The data was split into training and testing sets to evaluate the models ability to handle unseen data.

## Results

The regression model showed a positive relationship between curb weight and car price.

Key metrics:
-R2 ≈ 0.70
-RMSE ≈ $4,900

These metrics indicate curb weight alone explains roughly 70% of the variation in car price in this dataset.
The relationship is strong however, other variables like engine size, horsepower, and manufacturer may also influence car price.

## Limitations and Future Work

This model uses only one predictor variable (curb weight). It performs reasonably however, additional predictor variables could improve prediction accuracy. The hypothesis "heavier cars cost more" is not always true. Sports cars are traditionally low weight but high horsepower and with larger engines. Because of this sports cars tend to be more expensive in spite of not being heavy.

## Repository Layout

data/
    clean/
        cleaned automobile dataset
    raw/
        raw automobile dataset

notebooks/
    clean.ipynb
    explore.ipynb
    model.ipynb

README.md