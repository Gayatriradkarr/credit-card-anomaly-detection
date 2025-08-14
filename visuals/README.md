Transaction Amount Distribution (visuals/Transaction_Amount_Distribution.png):
Description: A histogram with a KDE curve showing the distribution of Transaction_Amount, with a red dashed line at the 99th percentile to highlight high-amount transactions.
Purpose: Identifies outliers (e.g., transactions >$2000 flagged as High_Amount).
Insight: Confirms high-amount anomalies (e.g., T008: $2500).
Hourly Spending Heatmap (visuals/Hourly_Spending_Heatmap.png):
Description: A heatmap showing total Transaction_Amount by day of week and hour, using a YlOrRd color scale. High values indicate unusual spending patterns.
Purpose: Detects off-hour activity (e.g., 2–4 AM spikes for U002, U004).
Insight: Highlights potential fraud in early morning hours, aligning with your off-hour rule.
Flagged Anomalies Scatter Plot (visuals/Flagged_Anomalies.png):
Description: A scatter plot with Transaction_Date (x-axis), Transaction_Amount (y-axis), colored and styled by Rule_Flag, and sized by Z_Score_Amount.
Purpose: Visualizes flagged transactions (e.g., High_Amount, Rapid_Succession, Off_Hour) over time.
Insight: Shows clusters of anomalies, e.g., T003/T004 (rapid succession, off-hour) for U002.
