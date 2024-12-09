Rainfall Prediction Across Australian Cities
================

## **Project Overview**

This project aims to forecast monthly rainfall patterns for selected
cities in Australia: Darwin, Perth, Sydney, and Melbourne. By leveraging
advanced machine learning and time series models, we aim to support
organizations in improving preparedness and mitigating the effects of
extreme weather events.

## **Table of Contents**

1.  [Objective](#objective)
2.  [Dataset](#dataset)
3.  [Methodology](#methodology)
4.  [Results](#results)
5.  [Key Findings](#key-findings)
6.  [Challenges](#challenges)
7.  [Future Work](#future-work)
8.  [Installation and Usage](#installation-and-usage)
9.  [Contributing](#contributing)
10. [License](#license)

## **Objective**

To develop accurate and interpretable models that forecast monthly
rainfall patterns, enabling stakeholders in industries such as
agriculture and infrastructure to respond effectively to challenges
posed by climate variability.

# Dataset

- **Source**: Australian Bureau of Meteorology  
- **Size**: ~145,000 daily weather observations aggregated into monthly
  data  
- **Features**: Rainfall, temperature, wind speed, cloud coverage,
  humidity, and more  
- **Preprocessing**: Missing value imputation, feature derivation, data
  aggregation, and time series formatting

# Methodology

## Exploratory Data Analysis (EDA)

- Investigated patterns and correlations across features.
- Visualized trends and seasonal variability in rainfall.

## Modeling

- **Linear Regression**: Baseline model to evaluate relationships
  between predictors.
- **ARIMA**: Time series model for univariate forecasting, capturing
  seasonality and trends.
- **XGBoost**: Tree-based ensemble model incorporating external
  predictors for robust forecasting.

## Evaluation Metrics

- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)

## Results

- **Best Model**: XGBoost achieved the lowest RMSE and MAE across
  cities.
- **Key Metrics**:
  - **Sydney**: XGBoost RMSE = 83.202, MAE = 52.196
  - **Perth**: XGBoost RMSE = 33.023, MAE = 24.536
  - **Darwin**: XGBoost RMSE = 88.583, MAE = 60.525
  - **Melbourne**: XGBoost RMSE = 26.023, MAE = 17.362
- For detailed performance metrics, see the Results Summary Table.

## Key Findings

- XGBoost excelled in handling the complex relationships and variability
  in rainfall data.
- ARIMA provided reliable trend analysis but struggled with variability.
- Linear Regression highlighted significant predictors but was less
  effective due to non-linear trends.

## Challenges

- High variability in rainfall across cities posed difficulties for all
  models.
- Data sparsity and missing values required extensive preprocessing.
- Extreme rainfall events, particularly in Darwin, were challenging to
  predict.

## Future Work

- Expand the geographic scope to include more regions of Australia.
- Incorporate advanced climate indices (e.g., ENSO, IOD) for better
  predictions.
- Develop real-time forecasting pipelines for dynamic weather
  monitoring.
- Experiment with deep learning models for improved accuracy.
