# Household Power Consumption — Time-Series Analysis

## Project Overview

This project analyzes household electricity consumption using time-series exploratory data analysis, preprocessing, feature engineering, K-Means clustering, anomaly detection, and automated machine learning.

The main objective is to understand electricity usage patterns and predict future electricity consumption.

## Dataset

**Dataset:** Individual Household Electric Power Consumption

**Source:** https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption

**Original file:** `household_power_consumption.txt`

The dataset contains household electricity measurements recorded approximately every minute over several years.

Measurements include global active power, global reactive power, voltage, global intensity, and three sub-metering values.

The original dataset is not included in this repository because it exceeds the GitHub browser-upload size limit.

## Part 1a: Exploratory Data Analysis

The exploratory analysis includes:

- Examining dataset dimensions and missing values.
- Converting date and time into a datetime index.
- Handling missing measurements using time-based interpolation.
- Analyzing daily, hourly, and monthly electricity consumption.
- Comparing electricity usage by season and day of the week.
- Investigating relationships between electrical measurements.
- Creating additional time-based features.

## Part 1b: Clustering and Anomaly Detection

Hourly electricity measurements were prepared for unsupervised learning.

K-Means clustering was used to identify groups of hours with similar electricity consumption characteristics.

The analysis included feature scaling, elbow method evaluation, silhouette scores, and PCA visualization.

Isolation Forest was used to identify potentially unusual electricity consumption patterns.

Potential anomalies were examined and retained because unusually high or low consumption does not necessarily indicate an invalid observation.

## Part 1c: AutoViML Machine Learning

AutoViML was used to predict the next hour's average global active power.

Features included electrical measurements, calendar variables, historical power consumption, and rolling averages.

A chronological 80/20 training and testing split was used to preserve the temporal order of the data.

The model was evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

A persistence baseline was also evaluated to compare the AutoViML model against a simple prediction strategy.

## How to Run

1. Download the dataset from the UCI Machine Learning Repository.
2. Extract `household_power_consumption.txt`.
3. Open `Household_Power_Analysis.ipynb` in Google Colab.
4. Upload the text dataset when prompted.
5. Install the required Python libraries.
6. Apply the AutoViML compatibility adjustments documented in the notebook if necessary.
7. Run all notebook cells in order.
8. Review the visualizations and evaluation metrics.

## Key Findings

The analysis explores variations in electricity consumption across different time periods.

Clustering identifies recurring consumption profiles, while anomaly detection highlights unusual observations.

AutoViML provides a machine-learning approach for predicting short-term electricity demand.

The model's effectiveness is assessed against the persistence baseline using the held-out testing data.

## Limitations

The dataset represents one household, so the results may not generalize to other households.

Time-series forecasting can also be affected by seasonal changes, unusual consumption events, and differences between training and testing periods.

## Conclusion

This project demonstrates the application of exploratory data analysis, clustering, anomaly detection, and automated machine learning to household electricity consumption data.
