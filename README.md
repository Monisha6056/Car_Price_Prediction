# Car_Price_Prediction
1. Project Objective
The goal of this project was to predict car prices using historical data. The prediction model was built using Linear Regression, which establishes a relationship between the features of the car and its price.
2. Dataset Overview
I worked with two datasets: a training dataset to build the model and a test dataset for evaluation.
The datasets included features like car make, model, location, engine power, transmission type, fuel type, and other car specifications. The target variable was the car price.
3. Data Cleaning and Preprocessing
I started by handling missing and duplicate values:
Columns with excessive null values (like body_type) were dropped.
For numerical columns like Distance, engine_power, seat_count, and door_count, I filled missing values with either the mean or median, depending on the distribution.
Categorical variables (Maker, model, Owner Type, etc.) were encoded using Label Encoding to convert them into numerical format.
I identified and removed outliers using z-score normalization, retaining only data points within ±2 standard deviations.
4. Feature Scaling
To ensure all features were on the same scale, I applied StandardScaler, which standardizes data by removing the mean and scaling to unit variance.
5. Model Building
For the training dataset:
I separated the features (X) and the target variable (y).
Built a Linear Regression model using the sklearn library.
The model's coefficients and intercept were calculated, representing how much each feature contributes to the car price.
6. Model Evaluation
To evaluate the model's performance on the training data:
I calculated metrics like Mean Squared Error (MSE) and Mean Absolute Error (MAE) to assess prediction accuracy.
The model achieved a reasonable fit, as indicated by its R² score.
7. Prediction on Test Data
For the test dataset:
Preprocessed it in the same way as the training data (handling null values, encoding, scaling, and removing outliers).
Used the trained Linear Regression model to predict car prices.
Finally, I combined the Id column with predicted prices and exported the results as a CSV file.
8. Key Insights
This project demonstrated the importance of data preprocessing and how linear regression can be used to understand the relationship between various car attributes and their prices.
The model provided interpretable results, such as how much a feature (e.g., engine power or car age) influenced the price.
