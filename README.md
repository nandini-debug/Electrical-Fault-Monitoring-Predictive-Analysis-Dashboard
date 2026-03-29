# ⚡ IoT-Driven Electrical Fault Monitoring & Predictive Maintenance System

## 🔹 Overview
This project is an end-to-end electrical fault monitoring and predictive maintenance system using IoT-based simulated data, Machine Learning, and Power BI dashboards.

It generates a full-year dataset, applies fault detection logic, trains a Random Forest model, and visualizes insights through interactive dashboards.

---

## 🔹 Dataset Generation
- Generated hourly data for the full year (2025)
- Simulates real-world IoT sensor readings:
  - Voltage
  - Current
  - Temperature
  - Vibration
  - Power (kW)

- Added time-based features:
  - Date, Month, Year
  - Month Name and Month-Year format

---

## 🔹 Fault Classification Logic
Faults are categorized into three levels:

- **Normal (0)** → Safe operating conditions  
- **Warning (1)** → High current or vibration  
- **Critical (2)** → Low voltage or high temperature  

---

## 🔹 Machine Learning Model
- Algorithm: Random Forest Classifier  
- Trained on sensor data to predict fault conditions  
- Parameters:
  - n_estimators = 120  
  - max_depth = 10  

- Dataset split:
  - 80% Training  
  - 20% Testing  

---

## 🔹 Predictions
- Model predicts fault category for each record  
- Output includes:
  - Actual Fault
  - Predicted Fault
  - Fault Status (Normal / Warning / Critical)

---

## 🔹 Dashboards Included

### 1. Electrical Fault Monitoring Dashboard
- Real-time system health overview

### 2. Fault Monitoring & Trend Analysis
- Monthly and historical trends

### 3. Predictive Fault Dashboard
- ML-based fault predictions

### 4. Advanced Predictive Dashboard
- KPIs and comparative insights

### 5. Future Scope & IoT Maintenance
- IoT-based automation concepts

---

## 🔹 Tools & Technologies
- Python (Pandas, NumPy, Scikit-learn)
- Machine Learning (Random Forest)
- Power BI (Visualization)
- IoT Data Simulation

---

## 🔹 Key Features
- Synthetic IoT dataset generation
- Fault classification logic
- Predictive modeling
- Trend analysis dashboards
- Interactive visualizations

---

## 🔹 Output File
- `electrical_fault_rf_2025.csv`
  - Contains full dataset with predictions and status labels

---

## 🔹 Conclusion
This project demonstrates how IoT data, Machine Learning, and data visualization can be integrated to build a predictive maintenance system that reduces failures and improves efficiency.

IoT-Electrical-Fault-Prediction
│
├── data/
│   └── electrical_fault_rf_2025.csv
│
├── notebook/
│   └── fault_prediction.ipynb
│
├── dashboard/
│   └── electrical_dashboard.pbix
│
├── images/
│   └── dashboard_screenshot.png
│
├── src/
│   └── data_generation_model.py
│
├── README.md
└── requirements.txt
pandas
numpy
scikit-learn
