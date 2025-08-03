# Credit Card Anomaly Detection Using Behavioral Rules and Statistical Profiling

This project simulates a rule-based fraud detection system for credit card transactions using behavioral analytics and statistical profiling. The objective is to identify suspicious activity by examining deviations from normal user patterns — using transparent, interpretable logic.

## Project Objective

To detect anomalous transactions by:
- Profiling user behavior over time  
- Defining business logic that mimics real-world fraud detection rules  
- Providing clean, interpretable outputs for risk analysis teams  

## Methodology

### Exploratory Data Analysis (EDA)
- Assessed transaction amount distribution and frequency  
- Identified time-of-day spending trends  
- Segmented activity patterns by user  

### Rule-Based Detection
- Flagged transactions above the 99th percentile  
- Detected multiple transactions in rapid succession  
- Highlighted off-hour activity (e.g., 2 AM–4 AM), which may indicate bot or compromised card usage  

### Statistical Profiling
- Applied Z-score analysis to detect sudden spending spikes  
- Compared transactions against user-specific behavior baselines  

### Time-Based Analysis
- Built heatmaps to visualize hourly and daily spend  
- Measured inter-transaction gaps to catch abnormal activity  

## Tools Used

- Python (Pandas, NumPy) – Data processing and logic building  
- Jupyter Notebook – Stepwise documentation and reproducibility  
- Matplotlib, Seaborn – Pattern visualization and risk communication  
- Excel/CSV Export – Final flagged transactions for operational review  

## Folder Structure
notebooks/ – All analysis steps and business rules in Jupyter format
data/ – Anonymized credit card transaction dataset
dashboards/ – Dashboard files (e.g., Streamlit, Excel, or Tableau if extended)
visuals/ – Screenshots of plots, charts, and dashboard views
README.md – This project overview and documentation


