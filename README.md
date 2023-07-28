## Medical-Insurance-Premium-Prediction-Python-Code


This code is a comprehensive script including a systematic approach to regression analysis on the insurance.csv dataset. Created building regression models to predict insurance charges based on several features. The goal is to predict insurance charges based on independent variables.

1. Library Imports and Data Loading:
Essential libraries such as numpy, pandas, matplotlib, seaborn, and several modules from sklearn and xgboost are imported.
The dataset named 'insurance.csv' is loaded into a DataFrame dataset.

2. Data Exploration:
Initial exploration commands retrieve insights like the top records, data types, shape, and basic statistical summary of the dataset.
The dataset is grouped based on categorical features like 'sex', 'smoker', and 'region' to obtain their respective mean values.

3. Handling Missing Values:
The script checks for any missing values and their total count across the dataset.

4. Encoding Categorical Data:
Identification of categorical columns takes place.
One-hot encoding is applied to transform categorical data, especially for 'sex', 'smoker', and 'region' columns.

5. Correlation Analysis:
A bar chart representation of correlations between features and charges (target variable) is plotted.
A heatmap visualizes the correlation matrix, offering a detailed view of feature interrelationships.

6. Data Splitting and Feature Scaling:
The dataset is split into training and testing sets (80% training, 20% testing).
Feature scaling is performed using the StandardScaler to standardize the features.

7. Model Building:
Three regression models are trained:
Multiple Linear Regression: Using the LinearRegression class.
Random Forest Regression: Utilizing the RandomForestRegressor class.
XGBoost Regression: Employing the XGBRFRegressor class.

For each model:
The model is trained on the training set.
Predictions are made on the test set.
The R-squared metric (r2_score) evaluates the model's performance.

8. Prediction for New Data Points:
The script predicts charges for two hypothetical customers, 'Frank' and 'Sara', using the XGBoost regression model. Both customers' details, such as age, BMI, and other relevant data, are provided as input to the model, after which the respective insurance charges are predicted.
In conclusion, this script showcases a structured data science pipeline—from data loading, preprocessing, model training, and to making predictions on new data points—for predicting insurance charges.

In summary, the code provides a systematic approach to regression analysis, from initial data exploration and preprocessing to model training and prediction. The use of multiple models and evaluation metrics ensures a robust and comprehensive analysis.
