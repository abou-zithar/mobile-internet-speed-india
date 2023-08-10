# mobile-internet-speed-india
https://www.kaggle.com/datasets/kishan305/mobile-internet-speed-india?select=September_MySpeed_2021.csv
# Telecom Data Analysis and Predictive Modeling

This repository contains code for analyzing and predicting telecom network performance using a dataset containing various parameters related to signal strength, speed, technology, and more. The dataset consists of multiple CSV files that have been merged into a single dataframe for analysis.

## Getting Started

To get started, make sure you have the necessary libraries installed by running the following commands:

```bash
pip install pandas numpy seaborn matplotlib xgboost
```
## Data Collection and Preparation
The code begins by importing required libraries and setting up the environment. It reads CSV files from a specified directory, creates individual dataframes for each CSV, and then concatenates them into a single dataframe called "data". The resulting dataframe contains information about signal strength, speed, technology, and more.

## Data Cleaning
The data is then cleaned to handle missing values and format issues. The missing value percentage for each feature is calculated and displayed. The "signal_strength" feature is converted to float, and missing values are imputed with the mean value. Similarly, "speed" is converted from Kbps to Mbps, and missing values are imputed with the mean.

## Data Visualization
Several data visualizations are generated to gain insights into the dataset. Scatter plots, bar plots, and heatmaps are used to visualize the relationships between features. Key observations include the impact of technology on speed and signal strength, distribution of operators and technology across different regions, and more.

## Feature Engineering
One-hot encoding is performed on categorical features, resulting in an encoded dataframe named "encoded_Data". Correlation between features is visualized using a heatmap.

## Predictive Modeling
The dataset is split into training and testing sets. Decision Tree and XGBoost models are trained for predictive modeling. Model accuracy is evaluated on both training and testing datasets.

## Conclusion
This code demonstrates how to analyze and predict telecom network performance using a real-world dataset. It covers data cleaning, visualization, feature engineering, and predictive modeling. Feel free to explore and modify the code to suit your specific use case.
