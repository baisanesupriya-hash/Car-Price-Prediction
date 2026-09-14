# Car Price Prediction Using Machine Learning
Machine learning project to predict used car selling prices using data preprocessing, feature engineering, exploratory data analysis, and regression models.

## Project Overview

This project focuses on predicting the selling price of used cars using
machine learning techniques.

The project uses the CarDekho used-car dataset and analyzes factors such
as car age, kilometres driven, fuel type, seller type, transmission,
ownership, and brand.

## Objective

The objective of this project is to build a machine learning regression
model that can predict the selling price of used cars based on features
such as car brand, car age, kilometres driven, fuel type, seller type,
transmission, ownership, and usage intensity.

## Dataset

The dataset used in this project is the **CarDekho Used Car Dataset**.

The dataset contains information about used cars, including:

- Car name
- Manufacturing year
- Selling price
- Kilometres driven
- Fuel type
- Seller type
- Transmission
- Number of previous owners

## Project Workflow

1. Data Collection
2. Data Understanding
3. Data Cleaning
4. Feature Engineering
5. Exploratory Data Analysis
6. Feature Encoding
7. Train-Test Split
8. Model Training
9. Model Evaluation
10. Model Comparison
11. Feature Importance Analysis
12. Final Prediction Analysis

## Data Preprocessing

The following preprocessing steps were performed:

- Checked the dataset shape and data types
- Checked for missing values
- Removed duplicate records
- Standardized categorical values
- Created `car_age` from the manufacturing year
- Extracted the car brand
- Created `km_per_year` as an additional feature
- Handled categorical variables using One-Hot Encoding

## Exploratory Data Analysis

The project includes the following visualizations:

- Selling price distribution
- Selling price by fuel type
- Selling price vs car age
- Selling price vs kilometres driven
- Correlation heatmap

These visualizations were used to understand the relationships between
vehicle characteristics and selling prices.

## Machine Learning Models

Three regression models were trained and compared:

1. Linear Regression
2. Random Forest Regressor
3. Gradient Boosting Regressor

## Evaluation Metrics

The models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

For MAE and RMSE, lower values indicate better performance.

For R², a higher value indicates better performance.

## Model Performance

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | ₹135,884 | ₹217,456 | 0.609 |
| Random Forest Regressor | ₹124,208 | ₹197,599 | 0.678 |
| Gradient Boosting Regressor | ₹115,262 | ₹179,366 | 0.734 |

## Best Performing Model

The **Gradient Boosting Regressor** achieved the best performance among
the tested models.

### Final Performance

- **MAE:** ₹115,261.93
- **RMSE:** ₹179,366.12
- **R² Score:** 0.7343

The model achieved the highest R² score and the lowest MAE and RMSE among
the three tested models.

## Feature Importance

Feature importance analysis was performed using the Gradient Boosting
model to understand which features contributed most to the predictions.

The analysis showed that **car age** was the most influential feature
among the features used by the model.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Files

- `Car_Price_Prediction.ipynb` - Complete Jupyter Notebook containing
  data analysis, visualizations, preprocessing, model training, and
  evaluation.
- `CAR DETAILS FROM CAR DEKHO.csv` - Dataset used for the project.
- `README.md` - Project documentation.

## Conclusion

This project demonstrates how data preprocessing, feature engineering,
exploratory data analysis, and machine learning can be used to predict
the resale prices of used cars.

Among the tested models, Gradient Boosting Regressor provided the best
overall performance with an R² score of 0.7343.

The project also demonstrates how feature importance can be used to
understand the factors contributing to machine learning predictions.
