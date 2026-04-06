# Analysis and Prediction of Used Car Prices

## Overview
This project predicts used car prices using regression models trained on vehicle data such as engine size, mileage, and fuel type.

## Dataset
Features include:
- **Target:** `Price`
- **Numerical:** `Year`, `Kilometer`, `Engine`, `Max Power`, `Max Torque`
- **Categorical:** `Fuel Type`, `Transmission`, `Make`, `Location`, `Seller Type`

## Key Work
- **Data cleaning:** Converted string-based fields (e.g., `"1248 cc"`, `"74 bhp"`) into numeric values  
- **Feature selection:** Dropped `Model` due to high cardinality  
- **Preprocessing:** Applied One-Hot encoding and scaling using a pipeline to avoid data leakage  

## Models
- Linear Regression
- K-Nearest Neighbors (KNN)
- Decision Tree Regressor  

## Results
- **Best model:** KNN
- Price range: 49,000 – 12,900,000  


| Metric | Training Phase | Final Evaluation (Unseen Data) |
| :--- | :--- | :--- |
| **RMSE** | ~599,000 | **~703,000** |
