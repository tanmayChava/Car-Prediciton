# Car-Prediciton
Used Car Price Prediction
A machine learning project that predicts the selling price of used cars using data from CarDekho. The goal is to build a robust regression model that accurately estimates car prices based on features like age, kilometers driven, fuel type, transmission, and more.

📁 Dataset
Source: CarDekho (public dataset)

Format: CSV
 
Columns Include:

name: Car model name (dropped during preprocessing)

year: Year of purchase

km_driven: Kilometers the car has been driven

fuel, seller_type, transmission, owner: Categorical features

selling_price: Target variable

✅ Project Workflow
1. Exploratory Data Analysis (EDA)
Visualized numeric and categorical distributions

Analyzed skewness and outliers using boxplots and histograms

Identified relationships between features and selling price

2. Feature Engineering
Created car_age = 2025 - year

Applied log1p() transformation to km_driven and selling_price to reduce skew

One-hot encoded categorical variables

Removed unnecessary features (name, year)

3. Modeling
Compared several regression models:

Linear Regression

Decision Tree Regressor

Random Forest Regressor

XGBoost Regressor

Evaluated with:

MAE (Mean Absolute Error)

RMSE (Root Mean Squared Error)

R² Score (Goodness of fit)

4. Hyperparameter Tuning
Used GridSearchCV to optimize XGBoost parameters:

📦 Tech Stack
Python

Pandas, NumPy

Seaborn, Matplotlib

Scikit-learn

XGBoost

🔮 Future Improvements
Extract brand/model from car name

Add location-based pricing features

Use SHAP for explainable AI (XAI)

Try LightGBM or CatBoost for comparison
