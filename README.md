# car_pricing_model
car pricing model

# Used Car Price Prediction

## Overview

This project aims to explore a dataset of used cars and develop a predictive model to determine what factors influence the price of a car. The analysis is geared towards helping used car dealerships understand what features drive higher or lower prices, ultimately enabling them to fine-tune their inventory to maximize profitability.

## Dataset

The dataset contains information on approximately 426,000 used cars, which is a subset of a larger dataset from Kaggle. Each car is described by various features, including:
- **Cylinders**
- **Odometer**
- **Manufacturer**
- **Drive type**
- **Fuel type**
- **Vehicle type**
- And more...

## Business Understanding

The main goal from a business perspective is to identify key drivers of used car prices. The task can be reframed as a data science problem where we build a predictive model that estimates car prices based on vehicle characteristics such as age, manufacturer, and condition. By providing insights into what consumers value, used car dealerships can better understand the market and optimize their inventory.

## Methodology

### CRISP-DM Framework

The project follows the CRISP-DM (Cross Industry Standard Process for Data Mining) methodology, which includes:
1. **Business Understanding**: Identifying the business goal of understanding factors driving car prices.
2. **Data Understanding**: Cleaning and preparing the data for modeling.
3. **Modeling**: Using various regression techniques to model the relationship between car features and price.
4. **Evaluation**: Evaluating model performance to ensure accuracy and reliability.

### Tools and Libraries

The following tools and libraries were used in the analysis:
- **Pandas** for data manipulation
- **NumPy** for numerical operations
- **Matplotlib** and **Seaborn** for data visualization
- **Scikit-learn** for machine learning models and feature selection
- **Statsmodels** for statistical analysis and time series modeling
- **GridSearchCV** for hyperparameter tuning
- **ARIMA** and **SARIMAX** for potential time series forecasting
- **Linear Regression, Ridge, Lasso, ElasticNet** for model building

### Feature Selection and Modeling

The project explores various regression models:
- **Linear Regression**: A basic model used to establish a baseline.
- **Ridge Regression**: Used to penalize large coefficients and avoid overfitting.
- **Lasso Regression**: Adds L1 regularization for feature selection by eliminating some features.
- **ElasticNet Regression**: Combines Lasso and Ridge to handle multiple correlated features.

## Model Performance

After evaluating the models, the following key performance metrics were considered:
- **Mean Squared Error (MSE)**: Measures the average squared difference between predicted and actual prices.
- **R-squared (R²)**: Indicates the proportion of variance in car prices explained by the model.

| Model                  | MSE         | R-squared |
|------------------------|-------------|-----------|
| Linear Regression       | 31,038,500  | 0.6977    |
| Ridge Regression        | 31,022,262  | 0.6978    |
| Lasso Regression        | 39,148,061  | 0.6187    |
| ElasticNet Regression   | 39,743,127  | 0.6129    |

### Recommendations for Car Dealerships

Based on the analysis:
- **High-Priced Cars**: Focus on vehicles with more cylinders, trucks, pickups, and luxury brands like **Toyota**, **Lexus**, and **Mercedes-Benz**. These vehicles tend to retain higher value.
- **Low-Priced Cars**: Avoid older vehicles with high mileage. Gasoline and hybrid vehicles, as well as sedans and hatchbacks, tend to fetch lower prices unless they have standout features.

## How to Run the Project

Clone the repository: 
git clone https://github.com/mcron10/car-price-prediction.git
cd PAA_5-1

make sure the data directory and csv files is present
## Future Work

- **Time Series Analysis**: Investigate how car prices change over time, possibly incorporating seasonal trends.
- **Further Feature Engineering**: Create additional features such as depreciation rate or owner history to improve model accuracy.
- **Advanced Modeling**: Experiment with more complex models like Gradient Boosting or Random Forest to potentially improve prediction accuracy.

## Conclusion

This project provides valuable insights into the factors that drive used car prices. By understanding these key variables, dealerships can better curate their inventory, focus on high-value vehicles, and ultimately increase profitability.
