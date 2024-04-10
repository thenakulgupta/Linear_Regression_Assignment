# Bike-Sharing Demand Prediction

> This project aims to predict the demand for shared bikes after the COVID-19 pandemic, helping BoomBikes to strategize their operations accordingly.

## Table of Contents

- [General Information](#general-information)
- [Technologies Used](#technologies-used)
- [Data Preparation](#data-preparation)
- [Model Building and Evaluation](#model-building-and-evaluation)
- [Conclusions](#conclusions)
- [Acknowledgements](#acknowledgements)

## General Information

- The objective is to model the demand for shared bikes with the given dataset, enabling BoomBikes to understand how demands vary with different features and adjust their business strategy.
- The background involves addressing the revenue dips BoomBikes faced due to the COVID-19 pandemic and preparing for the post-quarantine demand surge.
- The dataset contains daily data on bike rentals and various factors like weather conditions and holidays.

## Technologies Used

- Python - version 3.8
- pandas - version 1.2.4: For data manipulation and analysis.
- numpy - version 1.19.5: For numerical operations.
- matplotlib - version 3.3.4 and seaborn - version 0.11.1: For data visualization.
- scikit-learn - version 0.24.1: For implementing the multiple linear regression model and model evaluation.

## Data Preparation

- The 'season' and 'weathersit' variables were converted to categorical types to accurately represent their non-ordinal nature.
- A dummy variable trap was avoided by dropping the first level of each newly created dummy variable from 'season', 'weathersit', 'mnth', and 'weekday'.
- The 'yr' variable, representing years 2018 and 2019, was kept as a significant predictor for the model, acknowledging the increasing popularity of bike-sharing systems.

## Model Building and Evaluation

- A multiple linear regression model was built using significant predictors identified during the exploratory data analysis phase.
- The dataset was split into training and testing sets (80%-20%) to evaluate the model's performance.
- Model evaluation was performed using the R-squared score, which quantified how well the independent variables predict the bike demand on the test set.

## Conclusions

- The model successfully identified key factors affecting bike demand, including weather conditions, time of the year, and user type (casual or registered).
- R-squared score on the test set indicated an excellent fit, suggesting the model can accurately predict daily bike rental counts.
- Recommendations for BoomBikes include focusing marketing efforts during peak seasons and favorable weather conditions, and developing loyalty programs for registered users.

## Acknowledgements

- This project was inspired by the real-world challenges faced by the bike-sharing industry during the COVID-19 pandemic.
