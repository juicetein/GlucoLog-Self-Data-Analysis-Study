# GlucoLog: Self Data Analysis Study

###  Overview
**GlucoLog** is a personal research project exploring how lifestyle factors such as exercise, nutrition, insulin dosing, and sleep influence blood glucose stability and variability.  
The study uses **Dexcom G6 continuous glucose data**, analyzed with **Excel and Python**, to uncover trends, correlations, and actionable insights about daily glucose control.

---

##  Project Goal
To explore how daily habits impact glucose patterns through quantitative self-tracking and data analysis — transforming raw sensor data into health insights.

---

## MAIN Research Questions
1. How does time of day affect average blood glucose levels and variability?  
2. How does going to the gym impact glucose before, during, and after workouts?  
3. How do carb and protein intake influence post-meal glucose response?  
4. How accurate and effective are my insulin doses compared to predicted results?  
5. How does sleep duration affect fasting glucose and daily stability?  
6. Which factor (carbs, protein, gym, insulin, sleep) has the strongest correlation with glucose variability?

---

##  Data Structure

| Sheet | Purpose | Key Columns |
|--------|----------|-------------|
| Sheet 1: **Raw Dexcom Data** | Continuous glucose readings | Date, Time, Glucose, Trend, Notes |
| Sheet 2: **Lifestyle Log** | Daily manual tracking | Date, Gym?, Gym Duration, Gym Start, Carbs, Protein, Insulin, Sleep Hours, Stress, Notes |
| Sheet 3: **Calculated Metrics** | Combined daily summaries | Date, Avg Glucose, Min, Max, SD, Gym?, Carbs, Protein, Insulin, Sleep |
| Sheet 4: **Reference / Settings** | Constants & documentation | I:C Ratio, Correction Factor, Target Range, Notes on formulas |

---

##  Data Processing Steps
- Clean timestamps and remove duplicates  
- Merge Dexcom CSV with manual logs  
- Compute daily averages, highs/lows, and variability  
- Compare predicted vs. actual correction responses  
- Correlate glucose patterns with lifestyle variables  

---

##  Analysis Tools
- **Excel:** Initial logging, summary statistics  
- **Python:** Pandas, Matplotlib, Seaborn  
- **Visualizations:**  
  - Time-series glucose trends  
  - Scatter plots for carb vs. spike size  
  - Boxplots for gym vs. rest days  
  - Correlation heatmap  

---

##  Sharing & Results
The repository includes:  
/data/ → Excel + CSV files
/notebooks/ → Python analysis scripts
/images/ → Graphs + Visualizations
README.md → Research plan, findings, insights

---

##  Reflection & Insights
This study aims to use my own personal glucose data to identify measurable patterns, improve glucose management, and demonstrate how data science methods can apply to personal health analytics.

> “Turning personal data into personal insight.”  

---

