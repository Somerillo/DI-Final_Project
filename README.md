# **"Time Series Analysis of Pittsburgh Temperature, Energy Consumption, and Flu Contagion (2013–2015)"**

---

### **Objective:**  
To identify and explore temporal patterns, correlations, and potential causal relationships between temperature, energy consumption, and flu contagion in Pittsburgh during 2013–2015.

---
### **Key Files:**
   - dashboard_lpm.twbx
   - sources.txt
   - timeseries_EDa.ipynb
   - ARIMA_predictions.ipynb
   - forecast_with_XGBoost.ipynb
---

### **Key Datasets (sources.txt):**  
1. **USA Weather Dataset (2013–2015):**  
   - Temporal granularity: Hourly.
   - Variable of interest: Temperature. 

2. **PJM Historic Energy Consumption:**  
   - Temporal granularity: Hourly.
   - Scope: Energy usage data for Pennsylvania and Illinois.  
   - Key providers: Pennsylvania (Duquesne Light), Illinois (ComEd).  

3. **Flu Contagion Dataset by State (2013–2015):**  
   - Temporal granularity: Weekly  
   - Variables: Influenza-like illness (ILI) cases, city-level aggregation.  

---

### **Tools and Technologies:**  
- **Python (Jupyter Notebook):** Primary analysis tool for cleaning, preprocessing, statistical modeling, and visualization.  
- **Tableau:** For interactive and detailed data visualizations and dashboards.

---

### **Project Structure:**  
#### **1. Data Ingestion and Preparation (time_series_EDA.ipynb)**  
- **Goal:** Load, clean, and integrate datasets.  
- **Subtasks:**  
  - Import datasets into the environment.  
  - Handle missing or inconsistent data.  
  - Transform datasets to ensure compatible temporal granularity. 

#### **2. Exploratory Data Analysis (time_series_EDA.ipynb)**  
- **Goal:** Understand the datasets and derive preliminary insights.  
- **Subtasks:**  
  - Univariate analysis for each dataset: trends, seasonality, anomalies.  
  - Bivariate and multivariate analysis to explore relationships (e.g., temperature vs. energy consumption, flu cases vs. weather).
  - Analyze seasonality, trends, and residuals for each dataset.  
  - Conduct correlation analysis across datasets (e.g., ILI activity level vs. temperature). 

#### **3. Machine Learning Modeling (ARIMA_predictions.ipynb and forecast_with_XGBoost.ipynb)**  
- **Goal:** Model temporal patterns and assess interdependencies.  
- **Subtasks:**  
  - Apply modeling techniques:  
    - **Univariate Models:** XGBoost and ARIMA for temperature dataset.  
    - **Multivariate Models:** XGBoost for electric consumption and ILI activity dependency with temperature.  

#### **4. Data Visualization and Dashboarding (dashboard_lpm.twbx)**  
- **Goal:** Communicate findings effectively through visuals.  
- **Subtasks:**  
  - Comparative time series plots for weather, energy, and flu contagion trends.
