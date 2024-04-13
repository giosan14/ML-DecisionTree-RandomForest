# Decision Tree and Random Forest Regression/Classification

This repository contains Python code for implementing Decision Tree Regression and Classification, as well as Random Forest Regression using scikit-learn. These algorithms are widely used in machine learning for both regression and classification tasks.

## Dependencies

- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn

## Usage

1. Clone the repository or download the code files.
2. Ensure that you have the necessary dependencies installed in your Python environment.
3. Run the Python script `decision_tree_random_forest.py`.
4. The script reads two CSV files (`housing_train.csv` and `housing_test.csv`) containing training and test data, respectively.
5. The data is preprocessed and split into features (X) and target variables (y).
6. For Decision Tree Classification:
    - A Decision Tree Classifier is trained on the training data.
    - Predictions are made on the test data, and accuracy is computed.
7. For Decision Tree Regression:
    - A Decision Tree Regressor is trained on the entire dataset.
    - Predictions are made on the entire dataset, and metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R2) are computed and printed.
8. The script then categorizes the `SalePrice` column into 'Low', 'Medium', and 'High' categories based on specified conditions.
9. Finally, a Decision Tree is visualized using the `plot_tree` function.

## Results

- Decision Tree Classifier accuracy is computed using `metrics.accuracy_score`.
- Decision Tree Regressor metrics (MAE, MSE, R2) are computed using scikit-learn's `mean_absolute_error`, `mean_squared_error`, and `r2_score`.
- The categorization of `SalePrice` into three categories is done using NumPy's `np.select` function.
- Decision Tree visualization is achieved using matplotlib's `plot_tree` function.

## Additional Analysis

- A Random Forest Regressor is trained and used to predict housing prices.
- R-squared (R2) is computed for the Random Forest model.
- A Light Gradient Boosting Regressor (`DecisionTreeRegressor`) is trained and used to predict housing prices, and the Mean Squared Error (MSE) is computed.
