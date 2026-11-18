# NYC Airbnb — Exploratory Data Analysis and Machine Learning

## Project Overview

This project analyzes the New York City Airbnb 2019 dataset to explore rental pricing, listing characteristics, neighborhood differences, and patterns in Airbnb accommodations.

The analysis includes exploratory data analysis (EDA), data cleaning, feature engineering, K-Means clustering, anomaly detection, and automated machine learning using AutoViML.

## Dataset

**Dataset:** New York City Airbnb Open Data (2019)

**Source:** https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data

**Main file:** `AB_NYC_2019.csv`

The original dataset contains 48,895 Airbnb listings and 16 columns, including listing prices, neighborhoods, room types, minimum nights, reviews, and availability.

Additional large datasets, such as `calendar.csv`, `listings.csv`, and `reviews.csv`, are not included because of GitHub upload limitations. They are not required for the analysis in this notebook.

## Part 1a: Exploratory Data Analysis

The exploratory analysis focuses on:

- Examining dataset structure and descriptive statistics.
- Identifying missing values and duplicate records.
- Cleaning missing listing names and host names.
- Handling missing review information.
- Investigating rental prices and minimum-night requirements.
- Exploring listing distributions by neighborhood and room type.
- Visualizing relationships between listing characteristics.

After removing 11 zero-price records, the cleaned dataset contains 48,884 listings.

## Part 1b: Clustering and Anomaly Detection

K-Means clustering was applied to identify groups of Airbnb listings with similar characteristics.

The analysis included:

- Encoding categorical variables.
- Scaling numerical features.
- Testing different numbers of clusters.
- Evaluating inertia and silhouette scores.
- Visualizing clusters using Principal Component Analysis (PCA).
- Identifying potential anomalies using Isolation Forest.

Eight clusters were selected in the analysis. Isolation Forest flagged approximately 5% of listings as potential anomalies.

These observations were investigated because unusual listings do not necessarily represent incorrect data.

## Part 1c: AutoViML Machine Learning

AutoViML was used to investigate Airbnb price prediction using listing characteristics.

The regression target was transformed using `log1p(price)` to reduce the influence of highly skewed prices.

Predictive features included neighborhood information, room type, geographical coordinates, minimum nights, reviews, host activity, and availability.

The dataset was divided into training and testing sets using an 80/20 split.

Model performance should be interpreted using the evaluation results generated in the notebook.

## Key Findings

The analysis demonstrates that Airbnb listings vary considerably in price, availability, minimum-stay requirements, and other characteristics.

Clustering revealed different listing profiles, while anomaly detection identified listings with unusual combinations of characteristics.

## Limitations

The dataset represents Airbnb listings from 2019 and may not reflect current rental market conditions. Clustering and anomaly detection are exploratory techniques, and their results require interpretation.

## Conclusion

This project demonstrates how data preprocessing, exploratory analysis, clustering, anomaly detection, and automated machine learning can be applied to a real-world accommodation dataset.
