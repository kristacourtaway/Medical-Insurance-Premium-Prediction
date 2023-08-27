# Medical Insurance Premium Prediction

The Python code demonstrates a data science project that utilizes machine learning techniques to predict insurance charges. It starts by importing crucial libraries, including NumPy, Pandas, Matplotlib, Seaborn, and modules from the sci-kit-learn package. The dataset originates from a CSV file named 'insurance.csv.'

The data exploration phase examines the dataset's structure, dimensions, and types. It identifies both categorical and numerical columns. The code generates a statistical summary of the dataset to gain insights into its central tendencies and distribution. Additionally, it groups the dataset based on categorical variables like 'sex,' 'smoker,' and 'region' to grasp the average charges within each subgroup.

The code confirms the existence of missing values and then encodes categorical data using one-hot encoding for columns such as 'sex,' 'smoker,' and 'region.' It computes the correlation matrix, illustrating relationships between features and the target variable ('charges'). A bar plot displaying correlations and a heatmap visualize these relationships effectively.

The dataset is split into training and testing sets using the 'train_test_split' function from the sci-kit-learn library. The Python code applies feature scaling by standardizing the features. The subsequent section focuses on constructing regression models, employing three distinct techniques:

Multiple Linear Regression: The code trains a linear regression model using the training data and evaluates its performance on the testing data. It assesses the model's effectiveness using the coefficient of determination (R-squared).

Random Forest Regression: Using a Random Forest regressor with 100 estimators, the code trains and evaluates the model similarly to the linear regression approach.

XGBoost Regression: Similar to the previous models, an XGBoost regressor is trained and evaluated following the same procedure.

The code concludes by providing examples of predicting insurance charges for new customers using the trained XGBoost regressor. It presents two customer profiles featuring attributes like age, BMI, number of children, sex, smoker status, and region. The regressor predicts the corresponding charges based on these feature sets.

In summary, the provided Python code serves as a comprehensive demonstration of a data science workflow. It covers multiple phases, including data loading, exploration, preprocessing, constructing and evaluating various regression models (multiple linear regression, random forest regression, and XGBoost regression), and applying these models to predict insurance charges for new customers. This code effectively illustrates the practical application of machine learning in real-world scenarios involving insurance charge predictions.
