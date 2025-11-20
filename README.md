## Table of Content
- [Project Overview](#project_overview)
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
<details>
  
<summary>Click here for full Exploratory Data Analysis(EDA)</summary>

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

![Arrests_by_Gender](<img width="700" height="360" alt="Arrest by Gender" src="https://github.com/user-attachments/assets/9e51a4f2-5c13-417e-9aa2-5b94ac27b571" />)

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

![Arrests_by_Age](<img width="1104" height="360" alt="Arrests by Age" src="https://github.com/user-attachments/assets/24435040-0d76-4b74-a22c-91dfc1e290ab" />)

---

## Question 4 — Ethnicity With the Highest Arrests

The dataset shows disparities across ethnic groups.

**Analysis:**

* Non-Hispanic: 16,358 arrests
* Hispanic: 7,152 arrests

**Insight:**
Non-Hispanic suspects are arrested more than twice as often as Hispanic suspects, highlighting distinct ethnic trends in arrest patterns.

![Arrests_by_Ethnicity](<img width="700" height="360" alt="Arrests by Ethnicity" src="https://github.com/user-attachments/assets/d459d470-a2c9-4079-9d85-b50fbad749da" />)

---

## Question 5 - What Time Shows the Highest Arrests.

* Midnight (00:00) records the highest arrests (417 combined, accounting for duplicates)
* Other moderately high arrest periods: Midday (12:00), Late afternoon–evening (17:00–22:00)

This suggests increased police activity or incidents around midnight, with a secondary peak in the late afternoon and evening hours.

![Arrests_by_Top_Times](<img width="1104" height="360" alt="Arrests by Top Times" src="https://github.com/user-attachments/assets/bfc89bd5-c557-461c-b55e-bb275f23af64" />)

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

![Arrests_by_Month_Year](<img width="700" height="360" alt="Arrests by Month and Year" src="https://github.com/user-attachments/assets/a8962b95-c081-4273-9d0d-3fe2e3475c65" />)

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

![Assigned_Bureau_to_Race](<img width="1104" height="360" alt="Assigned Bureau by Race" src="https://github.com/user-attachments/assets/1538e316-0c25-49d5-9a52-117a53f27365" />)

--- 

## Question 8 — Breakdown of Arrests by Assigned Division with Respect to Ethnicity

This analysis examines arrests across police divisions by Hispanic vs. Non-Hispanic individuals.

**Key Insights:**

- Overall, **31.9% of arrests involve Hispanic individuals**, but this share varies dramatically by division.  
- **4D stands out** with both the highest volume and highest proportion of Hispanic arrests (41.7%), accounting for nearly a quarter of all Hispanic arrests.  
- **GPD** is essentially 50/50 Hispanic vs. Non-Hispanic, likely reflecting a specialized city-wide unit.  
- Many patrol districts (2D, 5D) and the **Criminal Investigations Division (CID)** have very low Hispanic representation.  
- **Insight:** Hispanic arrests are highly geographically concentrated, and division-level differences dominate the overall city-wide proportion. Any claim about “disproportionate” arrests must consider these stark division-specific patterns.

![Assigned_Division_to_Ethnicity](<img width="1104" height="360" alt="Assigned Division by Ethnicity" src="https://github.com/user-attachments/assets/928d0de3-dcf1-4e90-b09b-2ae49360b6ea" />)

</details>

---

## Findings

1. **Demographic patterns:**  
   - Male suspects are arrested more than three times as often as female suspects.  
   - Arrests peak among younger adults, especially ages 18–30.  
   - Non-Hispanic individuals are arrested more than twice as often as Hispanic individuals city-wide.  

2. **Temporal trends:**  
   - Highest arrests occur around midnight (00:00) and late afternoon/evening (17:00–22:00).  
   - November 2023 had the highest monthly arrests, while July 2024 had the lowest.  

3. **Bureau and division disparities:**  
   - PSB dominates total arrests, nearly 90–92% of the dataset.  
   - Racial and ethnic proportions vary widely by bureau and division.  
   - Hispanic arrests are highly concentrated in a few divisions (4D, 3D, 5D, GPD), while specialized units (CID, SOD, PSB) remain overwhelmingly Non-Hispanic.  

## Recommendations

1. **Targeted policy review:** Focus on divisions with high arrest volume and disproportionate ethnic or age patterns to ensure equitable policing.  
2. **Temporal resource allocation:** Adjust patrol schedules around peak arrest times (midnight, late afternoon/evening) to optimize coverage and response.  
3. **Division-level monitoring:** Analyze bureaus and divisions separately rather than city-wide to identify localized disparities in arrests.  
4. **Community engagement:** Implement outreach programs in high-arrest divisions to reduce potential over-policing of specific demographic groups.  
5. **Data-driven strategy:** Use this EDA to guide further investigations into factors driving demographic disparities, seasonal patterns, and geographic concentrations.  

## Conclusion

This exploratory data analysis reveals clear demographic, temporal, and geographic patterns in arrests. Arrests are concentrated among younger males, certain divisions, and specific time periods. Ethnic and racial disparities are highly dependent on the bureau or division, emphasizing the need for localized, data-driven strategies in policing and policy-making. Careful interpretation at the division and bureau level is critical to avoid misleading city-wide generalizations. The findings provide a foundation for informed decision-making, equitable resource allocation, and targeted community interventions.


