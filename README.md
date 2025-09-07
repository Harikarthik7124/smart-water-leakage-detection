💧 Smart Water Leakage Detection

Sustainable Water Resource Management using AI/ML

Project Overview

This project leverages AI/ML techniques to detect water leakages using pipeline sensor data, aiming to optimize water usage and support sustainable urban water management.

🌱 Week 1 Milestone – Data Preprocessing & EDA (30% Progress)
🔹 Dataset Overview

Source: Smart Water Leak Detection Dataset – Kaggle

Key Features: Flow_Rate, Pressure, Temperature, Vibration, RPM, Operational_Hours

Location Info: Zone, Block, Pipe, Location_Code, Latitude, Longitude

Target Variable: Leakage_Flag (continuous numeric for regression)

🔹 Preprocessing Steps

Filled missing values in sensor readings

Encoded categorical variables (Zone, Block, Pipe, Location_Code)

Scaled numeric columns for uniformity

Saved as cleaned_dataset.csv

🔹 Exploratory Data Analysis (EDA)

Distribution Plots: Flow_Rate & Pressure




Correlation Heatmap:


Boxplots: Detect outliers


Leakage Analysis: Pairplots & grouped averages


Insights:

Flow and Pressure are strong indicators of leakage events

Leakage events cluster around abnormal flow and pressure values

📌 Week 2 Milestone – ML Model Development & Evaluation (60% Progress)
🔹 Model Choice & Justification

RandomForestRegressor handles non-linear relationships, works with mixed feature types, and provides feature importance.

🔹 Model Training & Evaluation

Split data: 80% train, 20% test

Trained RandomForestRegressor with 100 estimators

Metrics:

RMSE: 0.0132

R² Score: 0.9894

MAE: 0.0101

MAPE: 4.2%

Actual vs Predicted Plot:


Feature Importance:


🔹 Deployment

Saved model: rf_leakage_model.pkl

Load & predict:

import joblib
loaded_model = joblib.load('rf_leakage_model.pkl')
new_predictions = loaded_model.predict(new_data)

📂 Repository Structure

raw_dataset.csv → Original dataset

cleaned_dataset.csv → Preprocessed dataset

Week1_EDA.ipynb → Notebook with Week 1 preprocessing & EDA

Week2_Model.ipynb → Notebook with Week 2 regression model, evaluation & deployment

rf_leakage_model.pkl → Saved Random Forest model

README.md → Project description and weekly milestones

📅 Weekly Timeline
Week	Focus	Status
1	Data preprocessing + EDA	✅ Completed
2	Feature engineering + ML model + evaluation + deployment	✅ Completed
3	Model optimization + Streamlit deployment	Pending
4	Final report + GitHub documentation	Pending

Overall Project Progress: 60%

💡 Next Steps (Week 3):

Optimize ML models for better accuracy

Deploy interactive dashboard (Streamlit)

Prepare final GitHub documentation & presentation
