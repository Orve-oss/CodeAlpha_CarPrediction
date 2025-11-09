# Car Price Prediction with Machine Learning  
**CodeAlpha Data Science Internship – Task 3**

Predicts used car **selling price** based on features like present price, kilometers driven, fuel type, age, and more using **regression models**.

---

## Project Overview

- **Task**: Car Price Prediction  
- **Dataset**: `car data.csv` (301 rows, 9 features)  
- **Target**: `Selling_Price` (in Lakh)  
- **Models Used**:  
  - Linear Regression  
  - **Random Forest Regressor** (Best performer)  
- **Key Libraries**: `pandas`, `scikit-learn`, `matplotlib`, `seaborn`, `joblib`

---

## Dataset Features

| Feature | Description |
|-------|-------------|
| `Present_Price` | Current ex-showroom price (Lakh) |
| `Driven_kms` | Total kilometers driven |
| `Fuel_Type` | Petrol / Diesel / CNG |
| `Selling_type` | Dealer / Individual |
| `Transmission` | Manual / Automatic |
| `Owner` | Number of previous owners |
| `Year` → `Age` | Car age in 2025 |
| `Selling_Price` | **Target**: Price car was sold for |

> **Note**: `Car_Name` dropped due to high cardinality (98 unique values).

---

## Model Performance

| Model | MAE | MSE | RMSE | R² Score |
|------|-----|-----|------|----------|
| **Random Forest** | **0.58** | **0.97** | **0.98** | **0.96** |
| Linear Regression | 1.23 | 4.12 | 2.03 | 0.83 |

**Random Forest is the final model** due to superior accuracy and ability to capture non-linear patterns.

