
# 🩺 Diabetes Disease Progression Prediction using Regression and SHAP

This project predicts diabetes progression using regression models and explains clinical feature impact with SHAP. It provides a transparent, interpretable, and reproducible machine learning pipeline for healthcare risk prediction.

---

## 🚀 Project Highlights

- 📊 Trained **Linear**, **Ridge**, and **XGBoost** regression models  
- 📈 Achieved **R² ≈ 0.45** using clinical indicators like BMI and blood sugar  
- 🔍 Applied **SHAP** and **Permutation Importance** for model interpretability  
- ➕ Included **Polynomial Feature Engineering** (degree=2)  
- ✅ Validated performance using **5-fold Cross-Validation**

---

## 🧪 Methodology

### 1. Data Preparation
- Loaded the diabetes dataset from `sklearn.datasets`
- Standardized features using `StandardScaler`
- Created non-linear interaction terms using `PolynomialFeatures`

### 2. Model Training
- Trained and compared: `LinearRegression`, `Ridge`, and `XGBRegressor`
- Evaluated using: MSE, RMSE, MAE, and R² Score
- Validated results with cross-validation

### 3. Model Interpretability
- Used **SHAP Summary Plots** to explain model predictions  
- Added **Permutation Feature Importance** to validate key predictors

---

## 📊 Results

| Model               | MSE   | RMSE  | MAE   | R² Score |
|---------------------|-------|-------|-------|----------|
| Linear Regression   | ~2892 | ~53.78| ~43.83| ~0.45    |
| Ridge Regression    | ~2892 | ~53.78| ~43.83| ~0.45    |
| XGBoost Regressor   | ~3351 | ~57.89| ~46.70| ~0.37    |

---

## 📂 Folder Structure

```
diabetes-progression-prediction/
├── README.md
├── requirements.txt
├── Diabetes Disease predcition.ipynb
```

---

## ⚙️ How to Run

Install dependencies:

```
pip install -r requirements.txt
```

Or manually:

```
pip install scikit-learn shap xgboost matplotlib seaborn
```

Run the notebook:

```
jupyter notebook Diabetes\ Disease\ predcition.ipynb
```

---

