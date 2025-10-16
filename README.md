#  GlucoLog: Self Data Analysis Study  
### Exploring the Quantitative Relationship Between Lifestyle and Glucose Behavior  

---

##  Overview  
**GlucoLog** is a personal data research study examining how lifestyle factors — including exercise, nutrition, insulin dosing, and sleep — influence blood glucose stability and variability.  

The project leverages **Dexcom G6 continuous glucose data**, manually logged lifestyle variables, and modern data tools (**Google Sheets, SQL, and Python**) to uncover trends, correlations, and actionable insights about personal glucose management.  

This project combines **self-tracking** with **data science methods** to transform raw numbers into meaningful understanding — a step toward data-driven personal health analytics.

---

##  Project Goal  
To explore how daily habits impact glucose control through a structured, data-driven analysis — turning 10 days of personal glucose and lifestyle data into quantifiable insights on stability, insulin response, and behavioral patterns.

---

##  Research Questions  
1. How does time of day affect average blood glucose levels and variability?  
2. How does going to the gym impact glucose before, during, and after workouts?  
3. How do carb and protein intake influence post-meal glucose response?  
4. How accurate and effective are my insulin doses compared to predicted results (based on I:C and correction factor)?  
5. How does sleep duration affect fasting glucose and overall daily stability?  
6. Which factor (carbs, protein, gym, insulin, sleep) has the strongest correlation with glucose variability?

---

##  Study Design  

This study spans approximately **10 consecutive days** of personal data collection.  
Daily data will be logged in **Google Sheets**, exported as structured CSV/Excel files, and imported into a **SQL database** for organization and analysis.  

Afterward, the cleaned dataset will be analyzed using **Python (Pandas, Matplotlib, Seaborn)** to generate statistical insights and visualizations.

---

##  Data Structure  

| Tab / Table | Purpose | Key Columns |
|--------------|----------|--------------|
| **Raw Data** | Continuous or manually logged glucose readings | Date, Time, Glucose (mg/dL), Trend, Notes |
| **Lifestyle & Insulin Log** | Tracks meals, insulin shots, gym activity, and sleep | Date, Meal, Carbs, Protein, Bolus Units, Bolus Time, Correction Units, Correction Time, Basal Units, Basal Time, Gym Duration, Sleep Hours |
| **Calculated Metrics** | Summarizes daily stats for analysis | Date, Avg Glucose, Max, Min, SD, Total Carbs, Total Insulin, Gym Duration, Sleep |
| **Reference Settings** | Stores constants and baseline assumptions | I:C Ratio, Correction Factor, Basal Type, Basal Time, Study Duration |

### Database Equivalent (SQL)
When imported into SQL (SQLite):
- **Table 1:** `raw_data`  
- **Table 2:** `lifestyle_log`  
- **Table 3:** `metrics_summary`  
- **Table 4:** `reference_settings`  

Each table will be joinable by the `Date` field for queries and correlations.

---

##  Data Processing Steps  

1. Collect and log Dexcom glucose readings (every 5 minutes or hourly).  
2. Record insulin doses, meals, and sleep manually in Google Sheets.  
3. Export all data to `.csv` or `.xlsx` for structured storage.  
4. Import datasets into a local **SQLite database** for SQL querying.  
5. Clean timestamps, remove duplicates, and merge related tables.  
6. Compute daily averages, highs/lows, and variability (SD).  
7. Compare predicted vs. actual correction responses.  
8. Analyze correlations between glucose and lifestyle factors.

---

##  Analysis Tools  

| Tool | Purpose |
|------|----------|
| **Google Sheets** | Data entry, logging, and basic formula summaries |
| **SQLite (SQL)** | Structured data storage and querying |
| **Python** | Statistical analysis and visualization |
| **Libraries Used:** | Pandas, Matplotlib, Seaborn, sqlite3 |
| **Visualizations:** | Time-series glucose trends, scatter plots, boxplots, correlation heatmaps |

---

##  Repository Structure  

GlucoLog-Self-Data-Analysis-Study/
├── data/ → CSV/Excel files and SQL database
├── notebooks/ → Python analysis notebooks
├── images/ → Graphs and visual outputs
├── requirements.txt → Python dependencies
└── README.md → Documentation (this file)

---

##  Reflection & Insights  

This study aims to use personal glucose data to identify measurable lifestyle patterns, evaluate insulin dosing accuracy, and demonstrate how **data analysis, SQL, and visualization** can translate health data into knowledge.  

> “Turning personal data into personal insight.”  

---

##  Project Progress Tracker  

- [x] **Phase 1: ASK** — Defined research questions ✅  
- [x] **Phase 2: PREPARE** — Set up Google Sheets structure and GitHub repo ✅  
- [ ] **Phase 3: PROCESS** — Begin 10-day glucose data logging  
- [ ] **Phase 4: ANALYZE** — Import data into SQL and Python for visualization  
- [ ] **Phase 5: SHARE** — Upload visuals and analysis notebooks  
- [ ] **Phase 6: ACT** — Reflect and summarize final insights  

---

###  Next Steps
1. Build the 4-tab **Google Sheet** for data logging.  
2. Log data consistently for 10 days.  
3. Export all data to `.csv` for **SQL import** and Python analysis.  
4. Create SQL scripts and Python notebooks for trend exploration.  
5. Publish insights and visualizations in this GitHub repository.  

---

###  Keywords:
`Data Analysis` • `Python` • `SQL` • `Google Sheets` • `Data Visualization` • `Health Analytics` • `Research Project`


