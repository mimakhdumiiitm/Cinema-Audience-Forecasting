# Cinema Audience Forecasting

An end-to-end Machine Learning pipeline developed for the **Machine Learning Practice** course of the **IIT Madras BS Degree in Data Science and Applications**. 

This project was built for a Kaggle competition hosted under the academic curriculum. Since the competition has been set to private by the authorities, this repository serves as a standalone archive containing the complete implementation, exploratory insights, and model pipelines.

## 📌 Project Overview
The core objective is to accurately predict the daily cinema audience count (`audience_count`) for various theaters based on integrated data from both online ticketing platforms and offline Point of Sale (POS) booking engines.

## 𝕿 Data Sources & Integration
The project heavily relies on comprehensive feature engineering across multiple raw tracking systems:
* **BookNow Platform:** Online transactional records (`booknow_booking.csv`) and associated metadata.
* **CinePOS System:** Over-the-counter offline booking records (`cinePOS_booking.csv`) and venue details.
* **Contextual Maps:** Mapping indices to match vendor theater IDs (`movie_theater_id_relation.csv`) along with calendar indicators (`date_info.csv`).

The raw data structures were systematically fused through two primary integration methodologies:
1.  **Granular Feature Integration:** Unifying timestamped offline and online ticket sales pipelines to analyze seasonal, hourly, and weekend-specific behaviors (`is_weekend`).
2.  **Show-Level Aggregation:** Systematically matching exact performance dates across mapping keys to compute aggregate operational indicators.

## 🛠️ Machine Learning Pipeline

### 1. Data Imputation & Outlier Mitigation
* Handling localized data dropouts (e.g., structural geometry calculations across diverse theater sets).
* Handling ticket outlier skewness using advanced capping transformations (95th percentile pruning).
* Expanding sparse descriptors into robust binary layouts via automated `OneHotEncoder` pipelines.

### 2. Feature Isolation & Dimension Reduction
* Applying `SelectKBest` with Mutual Information Regression indicators to compute non-linear performance scores.
* Integrating `TruncatedSVD` components to achieve sparse vector reduction while ensuring minimum information loss.

### 3. Evaluated Model Architectures
* **Linear Baselines:** Scaled structural estimators via `LinearSVR` configurations.
* **Non-Linear Estimators:** Optimization architectures based on `DecisionTreeRegressor` parameters.
* **Ensemble & Boosting Engines:** Bagged model variations and residual `GradientBoostingRegressor` engines.
* **Advanced Gradient Boosting:** Implementation of optimized LightGBM frameworks tuned across rigorous `TimeSeriesSplit` cross-validation loops.
* **Classical Time-Series:** Stationarity baseline modeling using structural `ARIMA` components verified via Augmented Dickey-Fuller (ADF) checks.

## 📈 Key Outcomes
* Evaluated model variations using Coefficient of Determination ($R^2$) metrics, Mean Absolute Error ($MAE$), and Root Mean Squared Error ($RMSE$).
* Fine-tuned tree structures using automated `GridSearchCV` routines to manage operational bias-variance trade-offs.
