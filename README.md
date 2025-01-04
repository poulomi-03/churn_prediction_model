# Churn Prediction Model
# Prepared By: Poulomi Bhattacharya

## Overview

This project aims to predict which users are most likely to churn (i.e., stop returning or purchasing) based on their interaction with the platform. We utilize a variety of data science techniques, including feature engineering, model training, and interpretation using SHAP values. The goal is to not only predict churn but also provide actionable business insights on why users are churning and how to retain them.

## Approach

### 1. Data Exploration and Cleaning
- **Dataset Loading**: Load the CSV data into a Pandas DataFrame.
- **Missing Values**: Handle missing values appropriately (if any).
- **Feature Engineering**: Create new features such as price sums, averages, and categories based on user interactions.
- **Churn Definition**: Define churn as users who have not interacted with the platform in the last 30 days.

### 2. Data Visualization
- **Bar Plots**: Visualize the distribution of event types, top brands, and top categories.
- **Line Plot**: Show the trend of events over time.
- **Scatter Plot**: Show the relationship between price and event activity for churned vs. non-churned users.
- **Pie & Donut Charts**: Visualize the distribution of churned and non-churned users.

### 3. Model Training
- **Feature Selection**: Choose relevant features such as user interactions and price information.
- **Train-Test Split**: Split the data into training and testing sets (70-30).
- **Model**: Use XGBoost (eXtreme Gradient Boosting) to train a classification model on the data.
- **Evaluation**: Evaluate the model using classification metrics (accuracy, AUC score) and SHAP for interpretability.

### 4. Insights & Recommendations
- **Churn Insights**: Provide actionable recommendations based on the analysis of features contributing to churn.
- **Model Interpretability**: Use SHAP to explain the impact of features on model predictions.

---

## Installation

To get started with the project, follow the installation instructions below.

### Prerequisites
You’ll need the following installed on your system:
- Python 3.x
- Google Colab or Jupyter Notebook (optional, but recommended for interactive development)
  
### 1. Install Required Libraries

You can install the required libraries using `pip`. Run the following command:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost shap
