## Medical-Insurance-Premium-Prediction

The provided code undertakes a comprehensive regression analysis on the "insurance" dataset. The goal is to predict insurance charges based on several independent variables.

Correlation Analysis:
The first segment of the code assesses the correlation of each independent variable with the target variable, 'charges'. Two visualization techniques are employed:

A bar plot displays the linear correlation of each feature with 'charges'. This helps in quickly identifying which variables have a strong or weak association with the target.
A heatmap is used to show pairwise correlations between all variables in the dataset. The color intensity and annotations provide a detailed view of how each variable relates to others, offering insights into potential multicollinearity.
Data Splitting:
Before model training, the dataset is partitioned into independent variables (denoted by 'x') and the dependent variable (denoted by 'y', which is 'charges'). The data is then split into training and testing sets, with 80% reserved for training and 20% for testing. This allows for unbiased evaluation of model performance.

Feature Scaling:
To ensure that all features have the same scale and contribute equally to the model's predictions, the StandardScaler is used. This process standardizes the features to have a mean of 0 and a standard deviation of 1. Scaling is especially important for models like linear regression, which can be sensitive to the scale of input features.

Model Building:
Three regression models are trained on the data:

Multiple Linear Regression: A linear regression model attempts to fit the best linear relationship between the independent variables and the dependent variable.
Random Forest Regression: This ensemble method constructs multiple decision trees during training and outputs an average prediction of the individual trees for regression tasks.
XGBoost Regression: An advanced gradient-boosted decision tree algorithm known for its efficiency and performance.
For each model, predictions are made on the test set, and the R^2 score is computed to evaluate the model's performance. The R^2 score provides a measure of how well the model's predictions match the actual values.

Predicting for New Customers:
The final segment of the code demonstrates how the trained XGBoost model can be used to predict charges for new customers. Two examples are provided:

Frank: A 40-year-old male smoker from the northeast with a BMI of 45.5 and 4 children.
Sara: A 19-year-old non-smoking female from the northwest with a BMI of 27.9 and no children.
For each new customer, the data is structured and scaled appropriately before feeding it into the model for prediction.

In summary, the code provides a systematic approach to regression analysis, from initial data exploration and preprocessing to model training and prediction. The use of multiple models and evaluation metrics ensures a robust and comprehensive analysis.
