💧 Smart Water Leakage Detection

Sustainable Water Resource Management using AI/ML

Project Overview

This project analyzes pipeline sensor data to detect water leakages and optimize water usage. The goal is to support sustainable urban water management by leveraging AI/ML algorithms for proactive leak detection and monitoring.

📌 Week 1 Milestone – Data Preprocessing & EDA (30% Progress)

During Week 1, the primary focus was dataset preparation and exploratory analysis to understand patterns and relationships in the data.

🔹 Dataset Overview

Source: Smart Water Leak Detection Dataset – Kaggle

Key Columns:

Sensor readings: Flow_Rate, Pressure, Temperature, Vibration, RPM, Operational_Hours

Location info: Zone, Block, Pipe, Location_Code, Latitude, Longitude

Target variable: Leakage_Flag (continuous numeric for regression)

🔹 Data Preprocessing

Filled missing values in sensor readings

Encoded categorical variables (Zone, Block, Pipe, Location_Code)

Scaled numeric columns for uniformity

Cleaned dataset saved as: cleaned_dataset.csv

🔹 Exploratory Data Analysis (EDA)

Distribution plots for Flow_Rate and Pressure

Correlation heatmap of numeric features

Boxplots for outlier detection

Leakage distribution analysis (imbalanced dataset)

Pairplots to observe relationships between Flow, Pressure, and Leakage_Flag

Grouped averages to identify patterns indicating leaks

🔹 Week 1 Insights

Flow and Pressure are strong indicators of leakage events

Leakage events cluster around abnormal flow and pressure values

Dataset is now clean and ready for feature engineering and model building

📌 Week 2 Milestone – ML Model Development & Evaluation (60% Progress)
🔹 Model Choice & Justification

RandomForestRegressor chosen for its ability to handle non-linear relationships, work with mixed feature types, and provide feature importance insights.

Robust baseline model for regression on continuous Leakage_Flag.

🔹 Model Training

Dataset split into train (80%) and test (20%)

Trained RandomForestRegressor with 100 estimators

Feature scaling applied to numeric columns; categorical features encoded

🔹 Evaluation Metrics

RMSE: 0.0132

R² Score: 0.9894

MAE: 0.0101

MAPE: 4.2%

🔹 Visualization

Scatter plot of Actual vs Predicted Leakage_Flag

Feature importance plot showing key predictors: Pressure, Flow_Rate, RPM, and Vibration

🔹 Model Deployment

Model saved using joblib as rf_leakage_model.pkl

Loading model and making predictions on new data:

import joblib
loaded_model = joblib.load('rf_leakage_model.pkl')
new_predictions = loaded_model.predict(new_data)


Ready for integration into dashboards or web apps (e.g., Streamlit)

📂 Repository Contents

raw_dataset.csv → Original Kaggle dataset

cleaned_dataset.csv → Preprocessed dataset for ML

Week1_EDA.ipynb → Notebook with Week 1 preprocessing and EDA

Week2_Model.ipynb → Notebook with Week 2 regression model, evaluation, and deployment

rf_leakage_model.pkl → Saved Random Forest model

README.md → Project overview and weekly milestones

📅 Weekly Timeline
Week	Focus	Status
1	Data preprocessing + EDA	✅ Completed
2	Feature engineering + ML model building + evaluation + deployment	✅ Completed
3	Model optimization + Streamlit deployment	Pending
4	Final report + GitHub documentation	Pending

💡 Project Status:

Week 1: Dataset prepared and insights gathered

Week 2: Regression model trained, evaluated, and deployed

Overall Progress: 60%

Ready to move to Week 3 for model optimization and dashboard deployment
