California Housing Regression Models Evaluation
 Overview

This project demonstrates the implementation and evaluation of multiple regression algorithms using the California Housing dataset from sklearn.datasets. The objective is to:
- Apply various regression techniques.
- Perform preprocessing, model training, and evaluation.
- Tune model hyperparameters using cross-validation.
- Select the best model based on evaluation metrics.
Dataset

- Source: fetch_california_housing() from sklearn.datasets
- Description: Contains information about California districts including:
  - Median income, house age, average rooms, etc.
  - Target variable: Median House Value (MedHouseVal)
Requirements

Install dependencies using pip:
pip install numpy pandas matplotlib seaborn scikit-learn

Implemented Models

The following regression algorithms were implemented:
- Linear Regression: Baseline linear model
- Decision Tree Regressor: Tree-based non-linear regression
- Random Forest Regressor: Ensemble of decision trees
- Gradient Boosting: Boosted decision trees for high accuracy
- Support Vector Regressor (SVR): Regression using SVM principles

 Evaluation Metrics

Each model is evaluated using the following metrics:
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R² Score (R-squared)

Cross-Validation & Tuning

Performed 5-fold cross-validation and hyperparameter tuning using:
- GridSearchCV for:
  - Decision Tree
  - Gradient Boosting
  - SVR

Results & Conclusion

The performance of all models was compared, and the best model was selected based on:
- Highest R² score on test set
- Lowest MAE and MSE
- Stable cross-validation performance

Example Result Table:

Model              | MSE   | MAE   | R²
-------------------|-------|-------|-------
Linear Regression | 0.52  | 0.45  | 0.60
Decision Tree     | 0.42  | 0.39  | 0.65
Random Forest     | 0.34  | 0.33  | 0.74
Gradient Boosting | 0.32  | 0.31  | 0.76 ✅
SVR               | 0.60  | 0.50  | 0.52 ❌

Best Performing Model: Gradient Boosting Regressor

Visualization

Exploratory Data Analysis (EDA) included:
- Feature distributions
- Correlation heatmaps
- Target relationships

:Learning Outcomes

- How to apply and evaluate regression algorithms.
- Importance of feature scaling.
- Effectiveness of hyperparameter tuning.
- Model comparison using reliable metrics.
 Author

sheji Adhil
Email: your.sheji882@gmail.com


