# 🏭 Manufacturing Equipment Output Prediction  
## Data Science Capstone Project  

### 📌 Project Overview

This project focuses on predicting hourly production output (number of parts produced per hour) of injection molding machines using **Linear Regression**.

The goal is to help manufacturing companies optimize machine settings, improve production efficiency, and identify underperforming equipment.

---

## 🎯 Problem Statement

Injection molding machines operate under various parameters such as temperature, pressure, cycle time, and material properties.  

This project builds a regression model that predicts:

> 🎯 **Target Variable:** Parts Produced Per Hour

Using machine operating conditions and environmental factors.

---

## 📊 Dataset Information

- 📁 Type: Synthetic Manufacturing Dataset  
- 📦 Size: 5,000+ records  
- 🎯 Target: Hourly Production Output  

### 🔢 Features

- Injection_Temperature (°C)  
- Injection_Pressure (bar)  
- Cycle_Time (seconds)  
- Cooling_Time (seconds)  
- Material_Viscosity (Pa·s)  
- Ambient_Temperature (°C)  
- Machine_Age (years)  
- Operator_Experience (months)  
- Maintenance_Hours (hours since last maintenance)

---

## 🔄 Project Workflow

### Step 1: Data Generation & Loading
- Generated synthetic manufacturing dataset
- Added realistic correlations and noise
- Saved dataset as CSV

### Step 2: Data Exploration
- Checked data types and summary statistics
- Identified missing values and outliers
- Analyzed target distribution

### Step 3: Exploratory Data Analysis (EDA)
- Histograms for variable distributions
- Correlation matrix
- Scatter plots between features and output
- Identified optimal operating ranges

### Step 4: Data Preprocessing
- Outlier handling using IQR method
- Feature engineering
- Train-test split

### Step 5: Model Building
- Built Linear Regression model
- Trained using training dataset
- Generated predictions on test dataset

### Step 6: Model Evaluation
- R² Score
- MSE
- RMSE
- MAE
- Residual analysis
- Predicted vs Actual comparison

### Step 7: Manufacturing Insights
- Identified most impactful parameters
- Interpreted regression coefficients
- Provided optimization recommendations

### Step 8: Business Recommendations
- Suggested optimal machine settings
- Recommended maintenance scheduling
- Proposed monitoring framework

### Step 9: Model Validation
- Checked regression assumptions:
  - Linearity
  - Independence
  - Homoscedasticity
  - Normality
- Assessed business impact

---

## 🚀 Deployment Pipeline (Advanced Extension)

### Step 10: Model Serialization
- Saved model using Pickle
- Saved preprocessing objects

### Step 11: FastAPI Backend
- Created REST API for predictions
- Implemented input validation with Pydantic
- Added health check endpoints

### Step 12: Docker Deployment
- Created Dockerfile
- Added docker-compose.yml
- Containerized FastAPI application

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- FastAPI
- Docker

---

## 📈 Expected Model Performance

- 🎯 R² Score > 0.75 (Test Data)
- Strong business-relevant insights
- Statistically validated model

---

## 💡 Key Learnings

- Manufacturing process analytics
- Regression modeling
- Feature engineering
- Model validation
- Business impact analysis
- API development and deployment

---

## 📂 Project Structure

```
Manufacturing-Output-Prediction/
│
├── capstone_project_1.ipynb
├── dataset.csv
└── README.md
```
---
