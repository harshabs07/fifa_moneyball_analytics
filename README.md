# ⚽ ProScout U23 Analytics: The "Hidden Gem" Pipeline

## 📖 Project Overview
I built an end-to-end data pipeline to solve a specific scouting challenge: **Identify high-potential midfielders under the age of 23 with a strict budget cap of €15M.** This project demonstrates the full data lifecycle—from raw CSV extraction to a professional executive dashboard.

## 🛠️ Tech Stack
* **Python:** Used for ETL (Extract, Transform, Load) to clean the raw Kaggle dataset.
* **MySQL:** Hosted the relational database for structured querying.
* **Power BI:** Developed an interactive dashboard with advanced filtering and scatter plot visualizations.

## 📊 The Dashboard
This interactive visualization highlights the "Target Quadrant" (high overall rating, low market value).

![Main Scouting Dashboard](output.png)

## 💡 Key Insights & Data Integrity
* **Handling Historical Data:** The raw dataset contained multiple entries per player across different game versions. I implemented **Average Aggregation** to ensure ratings reflected career consistency rather than inflated sums.
* **The "Golden Quadrant":** By analyzing the scatter plot of **Value vs. Overall Rating**, I successfully identified **A. Ramsey** (the young prospect) as a top-tier target—offering an elite **83 OVR** for only **€15M**.

## 🚀 How to Run this Project
1. Run the `push_data.py` script to populate your local MySQL instance.
2. Open the `.pbix` file in Power BI Desktop.
3. Refresh the data source to link to your local database.
