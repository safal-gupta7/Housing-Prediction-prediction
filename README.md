# Housing Price Prediction

## Overview
A machine learning regression project that predicts housing prices using structured housing data.

## Objectives
- Explore and understand the dataset.
- Perform data cleaning and preprocessing.
- Train and evaluate regression models.
- Tune a Random Forest Regressor using GridSearchCV.
- Generate predictions for the test dataset.

## Models
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

## Model Evaluation
The models are evaluated using:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

## Best Model
The current best model is a tuned Random Forest Regressor.

Validation results:
- MAE: 2.5341
- RMSE: 4.2245
- R²: 0.8328

These metrics were measured on a held-out validation set. They are not competition test-set scores.

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn (if used)
- Scikit-learn
- Jupyter Notebook

## How to Run
1. Clone this repository.
2. Install dependencies using `pip install -r requirements.txt`.
3. Place the permitted dataset files in the expected location.
4. Open and run the Jupyter notebook.

## Disclaimer
This is an educational machine learning project. Results depend on the dataset and validation split.