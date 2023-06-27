# House_Price_Prediction

# House Price Prediction using Linear Regression

This repository contains code for predicting house prices based on land area using linear regression. The dataset used for training and testing the model is provided in the 'House Price India.csv' file.

## Libraries Used
- Pandas: A library for data manipulation and analysis.
- sklearn.linear_model: A module from the scikit-learn library that provides various linear regression models.
- matplotlib.pyplot: A plotting library used for data visualization.

## Dataset
The dataset is loaded using the Pandas library's `read_csv()` function and stored in the `dataset` variable. Information about the dataset is displayed using the `shape` and `head()` functions.

## Data Visualization
The dataset is visualized by creating a scatter plot using the `scatter()` function from matplotlib. The x-axis represents the land area, and the y-axis represents the house price.

## Data Segregation
The dataset is segregated into input features (`X`) and output (`Y`) variables. The `X` variable contains all columns except for the 'Price' column, while the `Y` variable contains the 'Price' column.

## Model Training
A linear regression model is created using the `LinearRegression()` class from scikit-learn. The `fit()` function is used to train the model on the input (`X`) and output (`Y`) variables.

## Price Prediction
The code allows the user to input a land area value (`x`) for which they want to predict the house price. The model's `predict()` function is used to generate the predicted price for the given land area. The result is stored in the `PredictedmodelResult` variable and printed.

## Model Evaluation
To validate the model's accuracy, the coefficient (`m`) and intercept (`b`) values of the linear regression equation are calculated using the `coef_` and `intercept_` attributes of the trained model, respectively. The equation is then used to calculate the predicted price (`y`) based on the given land area (`x`). The result is printed as "The Price of {x} Square feet Land is: {y}".

This code can be further enhanced by incorporating techniques such as data preprocessing, feature scaling, cross-validation, and evaluating performance metrics to ensure accurate house price predictions.
