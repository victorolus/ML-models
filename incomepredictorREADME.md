# Income Predictor

This Python script aims to predict income levels based on demographic and socio-economic factors. It utilizes the Random Forest Classifier for predictive modeling.

## Setup

Ensure you have Python installed, along with the necessary libraries specified in the script, mainly pandas, seaborn, matplotlib, and scikit-learn.

## Usage

1. Clone the repository or download the script.
2. Install the required Python libraries if not already installed.
3. Run the script in your Python environment.

## Data Preparation

The script loads data from a CSV file (`income.csv`) and performs several preprocessing steps:

- One-hot encoding categorical variables like `occupation`, `workclass`, `marital-status`, `relationship`, `race`, and `native-country`.
- Encoding binary variables `gender` and `income`.
- Dropping the `fnlwgt` feature.
- Splitting the dataset into training and testing sets.

## Modeling

The script utilizes a Random Forest Classifier for prediction. It employs GridSearchCV for hyperparameter tuning to optimize the model's performance.

## Results

The script provides insights into feature importances, helping to identify which variables contribute most to predicting income levels.

## Link

https://www.kaggle.com/datasets/wenruliu/adult-income-dataset
