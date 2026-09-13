# ML Models for Predicting Atmospheric Emissions

Final Group Project for CSCK503 Machine Learning in Practice.

## Project overview

This project develops supervised machine-learning models to predict 2019 major-road NOx emissions in Greater London using traffic and road characteristics from the London Atmospheric Emissions Inventory (LAEI) 2019.

## Data

The project uses two LAEI 2019 datasets:

- Major-road vehicle kilometres, traffic flows and speeds
- Major-road NOx, PM and CO2 link emissions

The datasets are joined using the road-link TOID identifier.

The shared processed dataset used by all three models is:

`laei2019_model_data.csv`

The primary target is:

`NOx_total_2019`

The common predictor set contains vehicle-specific AADT traffic flows, general traffic speed, road-link length and road classification.

Vehicle-kilometre variables are excluded from the primary models because they are derived traffic-activity measures closely related to the construction of road-emission inventories. Vehicle-specific NOx emissions are also excluded to avoid target leakage.

## Models

- Regression - Brentin Govender
- Random Forest Regressor - Dooshina Oolun
- Gradient Boosting Regressor - Adam Ayad



## Evaluation metrics

Models will be compared using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R²

A common dataset and evaluation approach will be used to ensure that the models can be compared fairly.
