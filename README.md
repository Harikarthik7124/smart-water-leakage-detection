# smart-water-leakage-detection-
# 💧 Sustainable Water Resource Management using AI/ML  
### Project: Smart Water Leakage Detection  

## Week 1 Milestone (30%)  
“Week 1 milestone for the Sustainable Water Resource Management project – includes dataset exploration, initial data preprocessing, and preliminary analysis for building sustainable leakage detection insights.”  

🌱 **SMART WATER LEAKAGE DETECTION USING MACHINE LEARNING ALGORITHMS**  
This project focuses on analyzing pipeline sensor data to detect leakages and optimize water usage, supporting **sustainable urban water management**.  

---

## 📌 Week 1 Progress (30%)  
✅ In this week, we focused on initial **data preprocessing** and **exploratory data analysis (EDA)**.  

---

### 🔹 Dataset Description  
- **Source**: [Smart Water Leak Detection Dataset – Kaggle](https://www.kaggle.com/datasets/talha97s/smart-water-leak-detection-dataset)  
- **Key Columns**:  
  - Flow_Rate, Pressure, Temperature, Vibration, RPM, Operational_Hours  
  - Zone, Block, Pipe, Location_Code, Latitude, Longitude  
  - Leakage_Flag (0 = No Leak, 1 = Leak)  

---

### 🔹 Data Preprocessing  
- Removed missing values (handled NaN in Flow_Rate, Pressure, etc.).  
- Encoded categorical variables (Zone, Block, Pipe).  
- Applied scaling to numerical columns for consistency.  
- Saved the cleaned dataset as: **`cleaned_dataset.csv`**  

---

### 🔹 Exploratory Data Analysis (EDA)  
- Distribution plots for **Flow_Rate** and **Pressure**  
- Correlation heatmap of numerical features  
- Outlier detection using boxplots  
- Leakage distribution (imbalanced dataset: leaks are less frequent)  
- Pairplot of **Flow vs Pressure vs Leakage_Flag**  
- Grouped averages → Leakage points show distinct pressure & flow behavior  

📌 **Insights:**  
- Flow and Pressure are strong indicators of leakage.  
- Leakage events cluster around abnormal flow/pressure patterns.  
- Dataset is now clean and ready for ML feature engineering.  

---

## 📂 Files in Repository  
- `raw_dataset.csv` → Original dataset (Kaggle)  
- `cleaned_dataset.csv` → Cleaned dataset after preprocessing  
- `Week1_EDA.ipynb` → Notebook with preprocessing + EDA  
- `README.md` → Project description and weekly progress  

---

## 🚀 Next Steps (Week 2)  
- Feature engineering (derive new features like pressure-flow ratio)  
- Build initial ML pipeline for **leakage prediction**  
- Train and evaluate baseline models (Logistic Regression, Random Forest)  

---

## 📅 Weekly Plan  
- **Week 1** → Data preprocessing + EDA ✅  
- **Week 2** → Feature engineering + ML model building  
- **Week 3** → Model optimization + Streamlit deployment  
- **Week 4** → Final report + GitHub documentation  

---

💡 This is the **Week 1 milestone** — showing **30% project progress**.  

## 📂 Repository Structure  
