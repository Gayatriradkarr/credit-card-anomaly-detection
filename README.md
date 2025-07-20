# Credit Card Anomaly Detection Using Behavioral Rules and Statistical Profiling

This project analyzes anonymized credit card transaction data to identify unusual activity using only rule-based methods and statistical profiling — no machine learning. The focus is on understanding transaction patterns through user behavior, time-based analysis, and threshold logic that mirrors real-world fraud detection systems.

---

## Project Objectives

- Detect anomalies in transactions based on behavior, not models
- Flag potential fraud using business rules and visual analysis
- Create a clean, readable process for non-technical stakeholders to follow

---

## Techniques Used

1. **Exploratory Data Analysis (EDA)**
   - Amount distribution, time-of-day analysis
   - Transaction frequency per user

2. **Rule-Based Anomaly Detection**
   - Flagging transactions above the 99th percentile
   - Identifying multiple transactions in short time frames
   - Highlighting transactions during off-hours (e.g., 2–4 AM)

3. **Statistical Profiling**
   - Z-score detection to find spending spikes
   - User-level behavior baseline comparison

4. **Time-Based Pattern Recognition**
   - Daily and hourly spending heatmaps
   - Inter-transaction time gap analysis

---

## Tools Used

- Python (Pandas, NumPy)
- Jupyter Notebook
- Matplotlib, Seaborn for visualizations
- Optional: Excel/CSV output for flagged transactions

---

## Folder Structure
notebooks/   – Jupyter notebooks containing rule logic and analysis  
data/        – Credit card transaction dataset (CSV or Excel)  
dashboards/  – Dashboard files (e.g., Streamlit, Excel, or Tableau if extended)  
visuals/     – Screenshots of plots, charts, and dashboard views  
README.md    – This project overview and documentation  



