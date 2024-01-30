# House Price Prediction Model

## Overview
This project implements a house price prediction model using the California housing dataset. The dataset is preprocessed, features are engineered, and two regression models (Linear Regression and Random Forest) are trained to predict the median house value.

## Prerequisites
- Python 3
- Required Python libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

## Dataset
The dataset used for this project is the California housing dataset. You can download it [here](https://www.kaggle.com/datasets/camnugent/california-housing-prices).

## Code Structure
- `house_price_prediction.ipynb`: Jupyter Notebook containing the code.
- `README.md`: Documentation file (you're reading it).

## Usage
1. Ensure the dataset is available and update the file path accordingly.
2. Run the code in a Jupyter Notebook or any Python environment.

## Steps
1. **Data Loading and Cleaning:**
   - Load the dataset.
   - Drop missing values.

2. **Exploratory Data Analysis (EDA):**
   - Split the data into training and testing sets.
   - Visualize data distribution using histograms.
   - Explore correlations between features using heatmaps.

3. **Feature Engineering:**
   - Log transform certain features for normalization.
   - One-hot encode categorical variable (`ocean_proximity`).

4. **Model Training - Linear Regression:**
   - Train a Linear Regression model.

5. **Model Training - Random Forest:**
   - Train a Random Forest Regressor model.
   - Perform hyperparameter tuning using Grid Search.

6. **Model Evaluation:**
   - Evaluate the performance of both models on the test set.

## Results
- The Linear Regression model is trained and evaluated.
- The Random Forest Regressor is trained, and hyperparameter tuning is performed.
- Model performances are compared.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
