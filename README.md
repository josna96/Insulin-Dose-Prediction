# Predicting Regular Insulin Dosage for Diabetes Patients

This project aims to predict **regular insulin dosage levels** for diabetes patients using a dataset containing timestamped events, glucose measurements, meal ingestion details, and other relevant features.

## Dataset Description

The dataset consists of four fields per record:
- **Date**: MM-DD-YYYY format.
- **Time**: XX:YY format.
- **Code**: Numerical codes indicating the type of event (e.g., glucose measurement, insulin dose).
- **Value**: Numeric value corresponding to the event (e.g., glucose level, insulin dosage).

### Key Codes:
- `33`: Regular insulin dose (Target variable).
- `48-64`: Blood glucose measurements (pre/post meals).
- `66-71`: Meal ingestion and exercise activities.

## Project Overview

1. **Data Preprocessing**:
   - Cleaned and preprocessed the dataset, including timestamp conversion and filtering for regular insulin dosage events.
   - Created features based on pre- and post-meal glucose levels.

2. **Exploratory Data Analysis (EDA)**:
   - Visualized the distribution of regular insulin dosages and examined patterns in glucose levels and insulin requirements.

3. **Model Training and Evaluation**:
   - Built predictive models using machine learning algorithms like Linear Regression and Random Forest.
   - Evaluated models with metrics such as Mean Squared Error (MSE), Mean Absolute Error (MAE), and R-squared (R²).

4. **Insights and Challenges**:
   - Found that pre- and post-glucose levels are the most influential features for predicting insulin dosage.

## Random Forest Regression Model Performance

- **Mean Squared Error (MSE)**: 17.298441916207455
- **Mean Absolute Error (MAE)**: 3.048767699986335
- **R-squared (R²)**: 0.1870124947550219

### Feature Importance:
- Pre-Glucose Level: 0.4747
- Post-Glucose Level: 0.4178
- Hypoglycemic Symptoms: 0.0257
- Typical Meal Ingestion: 0.0304
- More-than-usual Meal Ingestion: 0.0334
- Less-than-usual Meal Ingestion: 0.0018
- Typical Exercise Activity: 0.0038
- More-than-usual Exercise Activity: 0.0066
- Less-than-usual Exercise Activity: 0.0058

## Conclusion

The project demonstrated the feasibility of predicting regular insulin dosage using machine learning. While the model achieved moderate performance, further improvements can be made with:

1. Advanced feature engineering (e.g., incorporating time-series patterns and additional contextual data).
2. Fine-tuning hyperparameters for optimal performance.

## Future Work

- Experiment with time-series models (e.g., LSTMs) for sequential data analysis.
- Investigate additional external factors affecting insulin dosage.
- Enhance model explainability with SHAP values or feature importance plots.

---

## How to Run

1. Clone this repository:
   ```bash
   git clone <repository-url>
