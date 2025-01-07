# COVID-19 Prediction and Analysis
# Repository: COVID-19 Prediction Analysis
# Overview
This repository contains a Jupyter Notebook that explores and analyzes COVID-19 data using machine learning techniques. The main goal of this project is to predict the number of new COVID-19 cases across various states in the US, leveraging time-series data and feature engineering. The project uses the covid19_open_data public dataset available in Google BigQuery, enriched with population and other relevant features for normalization and model training.

# Key Features
**Data Preparation and Cleaning**
Handling missing values in critical columns such as new_persons_fully_vaccinated and population.
Dropping columns with high percentages of null values, like vaccination-related fields, and filling remaining missing values with appropriate defaults.

**Feature Engineering**
Creating lag variables (e.g., 10-14 day lags) to capture COVID-19’s cyclical nature.
Generating rolling averages and sums to highlight trends over time.
Normalizing data by population to enable cross-state comparisons.

**Exploratory Data Analysis (EDA)**
Identifying trends and patterns in the data using visualizations.
Examining the correlation between COVID-19 spread and population density.

**Predictive Modeling**
Implementing a Random Forest Regressor to predict new COVID-19 cases.
Evaluating the model with metrics like Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared (R²).
Analyzing feature importance to identify key drivers of COVID-19 spread.

**Visualization**
Creating intuitive plots for feature importance and other key insights to communicate findings effectively.

**Tools and Technologies**
Python: Core programming language for data processing and model development.
Pandas: For data manipulation and cleaning.
Matplotlib/Seaborn: For data visualization.
Scikit-learn: For machine learning and model evaluation.
Google BigQuery: To access and query the public COVID-19 dataset.

**Objectives**
Predict the number of new COVID-19 cases by state for the final quarter of the year.
Understand factors influencing the spread of the virus to help inform policy and public health decisions.
Practice feature engineering and predictive modeling in a real-world data scenario.
