# 🚆MTA NYCT Safety Data: Beginning 2019 - Machine Learning Project (EDA Phase)

This repository contains a complete **Exploratory Data Analysis (EDA)** project focused on analyzing public transport safety metrics (Bus and Subway) collected over time. The aim is to uncover trends, distributions, and anomalies that can inform future predictive modeling or policy decisions.

---

## ✨ Project Overview

The primary objective is to understand key safety indicators across subway and bus services in a major metropolitan area. The project focuses on:

- Analyzing trends in incidents like **collisions**, **fires**, and **accidents**
- Identifying outliers and inconsistencies
- Comparing performance metrics between departments
- Preparing the dataset for downstream machine learning applications

---

## 📊 Dataset Description

**Domain**: Transportation / Safety Analytics  
**Source**: MTA (Metropolitan Transit Authority) Dataset  
**Format**: Tabular (CSV)  
**Attributes Include**:
- `Bus Collision Per Million Miles`
- `Subway Fires`
- `Subway Customer Accidents`
- `Vision Zero Training Count`
- `Friction Pad Installation`
- And many more operational and incident-related metrics

---

## 🔍 Exploratory Data Analysis (EDA)

### ✅ Step 1: Data Overview & Inspection

- Loaded dataset using Pandas
- Inspected data types, nulls, and basic stats
- Dataset contained monthly counts of various safety metrics for Bus and Subway departments

**Observation**:
- Data fairly balanced across both departments
- No extreme missing value problems

---

### ✅ Step 2: Metric Distribution Analysis

- Created **box plots** for each safety metric to examine spread and skewness  
- Used **log scale** due to high variation across metrics  

<img src="C:\Users\RAJ LANDE\OneDrive\Desktop\download4.png" width="800"/>

**Observation**:
- Metrics like `Bus Collisions` have low variance
- Metrics like `Friction Pad Installation` and `Continuous Welded Rail` show high outlier count and wide spread

---

### ✅ Step 3: Department-wise Metric Count

- Compared number of records between Subway and Bus departments

**Observation**:
- Subway slightly dominates in total metric count
- Ensures fairly balanced data for future modeling

---

### ✅ Step 4: Outlier Detection

- Identified outliers using boxplots and IQR technique  
- Focused on metrics like:
  - `Subway Fires`
  - `Customer Accidents`
  - `Audible Pedestrian Turn Warning`

**Insight**:
- Some features contain operational anomalies worth further investigation

---

### ✅ Step 5: Correlation & Redundancy

- Planned (but not yet implemented) correlation analysis for dimensionality reduction
- Initial observation: low correlation between many operational metrics

---

## 📈 Sample Graphs & Visuals

- 📦 Boxplot (log-scale) for metric comparison  
- 📊 Bar chart comparing number of entries per department  
- 📉 Line plots for metric trend over time *(to be added in next phase)*

---

## 🛠️ Technologies Used

- Python 3.x
- Jupyter Notebook
- Pandas, NumPy
- Seaborn, Matplotlib
- Plotly (optional)

---
