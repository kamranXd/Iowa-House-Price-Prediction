# Iowa House Price Prediction

This project builds an end-to-end machine learning pipeline to predict house prices in Iowa using features like lot size, year built, and the number of rooms. This was completed as part of the Kaggle "Intro to Machine Learning" course.

## Project Structure
├── data/
│   ├── train.csv
│   └── test.csv
├── notebooks/
│   └── iowa_house_prices.ipynb
├── README.md
└── requirements.txt

## Project Overview
- **Data Source:** Kaggle Housing Prices Competition for Kaggle Learn Users
- **Target Variable:** `SalePrice` (The price of the house)
- **Objective:** Minimize the Mean Absolute Error (MAE) on validation data.

## Steps Completed
1. **Data Exploration & Cleaning:** Handled features and target variables using Pandas.
2. **Data Splitting:** Divided the data into training and validation sets using `train_test_split` to prevent overfitting.
3. **Model Selection & Tuning:** - Tested a `DecisionTreeRegressor` across multiple `max_leaf_nodes` sizes to find the optimal tree depth.
   - Upgraded to a `RandomForestRegressor` to improve accuracy by averaging multiple decision trees.
4. **Final Model Training:** Retrained the optimized Random Forest model on the complete dataset (training + validation) to maximize performance.
5. **Submission:** Generated predictions on the hidden test set and submitted to the Kaggle leaderboard.

## Tech Stack
- Python
- Pandas
- Scikit-Learn
- NumPy
