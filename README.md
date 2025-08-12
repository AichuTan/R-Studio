https://aichutan.github.io/Google-Analytics-Bellabeat/


# 📊 Bellabeat Data Analysis Case Study

**Author:** Aichu Tan  
**Live Project:** [Bellabeat Data Analysis Website](https://aichutan.github.io/Google-Analytics-Bellabeat/)

---

## 📌 Project Overview

This project is part of the Google Data Analytics Capstone. As a junior data analyst on the Bellabeat marketing analytics team, I analyzed smart device usage data to uncover trends and deliver recommendations that inform Bellabeat’s marketing strategy.

> Bellabeat is a high-tech company focusing on women’s wellness, offering products like fitness trackers, a smart water bottle, and personalized health guidance.

---

## 🧭 Business Task

**Guiding Questions:**
- What are some trends in smart device usage?
- How could these trends apply to Bellabeat customers?
- How can these trends influence Bellabeat’s marketing strategy?

---

## 📁 Data Source

- **FitBit Fitness Tracker Data**  
  Open dataset of 33 Fitbit users (CC0: Public Domain)  
  Time period: April 12 – May 12, 2016  
  [Available via Mobius / Kaggle](https://www.kaggle.com/datasets/arashnic/fitbit)

> Note: This is a small, dated dataset and may not be representative of all users.

---

## 🔧 Tools and Packages Used

- R Programming
- `tidyverse`, `lubridate`, `janitor`, `skimr`
- `ggplot2`, `dplyr`
- RMarkdown

---

## 📊 Data Cleaning & Transformation

- Converted ID columns to `character`
- Converted date columns to `Date`
- Merged `daily_activity` and `daily_sleep` datasets
- Removed duplicates using `distinct()` and `drop_na()`
- Added derived columns:
  - `Weekday`
  - Active minutes → active hours

---

## 📈 Key Insights

### 🏃 Daily Steps (33 users)
- **Average:** 7,629 steps per day → *"Somewhat Active"*
- **Most active days:** Tuesday and Saturday
- **Least active:** Sunday

### 🔥 Activity Level Breakdown
- **Sedentary (device-based):** 81.3% of daily time
- **Step-based classification (CDC definition):**
  - 27.3% Somewhat Active
  - 27.3% Low Active
  - 6.1% Highly Active
  - 24.2% Sedentary

### 😴 Sleep Duration (24 users)
- **Average Sleep:** 6.9 hours/day
- **Highest:** Sunday (7.5 hrs)
- **CDC Recommendation:** ≥7 hrs/night

### 🔁 Relationship Between Activity & Sleep
- More steps on Tuesday/Saturday → More sleep on Wednesday/Sunday
- Walking more may help improve sleep duration

### 🔄 Hourly Steps
- Activity starts ~5 AM, peaks around 6–7 PM

---

## 📊 Visualizations

- **Figure 1:** Average steps by weekday  
- **Figure 2:** Daily average calories burned  
- **Figure 3:** Daily average sleep hours  
- **Figure 4:** Activity level breakdown (Very, Fairly, Lightly, Sedentary)  
- **Figure 5:** Step-based user activity type (CDC categories)  
- **Figure 6:** Hourly total steps

---

## 📢 Recommendations for Bellabeat

1. **Encourage 7,500–10,000 daily steps**  
   Notify users to stay within this target for optimal health benefits.

2. **Promote better sleep habits**  
   Encourage walking >8,000 steps daily to improve sleep duration.

3. **Align device activity categories with CDC standards**  
   Update software to better reflect definitions of sedentary/active levels.

---

## 📚 References

- [CDC – Physical Activity Basics](https://www.cdc.gov/physical-activity-basics/about/index.html)
- [MedicineNet – Steps Per Day](https://www.medicinenet.com/how_many_steps_a_day_is_considered_active/article.htm)
