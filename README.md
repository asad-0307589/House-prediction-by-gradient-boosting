📊 House Price Prediction using Gradient Boosting
📝 Task Objective
The goal of this project is to build a regression model that can accurately predict house prices based on various property features such as area, number of bedrooms, location attributes, and amenities.

📂 Dataset Used
Source: Housing.csv — A commonly used dataset containing residential house prices with features such as:

area, bedrooms, bathrooms, stories, parking

Binary columns: mainroad, guestroom, basement, hotwaterheating, airconditioning, prefarea

Categorical column: furnishingstatus

Target variable: price

🤖 Models Applied
Gradient Boosting Regressor (from sklearn.ensemble)

Pipeline with:

Feature preprocessing using ColumnTransformer

Feature scaling with StandardScaler (for numeric features)

One-hot encoding of furnishingstatus

Hyperparameter tuning using GridSearchCV with cross-validation

📈 Key Results and Findings
Best Parameters from Grid Search:

n_estimators=300, learning_rate=0.1, max_depth=5

Performance on Test Set:

MAE: 153,147

RMSE: 233,973

R² Score: 0.9857

Baseline MAE (predicting mean): 1,569,994
→ Improvement: 90.25% better than baseline

Visualization:

Actual vs Predicted plot shows strong alignment along the diagonal line.

Residuals are tightly distributed around 0, indicating low bias and variance.
