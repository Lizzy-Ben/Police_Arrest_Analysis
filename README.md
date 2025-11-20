# Police Arrest Data Analysis
- A Full Exploratory Data Analysis Using Python
## Project Overview
- This project explores a real-world police arrest dataset to identify patterns in arrest frequency across demographic groups, locations, time periods and police units.
It applies end-to-end data analysis techniques — from cleaning and transformation to visualization and insights using Python and Plotly Express.
- The goal is to understand when, where, and to whom arrests occur most frequently and to develop insights that can support operational planning and public safety decision-making.
## Objectives
- Examine arrest patterns across gender, ethnicity, and race
- Identify the bureau and division with the highest arrests
- Analyze arrests by time of day, month, year, and Month-Year
- Determine the specific Month-Year with the highest and lowest arrest counts
- Create interactive visualizations using Plotly Express
- Apply data cleaning, preprocessing, and exploratory data analysis (EDA)
## Data Source
- The dataset used is an Excel file.
## Tools Used
- Python
- Jupiter Notebook
## Exploratory Data Analysis
# Police Arrest Data Analysis
This project explores a police arrest dataset to uncover patterns in arrests across demographics (gender, age, ethnicity) and temporal trends (time of day). Using Python and Plotly Express, the analysis visualizes key trends and derives actionable insights.
## Question 1 — Total Number of Suspects

To establish the scale of the dataset, the total number of unique suspects was computed.
**Analysis:**
➡️ **23,510 suspects**

This provides a solid foundation for downstream demographic, temporal, and departmental breakdowns. Understanding the dataset size ensures that subsequent insights—such as gender distribution, arrest times, and bureau patterns—are interpreted within the correct population context.

---

## Question 2 — Gender With the Highest Arrests

The gender distribution of arrests shows a significant imbalance between male and female suspects.

**Analysis:**

* Male suspects: ~18,000 arrests
* Female suspects: ~5,000 arrests

**Insight:**
Male suspects are arrested more than three times as often as female suspects, suggesting strong gender-related patterns in criminal activity, enforcement outcomes, or reporting practices. This sets the stage for deeper demographic analysis such as age and ethnicity breakdowns.

---

## Question 3 — Age With the Highest Arrests

The age distribution of arrests reveals a clear concentration among younger adults.

**Analysis:**

* Age 18: highest number of arrests (~800+)
* Ages 19–30: consistently high arrest frequencies
* After age 30: gradual decline
* Beyond age 50: significantly fewer arrests

**Insight:**
Late teens to late twenties represent the most active arrest age range, indicating age-related behavioral or societal factors influencing arrest likelihood.

---

## Question 4 — Ethnicity With the Highest Arrests

The dataset shows disparities across ethnic groups.

**Analysis:**

* Non-Hispanic: 16,358 arrests
* Hispanic: 7,152 arrests

**Insight:**
Non-Hispanic suspects are arrested more than twice as often as Hispanic suspects, highlighting distinct ethnic trends in arrest patterns.

## Question 5 - What Time Shows the Highest Arrests.

* Midnight (00:00) records the highest arrests (417 combined, accounting for duplicates)
* Other moderately high arrest periods: Midday (12:00), Late afternoon–evening (17:00–22:00)

This suggests increased police activity or incidents around midnight, with a secondary peak in the late afternoon and evening hours.

---
## Question 6 — Month and Year With the Highest and Lowest Arrests

This analysis examines arrest trends across different months and years to identify periods with the most and fewest arrests.

**Analysis:**  
- **Highest arrests:** November 2023 — 676 arrests  
- **Lowest arrests:** July 2024 — 3 arrests  

**Insight:**  
- Arrest activity peaked in **November 2023**, possibly reflecting higher criminal activity, increased law enforcement operations, or reporting patterns.  
- Arrest activity was lowest in **July 2024**, which may indicate seasonal factors, policy changes, or other influences affecting arrest frequency.  
- Tracking month-year patterns helps identify temporal trends and can support further analysis on causes behind fluctuations in arrests.

---

## Question 7 — Breakdown of Arrests by Assigned Bureau with Respect to Race

This analysis examines how arrests are distributed across different police bureaus with respect to race.

**Analysis & Key Insights:**

- The dataset is dominated by **PSB**, which accounts for ~90–92% of all arrests (~21,000 out of ~23,367). The other three bureaus combined have only ~2,400 arrests.
- **Racial proportions vary dramatically by bureau:**  
  - FSB: White-majority (~64% White vs. 36% Black)  
  - ISB: Roughly even (53% White, 47% Black)  
  - PSB: Near 50/50 split between White and Black, small Asian share (~2.5%)  
  - MSB: Black-majority (~67% Black vs. 33% White)
- In raw numbers, PSB contributes the overwhelming majority of both White and Black arrests (~88% of White arrests and ~91% of Black arrests), which makes city-wide totals appear roughly balanced despite very different patterns in other bureaus.
- **Insight:** Any discussion of racial disparities must be **bureau-specific**; aggregating all bureaus together hides large geographic variation.

## Question 8 - Breakdown of arrest in the assigned division with respect to ethnicity?



