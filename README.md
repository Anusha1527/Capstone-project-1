# 🏭 Manufacturing Equipment Output Prediction  
### 📊 Linear Regression for Production Optimization  

---

## 🚀 Project Overview  

This project builds a **Linear Regression model** to predict the **hourly production output** of injection molding machines based on operational parameters such as temperature, pressure, cycle time, and maintenance conditions.

The goal is to help manufacturing teams:

- ⚙ Optimize machine settings  
- 📈 Increase production efficiency  
- 🔧 Identify underperforming machines  
- 💰 Reduce operational costs  

---

## 🎯 Problem Statement  

Manufacturing companies operate injection molding machines to produce plastic components.  

Production output depends on multiple machine parameters such as:

- Injection Temperature  
- Injection Pressure  
- Cycle Time  
- Cooling Time  
- Material Properties  
- Machine Age  
- Operator Experience  

This project predicts:

> 🏭 **Parts Produced Per Hour**

Using a supervised machine learning approach.

---

## 📁 Dataset Information  

A **synthetic manufacturing dataset** (6000+ records) was generated with realistic industrial relationships.

### 🔹 Features

| Feature | Description | Range |
|----------|-------------|--------|
| Injection_Temperature | Molten plastic temperature (°C) | 180–250 |
| Injection_Pressure | Hydraulic pressure (bar) | 80–150 |
| Cycle_Time | Time per production cycle (sec) | 15–45 |
| Cooling_Time | Cooling duration (sec) | 8–20 |
| Material_Viscosity | Flow resistance (Pa·s) | 100–400 |
| Ambient_Temperature | Factory temperature (°C) | 18–28 |
| Machine_Age | Machine age (years) | 1–15 |
| Operator_Experience | Experience (months) | 1–120 |
| Maintenance_Hours | Hours since last maintenance | 0–200 |

### 🎯 Target Variable
`Parts_per_Hour`

---

## 🛠️ Tech Stack  

- 🐍 Python  
- 📊 Pandas  
- 🔢 NumPy  
- 📉 Matplotlib  
- 🎨 Seaborn  
- 🤖 Scikit-Learn  
- 💾 Pickle (Model Serialization)  

---

## 🔍 Project Workflow  

### 1️⃣ Data Generation  
- Created synthetic dataset with realistic industrial relationships  
- Added controlled noise for real-world behavior  

### 2️⃣ Exploratory Data Analysis  
- Histograms  
- Correlation heatmap  
- Scatter plots  
- Target distribution analysis  

### 3️⃣ Data Preprocessing  
- Outlier removal (IQR method)  
- Feature engineering (Efficiency ratio)  
- Train-test split  
- Feature scaling  

### 4️⃣ Model Building  
- Linear Regression  
- Reproducible results using random state  

### 5️⃣ Model Evaluation  

Metrics used:

- R² Score  
- Mean Squared Error (MSE)  
- Root Mean Squared Error (RMSE)  
- Mean Absolute Error (MAE)  

✔ Achieved **R² > 0.90** on test data  

---

## 📈 Model Performance  

| Metric | Training | Testing |
|--------|----------|----------|
| R² Score | > 0.90 | > 0.90 |
| RMSE | Low | Low |
| MAE | Low | Low |

The model satisfies the success criteria of:

> ✅ R² > 0.75  

---

## 🧠 Key Manufacturing Insights  

- 🔴 Higher Cycle Time reduces production output  
- 🟢 Higher Injection Pressure increases output  
- 🔵 Operator Experience improves efficiency  
- 🟠 Machine Age negatively impacts productivity  
- 🟣 Regular maintenance improves performance  

---

## 🏭 Production Optimization Recommendations  

- Reduce Cycle Time within safe operating limits  
- Maintain Injection Pressure between 100–130 bar  
- Schedule maintenance every 100 hours  
- Replace machines older than 10 years  
- Invest in operator training programs  

---

## 💾 Model Deployment Ready  

The trained model and scaler are saved using:

```python
pickle.dump(model, open("manufacturing_model.pkl", "wb"))
pickle.dump(scaler, open("scaler.pkl", "wb"))
```
```
📦 Manufacturing-Output-Prediction
 ┣ 📜 capstone_project.ipynb
 ┣ 📜 manufacturing_data.csv
 ┣ 📜 manufacturing_model.pkl
 ┣ 📜 scaler.pkl
 ┣ 📜 README.md
```
