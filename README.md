This README provides a professional overview of my capstone project, "Walmart Weekly Sales Prediction," completed at TSAcademy. It highlights data science workflow, including exploratory data analysis, feature engineering, and advanced machine learning modeling.

---

# Walmart Weekly Sales Prediction: Capstone Project

## Project Overview

This project was developed as a capstone project for **TSAcademy**. The primary goal is to predict the weekly sales for Walmart stores using historical sales data and environmental factors. Accurate sales forecasting is critical for optimizing inventory levels, staffing, and supply chain management in a retail environment.

## Team Members

* **Samuel Ajeboriogbon A.**
* **Jeremiah ...**

## Key Objectives

* **Data Preparation:** Clean and merge multiple datasets, including store details, weekly sales records, and exogenous variables like temperature and fuel prices.
* **Exploratory Data Analysis (EDA):** Identify seasonal trends, the impact of holidays, and correlations between sales and external factors.
* **Feature Engineering:** Enhance predictive power by creating new time-based features (month, day, year) and encoding categorical variables.
* **Predictive Modeling:** Build and evaluate robust machine learning models to forecast future sales accurately.

## Methodology & Workflow

### 1. Data Cleaning and Preprocessing

* **Handling Missing Values:** Addressed missing data in features such as `MarkDowns` by filling them with zeros.
* **Date Transformation:** Converted raw date strings into standard `datetime` formats to extract granular time features.
* **Categorical Encoding:** Applied Label Encoding and One-Hot Encoding to categorical variables like `Store Type` and `IsHoliday`.

### 2. Exploratory Data Analysis (EDA)

* **Trend Analysis:** Visualized weekly sales over time, revealing significant spikes during holiday periods such as Christmas and Thanksgiving.
* **Feature Impact:** Analyzed how variables like `Unemployment`, `CPI`, and `Temperature` correlate with consumer spending.
* **Outlier Detection:** Identified and managed anomalies in the sales data to ensure model stability.

### 3. Machine Learning Models

We implemented and compared several algorithms to determine the most effective predictor:

* **Linear Regression:** Used as a baseline model for sales estimation.
* **Decision Tree Regressor:** Captured non-linear relationships within the data.
* **Random Forest Regressor:** An ensemble approach that significantly improved accuracy and reduced variance.
* **XGBoost Regressor:** Utilized gradient boosting for optimized performance and high prediction precision.

## Key Results & Findings

* **Seasonality:** Sales are heavily influenced by the retail holiday calendar, with peak periods occurring in late Q4.
* **Model Performance:** The **Random Forest** and **XGBoost** models outperformed simpler linear models, achieving higher $R^2$ scores and lower Root Mean Squared Error (RMSE).
* **Feature Importance:** Time-based features and specific store identifiers were found to be the most influential predictors of weekly sales.

## Technical Stack

* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, PMDARIMA
* **Environment:** Jupyter Notebook

## How to Run

1. Clone this repository.
2. Install the required libraries: `pip install pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, pmdarima`.
