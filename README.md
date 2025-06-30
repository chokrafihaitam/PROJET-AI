# Real Estate Price Prediction Analysis

This project focuses on scraping real estate data from Mubawab, cleaning and preprocessing it, conducting exploratory data analysis (EDA), and applying regression models to predict property prices.

## Key Data Insights
- The dataset initially contains **1400** listings with 8 features.
- After cleaning, **1339** listings and **14** features remain.
- Average property price is approximately **5729682.56 DH**, with a median of **2100000.00 DH**.

- Price distribution and variation are visualized in the plot saved at `visualizations/price_distribution_HAITAM_CHOKRAFI.png`.

## Data Preprocessing Details
A sample of the cleaned dataset is shown below:

```
     Prix   Surface    Pieces  Chambres  SallesDeBain  Ville_Casablanca  Ville_Marrakech  Ville_Rabat  Ville_Tanger  TypeBien_Appartement  TypeBien_Maison  TypeBien_Riad  TypeBien_Villa  Titre_length
-0.217653 -0.455549 -1.020118 -0.739313     -0.353693               0.0              0.0          0.0           1.0                   1.0              0.0            0.0             0.0          63.0
-0.147399 -0.404648 -0.664127 -0.739313     -0.979315               0.0              0.0          0.0           1.0                   1.0              0.0            0.0             0.0          63.0
-0.213057 -0.368525 -0.664127 -0.739313     -0.353693               0.0              0.0          0.0           1.0                   1.0              0.0            0.0             0.0          48.0
-0.143897 -0.444055 -0.308136 -0.739313     -0.353693               0.0              0.0          0.0           1.0                   1.0              0.0            0.0             0.0          41.0
-0.181432 -0.375092 -0.308136 -0.133845     -0.353693               0.0              0.0          0.0           1.0                   1.0              0.0            0.0             0.0          25.0
```

The cleaned dataset has been saved as `mubawab_data_HAITAM_CHOKRAFI.csv`.

## Model Performance Summary
Several regression models were evaluated for their predictive accuracy. Metrics for each model are presented below:

| Model               | R²    | RMSE       | MAE        |
|---------------------|-------|------------|------------|
| Linear Regression   | 0.785 | 47097.02 | 38358.67 |
| Log Regression      | 0.698 | 55772.67 | 42099.84 |
| Random Forest       | 0.698 | 55836.02 | 45852.00 |
| Gradient Boosting   | 0.732 | 52593.81 | 43562.65 |

## Visualizations
- **Linear Regression Analysis:** See `visualizations/linear_regression_HAITAM_CHOKRAFI.png` for predicted vs actual prices and feature importance.
- **Model Comparisons:** Detailed plots of model predictions saved at `visualizations/model_comparison_HAITAM_CHOKRAFI.png`.
- **Performance Metrics:** Bar charts comparing model performances at `visualizations/performance_comparison_HAITAM_CHOKRAFI.png`.

## Conclusion & Next Steps
The linear regression model performed best with an R² around 0.78. Further improvements could include feature engineering, hyperparameter tuning, and exploring advanced models like XGBoost.

