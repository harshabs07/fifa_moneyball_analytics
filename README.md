# ⚽ FIFA "Moneyball" Scouting Dashboard

An end-to-end data engineering and analytics project to identify undervalued U-23 football talent using a data-driven scouting approach.

---

# 🎯 Problem Statement

A mid-table football club has recently sold its star central midfielder to generate transfer funds. The transfer created a major gap in the squad, and the club must quickly find a replacement before the upcoming season.

However, the club faces two key constraints:

- A limited transfer budget of **€15M**
- A preference for **young players (U-23)** who can develop into future stars

Traditional scouting methods rely heavily on manual observation and subjective judgement, which can sometimes overlook undervalued talent across global leagues.

To address this problem, this project applies a **data-driven scouting approach inspired by the Moneyball philosophy**, using FIFA player data to identify midfielders who provide the best **performance-to-value ratio**.

The objective is to answer the key scouting question:

> **Which U-23 CM/CDM under €15M offers the best value and can replace the club's departing star player?**

---

# 🛠️ Tech Stack

- **Python:** Data cleaning and ETL (Extract, Transform, Load)
- **MySQL:** Relational database for structured data storage
- **Power BI:** Interactive visualization and business intelligence

---

# 📊 The Dashboard

![Main Dashboard](output.png)

---

# 💡 Key Technical Solutions

### Handling Dirty Data
Resolved duplicate player entries across multiple FIFA versions by implementing **average aggregation** for player ratings and market values.

### Automated Data Pipeline
Built a Python ETL script using **SQLAlchemy** to automatically transfer **19,000+ player records** from CSV files into a local MySQL database.

### Advanced Visualization
Designed an interactive **Value vs Performance scatter plot** in Power BI with dynamic slicers for:

- Age
- Position
- Transfer value
- Overall rating

This enables real-time scouting analysis.

---

# 🏆 Final Recommendation

Based on the data analysis, **A. Ramsey** emerged as the best replacement option.

- **Overall Rating:** 83 OVR
- **Age:** Under 23
- **Market Value:** €15M
- **Position:** CM

He provides elite performance within the club's financial constraints, making him the ideal signing based on the data-driven scouting model.
