**COVID-19 Prediction Project

Objective**

The goal of this project is to predict daily confirmed COVID-19 cases in the United States using machine learning techniques. The focus was on feature engineering and model optimization to improve predictive accuracy.

**Dataset**

The dataset used contain COVID-19 case data, including engineered features:

new_confirmed: Daily new confirmed cases.

new_deceased: Daily new deaths.

Lag features (new_confirmed_lag_10, new_deceased_lag_10, etc.) for temporal patterns.

Rolling averages and sums (e.g., new_confirmed_10_14_avg).

Population-normalized metrics (e.g., new_confirmed_per_100k).

Vaccination data (percent_fully_vaccinated).

**Steps Taken

Data Preprocessing**

Handled missing values.

Created lag features to capture temporal trends.

Added rolling averages and sums for smoothing.

Normalized metrics using population data.

**Feature Selection**

Applied Recursive Feature Elimination (RFE) to identify the most important features for prediction.

Selected features: new_deceased, new_deceased_10_14_avg, new_deceased_10_14_sum, new_confirmed_per_100k, and new_deceased_per_100k.

**Model Training**

Used a Random Forest Regressor for prediction.

Optimized the model using selected features.

**Model Evaluation**

Mean Absolute Error (MAE): 27.22

Root Mean Squared Error (RMSE): 318.68

R-squared (R²): 0.86

**Visualization**

Plotted Actual vs. Predicted values to assess model performance.

Created scatter plots and trend lines for better interpretability.

**Results**

The optimized Random Forest model demonstrated significant improvement in predictive accuracy, with an R² score of 0.86, explaining 86% of the variance in the target variable.

**Files in the Repository**

**notebooks/:**

Jupyter Notebook containing data exploration, preprocessing, model training, and evaluation.

**results/:**

Visualizations (e.g., Actual vs. Predicted plots).

**models/:**

Serialized Random Forest model (random_forest_model.pkl).

**README.md:**

Project overview.

requirements.txt:

Python libraries required to run the project.

Run the notebook
Open the Jupyter Notebook in the notebooks/ folder and run the cells.

Future Work

Incorporate external data (e.g., mobility data, government policies).

Explore time-series models (e.g., ARIMA, Prophet) for comparison.

Deploy the model as a web application using Flask or Streamlit.

License

This project is licensed under the MIT License. See the LICENSE file for details.


