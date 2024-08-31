[![Codacy Badge](https://app.codacy.com/project/badge/Grade/32301d7281ec464d8023edf6cedd0add)](https://app.codacy.com/gh/Abhinav330/Customer-behavior-Analysis-Linear-Regression/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Abhinav330/Customer-behavior-Analysis-Linear-Regression/matplotlib?color=green)
![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Abhinav330/Customer-behavior-Analysis-Linear-Regression/numpy?color=silver)
![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Abhinav330/Customer-behavior-Analysis-Linear-Regression/pandas?color=red)
![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Abhinav330/Customer-behavior-Analysis-Linear-Regression/scikit-learn?color=red)
![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Abhinav330/Customer-behavior-Analysis-Linear-Regression/scipy?color=yellow)
![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Abhinav330/Customer-behavior-Analysis-Linear-Regression/seaborn?color=beige)
![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/Abhinav330/Customer-behavior-Analysis-Linear-Regression?color=dark%20green)
![GitHub repo size](https://img.shields.io/github/repo-size/Abhinav330/Customer-behavior-Analysis-Linear-Regression)

# Customer-behavior-Analysis-Linear-Regression

# Code Summary

This repository explores customer behavior data for an NYC clothing company with both a mobile app and website. They want to understand which platform drives higher sales.

## Data Exploration and Visualization

The code starts by importing necessary libraries, loading the 'Ecommerce Customers' dataset using pandas, and performing data exploration and visualization tasks:

- Displays the first few rows of the dataset using `customers.head()`.
- Provides summary statistics using `customers.describe()`.
- Shows dataset information using `customers.info()`.
- Creates various plots and visualizations:
  - Joint plots to explore relationships between 'Time on Website/App' and 'Yearly Amount Spent'.
  - A pair plot to visualize pairwise relationships between numerical features.
  - A linear regression plot (`lmplot`) to visualize the relationship between 'Yearly Amount Spent' and 'Length of Membership'.

## Data Preprocessing

The code preprocesses the data by selecting specific columns for feature variables ('X') and the target variable ('Y'). It then splits the dataset into training and testing sets using `train_test_split()`.

## Linear Regression Modeling

The script proceeds to build a Linear Regression model to predict 'Yearly Amount Spent' based on the selected features ('Avg. Session Length', 'Time on App', 'Time on Website', 'Length of Membership'):

- Imports `LinearRegression` from scikit-learn.
- Initializes and fits a Linear Regression model to the training data.
- Calculates the coefficients of the model using `lm.coef_`.
- Makes predictions on the testing data using `lm.predict()`.
- Visualizes the predictions against actual values using a scatter plot.

## Model Evaluation

The code evaluates the Linear Regression model's performance by calculating and printing various regression metrics:

- Mean Absolute Error (MAE).
- Mean Squared Error (MSE).
- Root Mean Squared Error (RMSE).
- Additionally, it visualizes the distribution of residuals (the difference between actual and predicted values) using a histogram (`sns.distplot`).

## Coefficients

The script creates a DataFrame (`coof`) to display the coefficients of the Linear Regression model along with their corresponding feature names.

