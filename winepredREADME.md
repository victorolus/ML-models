# Wine Quality Prediction

This project applies machine learning techniques to predict wine quality based on physicochemical properties measured from red and white vinho verde wines from Portugal.

## Overview
- **Objective:** Predict wine quality (scored from 0 to 10) using measurable chemical properties.
- **Dataset:** 6,497 samples (1,599 red and 4,898 white wines) with 11 continuous features and one categorical feature (color).
- **Models Used:** 
  - **CART** for feature selection and interpretation.
  - **Random Forest** for ensemble-based prediction.

## Data Preparation
- **Data Cleaning:** Converted data types appropriately and removed 1,177 duplicate records to ensure data integrity.
- **Exploratory Data Analysis:** Performed correlation analysis using heatmaps to identify key predictors such as alcohol content and volatile acidity.
- **Data Splitting:** Utilized stratified sampling (60% training, 40% testing) to maintain class proportions.

## Modelling Approach
- **CART:** Constructed decision trees using the `rpart` package in R for feature selection and model interpretability. Pruned the tree to reduce overfitting.
- **Random Forest:** Built an ensemble model with 300 trees using the `randomForest` package to improve prediction accuracy and reduce variance.

## Results
- **CART Model:** Achieved an overall accuracy of ~52.5%, with difficulties in predicting minority quality classes.
- **Random Forest Model:** Outperformed the CART model with an accuracy of 65.73% and a higher Kappa score. Key predictors included alcohol, volatile acidity, and total sulfur dioxide.

## Setup & Execution
- **Requirements:** R (version X.X or higher) with the following packages:
  - `rpart`
  - `randomForest`
  - `caret`
  - `tidyverse`
- **Steps:**
  1. Clone the repository.
  2. Install the required R packages.
  3. Execute the provided R script (e.g., `wine_quality_prediction.R`) to run data cleaning, modeling, and evaluation.

## Future Work
- Address class imbalance with techniques such as SMOTE and class weighting.
- Enhance model performance through further hyperparameter tuning and exploring advanced ensemble methods.

## References
- Dataset reference: Cortez et al. (2009)
- Methodological insights: James et al. (2021) and Breiman (2001)
