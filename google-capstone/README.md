# Bellabeat Case Study
*A Google Data Analytics Capstone Project*

## Project Overview
This project explores how **Bellabeat**, a women's wellness technology company, can utilize smart device data to understand consumer behavior and enhance its marketing strategies.

**Business Task:**  
How can Bellabeat utilize smart device data to gain insights into user activity, sleep patterns, and engagement to improve its marketing and product decisions?

---

## Dataset
**Name:** Fitbit Fitness Tracker Data  
**Source:** [Kaggle – FitBit Fitness Tracker Data](https://www.kaggle.com/datasets/arashnic/fitbit)  
**Time Period:** March–May 2016 (~62 days)  
**Participants:** 30–33 unique Fitbit users  

---

## Limitations
- Small dataset (~33 users) limits generalizability  
- Short tracking duration (62 days)  
- Data is **self-reported** and may include inaccuracies 
- The data is from a secondary source (Fitbit), not Bella Beat, so it’s not fully representative.
- Data is several years old (2016)

---

## Tools Used
- **Excel:** Data cleaning, merging, calculations  
- **Tableau:** Visualization and dashboard creation

**Key Steps:**  
- Data cleaning in **Excel**  
- Exploratory analysis and aggregation  
- Visualization and dashboard design in **Tableau**

---

## Data Cleaning & Aggregation (Excel)
1. **Inspected data for missing values and duplicates**  
   - Removed duplicate user records across multiple CSV files.  
   - Handled null or zero values in *sleep* and *weight* datasets.

2. **Standardized date and time formats**  
   - Converted text timestamps to proper *datetime* format for consistency.  
   - Extracted *date*, *weekday*, and *hour* fields for time-based analysis.

3. **Merged datasets**  
   - Combined activity, sleep, and calories tables using *user ID* and *date* as keys.  
   - Created a unified dataset to enable user-level summaries.

4. **Created calculated fields**  
   - **Step Goal %:** `(Total Steps / 10,000) * 100`  
   - **Sleep Efficiency:** `(Minutes Asleep / Minutes in Bed) * 100`  
   - **User Category:** based on *days logged* (Light, Moderate, Heavy).  
   - **Sleep Category:** based on average sleep hours (Short <7h, Normal 7–9h, Long >9h).  

5. **Validated and summarized data**  
   - Cross-checked counts and averages to ensure consistency across all datasets.

---

## Key Insights
- Average daily steps: **7,519** (below the 10,000 recommended goal)  
- Average sleep: **2.9 hours** (below the 7-hour minimum recommendation)  
- Only **12%** of users met both sleep and activity targets  
- **87%** of users logged data consistently (heavy users)

---

## Recommendations
1. **Personalized Goals:** Enable adaptive step and sleep targets based on user patterns.  
2. **Sleep Improvement Features:** Introduce sleep tips and insights within the app.  
3. **App Engagement Incentives:** Encourage regular logging with badges, streak rewards, or reminders.  
4. **Targeted Notifications:** Nudge users on low-activity or low-sleep days.

---

## Visualizations
- [Executive Dashboard](./Visualizations/Executive_overview.png)

View interactive dashboard: [Tableau Link](https://public.tableau.com/views/ExecutiveOverviewActivitySleepEngagement/EXECUTIVEOVERVIEW?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
 
- [Activity Deep Dive](./Visualizations/Activity_deep_dive.png)

View interactive dashboard: [Tableau Link](https://public.tableau.com/views/ActivityDeepDive/ACTIVITYDEEPDIVE?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

- [Sleep Analysis](./Visualizations/Sleep_deep_dive.png)

View interactive dashboard: [Tableau Link](https://public.tableau.com/views/SleepDeepDive/SLEEPDEEPDIVE?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

- [`Engagement Correlation`](./Visualizations/Engagements_and_correlations.png)

View interactive dashboard: [Tableau Link](https://public.tableau.com/views/EngagementsCorrelations/ENGAGEMENTSCORRELATIONS?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

---

## Files Used
- [`merged_cleaned_dataset.xlsx`](./Sheets/cleaned_merged_dataset.xlsx) – Final dataset used for analysis and visualization (cleaned, merged, with calculated metrics).  
- [`user_summary.xlsx`](./Sheets/User_Summary.xlsx) – Aggregated summary of user-level statistics (daily steps, sleep, activity patterns).  

---

## Author
**Shulammite Okafor**

[LinkedIn](https://www.linkedin.com/in/shulammiteokafor) | [Email](mailto:okaforshula@gmail.com)
