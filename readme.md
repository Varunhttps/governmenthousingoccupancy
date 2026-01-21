# Predicting Occupancy Rate of Government Housing Projects in India

## Problem Statement
This project aims to predict the percentage of government-developed houses that are occupied in each Indian state using publicly available housing data.

## Dataset
Source: https://www.data.gov.in/sector/Housing  
The dataset contains state-wise information on housing projects, investment, and physical progress.

## Approach
- Data cleaning and preprocessing
- Feature engineering (Occupancy Percentage)
- Train-test split
- Linear Regression model
- Evaluation using RMSE
- Visualization of actual vs predicted values

## Model Used
- Linear Regression

## Evaluation Metric
- Root Mean Squared Error (RMSE)

## Results
The model captures the general trend between housing project progress and occupancy, with reasonable accuracy given the small dataset.

## Tools & Technologies
- Python
- pandas
- scikit-learn
- matplotlib

## Limitations
- Small dataset (state-level aggregation)
- No time-series information
- State-specific policy factors not included

## Future Improvements
- Try advanced models (Ridge, Random Forest)
- Add more government datasets
- Perform deeper exploratory data analysis
