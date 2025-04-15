Diabetes Disease Progression Prediction
This project builds regression models to predict diabetes progression using clinical features like BMI, blood pressure, and serum measurements. It emphasizes model performance, interpretability, and robustness using SHAP, cross-validation, and permutation importance.

Dataset
Source: sklearn.datasets.load_diabetes()

442 patient records

10 physiological features (e.g., age, BMI, BP, serum markers)

Target: Disease progression after one year

Methods Used
Linear Regression

Ridge Regression

XGBoost Regressor

Polynomial Feature Engineering (degree=2)

Cross-Validation (5-fold)

SHAP for feature impact

Permutation Feature Importance

Evaluation Metrics
Models were evaluated using:

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

Mean Absolute Error (MAE)

R² Score

Model	MSE	RMSE	MAE	R² Score
Linear Regression	~2892	~53.78	~43.83	~0.45
Ridge Regression	~2892	~53.78	~43.83	~0.45
XGBoost Regressor	~3351	~57.89	~46.70	~0.37
Interpretability
SHAP Summary Plots show the global impact of features on predictions

Permutation Importance validates feature relevance across models

Key Findings
BMI and s5 (blood sugar) are the most important predictors

Linear and Ridge models outperform XGBoost on this dataset

Model generalizes well with 5-fold cross-validation (R² ~0.45)

Install dependencies:

pip install shap xgboost scikit-learn matplotlib seaborn
