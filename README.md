# Perfume Price Predictor

This project predicts perfume prices based on features like brand, type, available stock, sold quantity, and item location. It uses supervised machine learning regression models to identify patterns in the data and estimate prices.

## Dataset

The dataset includes the following columns:
- `brand`
- `type`
- `available`
- `sold`
- `itemLocation`
- `price` (target)

## Preprocessing & Feature Engineering

- Handled missing values using median (for numeric) and mode (for categorical).
- Dropped irrelevant columns such as `title`, `lastUpdated`, and `availableText`.
- Applied label encoding to categorical features.
- Created a `sold-to-stock ratio` to capture product demand.

## Models Used

- Linear Regression  
- Decision Tree Regression  
- Random Forest Regression  
- Support Vector Regression (SVR)  
- Gradient Boosting Regression

## Evaluation Metrics

- R² Score  
- Mean Absolute Error (MAE)  
- Root Mean Squared Error (RMSE)

## Results

Random Forest performed the best with the highest R² score and lowest RMSE. Gradient Boosting also showed strong performance. Linear Regression and SVR underperformed due to the non-linear nature of the data.

## How to Use

Run `perfume.ipynb` to view the complete workflow including preprocessing, training, evaluation, and visualization. Make sure the dataset file is in the same directory.

