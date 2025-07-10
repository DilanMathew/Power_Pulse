**Overview**
PowerPulse is a machine learning project that predicts household energy consumption using historical power consumption data. The goal is to provide actionable insights for energy management, helping both consumers and energy providers optimize usage, reduce costs, and support sustainability initiatives.

This project demonstrates advanced techniques in data preprocessing, feature engineering, regression modeling, and visualization.

**Problem Statement**
In today’s world, accurate energy consumption forecasting is crucial for:

Reducing household energy bills.

Enabling energy providers to manage demand efficiently.

Supporting smart grid integration and sustainability goals.

This project builds predictive models to estimate Global Active Power consumption and identify key drivers of energy usage.
**Dataset**
Individual Household Electric Power Consumption Dataset

Records: ~2 million

Features:

Date, Time

Global_active_power (target)

Global_reactive_power

Voltage

Global_intensity

Sub_metering_1, Sub_metering_2, Sub_metering_3

Skills Demonstrated
✅ Data Preprocessing (handling nulls, parsing dates, scaling)
✅ Feature Engineering (rolling averages, peak hours, anomaly detection)
✅ Regression Modeling (Linear Regression, Random Forest, Gradient Boosting, Neural Networks)
✅ Hyperparameter Tuning (GridSearchCV)
✅ Evaluation Metrics (RMSE, MAE, R²)
✅ Data Visualization (matplotlib, seaborn)

📈 Approach
Data Understanding & EDA

Explored feature distributions, trends, and anomalies.

Visualized time-series energy usage.

Data Preprocessing

Parsed date-time features.

Removed outliers using Z-score and IQR methods.

Created new features:

Daily_Avg_Global_active_power

Is_Peak_Hour

Rolling_Avg_3H, Rolling_Avg_24H

Feature Engineering

Selected relevant predictors excluding redundant ones (e.g., Global_intensity).

Model Training & Evaluation

Split data into train/test sets (80:20).

Trained:

Linear Regression

Random Forest Regressor (Tuned)

Gradient Boosting Regressor (Tuned)

Neural Network (MLPRegressor)

Evaluated models using RMSE, MAE, and R².

📊 Results
Model	RMSE	MAE	R² Score
Linear Regression	0.000285	0.000179	0.9685
Random Forest	0.000162	0.000114	0.9821
Gradient Boosting	0.000192	0.000126	0.9788
Neural Network	0.000180	0.000121	0.9801

✅ Best Model: Random Forest Regressor (Tuned)

🔑 Key Insights
Top Predictors:

Rolling_Avg_3H

Sub_metering_1

Daily_Avg_Global_active_power

Global_reactive_power

Voltage

Energy usage peaks during specific hours and days.

Strong correlation between sub-metering and global power consumption.

📊 Visualizations
Distribution & Boxplots of key features

Correlation Heatmap

Time-series plots of energy usage

Feature Importance Charts

Actual vs Predicted Scatterplots for all models

📋 Project Deliverables
✅ Jupyter Notebook with complete code and markdown explanations
✅ Report summarizing:

Approach

Data Analysis

Model Evaluation

Insights and Recommendations
✅ Visualizations folder for quick reference

🚀 Technologies Used
Python (pandas, numpy, matplotlib, seaborn, scikit-learn)

Jupyter Notebook

Machine Learning: Linear Regression, Random Forest, Gradient Boosting, Neural Networks

