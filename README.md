# House-Pricing-Prediction-Model-Comparison

Project Overview
This project involves predicting house prices using machine learning models based on real estate data. The dataset includes key house features (e.g., bedrooms, bathrooms, lot size, house size) and location information (e.g., zip codes). The goal is to analyze and predict house prices accurately while identifying the most impactful features influencing price variations.

Datasets:

Real Estate Pricing Data:

Contains historical price trends across different regions, including zip codes and counties.
Used to understand location-based pricing patterns.
House Features Dataset:

Includes house-specific attributes such as number of bedrooms, bathrooms, lot size, and house size.
Provides details like zip code and previous sale date.

Machine Learning Models
The following models were implemented and evaluated:

Linear Regression:

A baseline model to capture simple relationships between features and prices.
Metrics: 
𝑅 Squared, Mean Squared Error (MSE), Mean Absoloute Error (MAE)

Decision Tree:

Captures non-linear relationships and feature interactions.
Tuned for depth and splits to balance overfitting and underfitting.

Random Forest:

Ensemble of decision trees to reduce variance and improve generalization.
Delivered the best performance with 
𝑅 Squared
 ≈0.9995
 
Performance Metrics
The models were evaluated using:

Mean Absolute Error (MAE): Average error magnitude.
Mean Squared Error (MSE): Penalizes larger errors more heavily.
R-squared:
Proportion of variance explained by the model.

Key Steps
Data Preprocessing:

Merged datasets on zip code to combine location and house-specific features.
Handled missing values, duplicate rows, and inconsistent data types.
Normalized numerical features using StandardScaler.
Feature Selection:

Selected key features influencing house prices:
Number of bedrooms (bed)
Number of bathrooms (bath)
Lot size in acres (acre_lot)
House size (house_size)
Added zip code as a categorical feature using one-hot encoding.
Model Training and Evaluation:

Split data into training and test sets (80/20 split).
Trained models and evaluated using performance metrics.
Results
Random Forest achieved the best performance
Decision Tree and Linear Regression also provided insights but were outperformed by Random Forest.

Technologies Used
Python:
Libraries: pandas, scikit-learn, numpy, matplotlib.
Machine Learning Models:
LinearRegression, DecisionTreeRegressor, RandomForestRegressor.
Future Work
Feature Expansion:
Incorporate external datasets (e.g., school ratings, crime statistics, proximity to amenities) to enhance predictions.
Geographical Generalization:
Extend the analysis to other cities or states.
Hyperparameter Tuning:
Optimize models further using advanced techniques like GridSearchCV or RandomizedSearchCV.
