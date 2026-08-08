# Nhs-outpatient-performance-analysis
I have analyzed 113 million NHS outpatient appointments to identify strategic opportunities for capacity expansion and efficiency improvement.And it focuses on three core questions:

1. Where is demand concentrated, and which conditions drive the highest volume?
2. How efficient is the current mix of first appointments vs follow-ups?
3. Which diagnoses are most suitable for telehealth, and what capacity could be unlocked?

## Approach
This project uses **Business Analysis** with Python for data processing 
and Power BI for visualization.

| Phase | Focus | Activities |
|-------|-------|------------|
| 1 | Data Understanding | Extracted 113M records, assessed data quality, identified gaps |
| 2 | Exploratory Analysis | Diagnosis distribution, appointment type patterns, telehealth adoption |
| 3 | Diagnostic Analysis | Follow-up ratios, priority scoring, outlier detection |
| 4 | Telehealth Scoring | Custom 0–100 suitability model (exam requirements, acuity, symptoms, monitoring) |
| 5 | Capacity Projection | Modelled impact of data quality, follow-up optimisation, and telehealth expansion |
| 6 | Visualisation | Power BI dashboard with interactive filters and KPIs |

## Key Findings

- **Data Quality**: 79% of appointments have diagnosis codes. Improving coding quality alone could free **15,000–30,000** additional appointment slots.
- **Follow-up Ratios**: Follow-up to first-appointment ratios range from **0.7 to 14.1** across diagnoses. Optimising high-ratio pathways could release **22,000–44,000** appointments.
- **Telehealth Potential**: Diagnoses were scored 0–100 on clinical suitability (examination needs, acuity, monitoring capability). Expanding telehealth for “Safe” and “Hybrid” categories offers an estimated **50,000+** additional capacity.
- **Total Opportunity**: Combined improvements point to **87,000–114,000** additional appointments per year.

---

---

**Dashboard**
##   Executive summary

<img width="591" height="332" alt="image" src="https://github.com/user-attachments/assets/05a52363-8072-4fb3-8e2c-3f0c5afbc35c" />

```Insights:

Analysed 113 million outpatient appointments, of which 89 million have coded diagnoses.
Top diagnosis by volume is Malignant neoplasms (214K attendances).
Current telehealth adoption stands at 17.99%.
Estimated capacity opportunity: 370.19K appointment slots could be freed through optimisation.
Attendance type split shows 56.56% subsequent appointments, highlighting significant follow-up demand.
Shifting just 25% of malignant neoplasm follow-ups to remote care could free approximately 53.5K in-person slots and potentially reduce wait times by 8–12 weeks.

```

## Demand analysis

<img width="590" height="330" alt="image" src="https://github.com/user-attachments/assets/f347c0d0-9b07-4d58-81e2-f5aa0e498aca" />

```Insights:

The top 5 diagnosis groups account for roughly 50% of total outpatient demand.
Malignant neoplasms lead with 214K visits — high clinical priority but currently low telehealth adoption (25%).
Pregnant state, incidental (194K visits) has very low telehealth adoption (7%) and typically requires in-person investigations (ultrasound, blood tests).
After-cataract (171K visits) shows limited remote suitability for initial assessment but potential for routine follow-ups.
High-volume conditions such as pain in joint, degeneration of macula, and other senile cataract also drive substantial demand and should be prioritised for pathway redesign.

```

## Operational Efficiency

<img width="595" height="332" alt="image" src="https://github.com/user-attachments/assets/8949ac5d-ff85-49b1-9879-96a448dd11b0" />

```Insights:

-Average follow-up ratio is 1.6 subsequent appointments per first appointment (range: 0.70 – 14.10 across diagnoses).
-Highest follow-up burdens:
i.Degeneration of macula: 11.40 follow-ups per patient
ii. Malignant neoplasm of prostate: 11.10 follow-ups
iii. Malignant neoplasm of breast: 7.40 follow-ups
-These elevated ratios indicate either appropriate chronic disease monitoring or opportunities to introduce clearer discharge criteria and virtual follow-up models.
- Optimising high-ratio pathways is projected to free 370.19K outpatient slots.
- Diagnoses with both high volume and high follow-up ratios represent the greatest efficiency opportunity.

```

## Tele-health opportunities

<img width="592" height="336" alt="image" src="https://github.com/user-attachments/assets/ddda1ae0-b48f-4bd8-b813-72cbece24d56" />

```Insights:

-Overall telehealth adoption is currently 17.99% (2 million tele appointments out of 113 million total).
-Several low-volume diagnoses already achieve 100% telehealth adoption (e.g. Actinomycetoma, Acute bronchitis, Acute hepatitis B, Agalactia).
-High-volume conditions show much lower adoption:
i. Malignant neoplasm of prostate: 25%
ii. Malignant neoplasm of breast: 21%
iii. Pain in joint: 13%
iv. After-cataract & Degeneration of macula: near 0%
v. Expanding telehealth for clinically suitable high-volume pathways could significantly increase remote capacity while protecting in-person slots for complex cases.
vi. Current adoption is a solid starting point but falls well short of the estimated potential (35–40%) based on diagnosis suitability scoring.
```
## Tools
- **Python:** pandas, numpy
- **Visualization:** matplotlib, seaborn
- **Power BI:** Data modeling, DAX calculations

---

## How to Explore

1. Clone the repository
2. Open the analysis folder for notebooks and scripts
3. Review the Power BI dashboard

---

## Validation
- Data quality checks (null values, duplicates, outliers)
- Spot-checks against raw data
- Peer review with clinicians
- Sensitivity analysis on assumptions

---

## Limitations

- Analysis is retrospective and based on historical patterns
- Telehealth suitability scores are model-based; actual clinical adoption may differ
- External factors (policy changes, workforce constraints) are not modelled
- Some diagnosis coding gaps remain in the source data

---

## Recommendations

- Prioritise high-volume, high follow-up-ratio pathways for pathway redesign
- Pilot telehealth for diagnoses scoring highest on the suitability model
- Improve diagnosis coding completeness as a quick-win capacity lever
- Re-run the analysis quarterly to track impact of interventions

## Author

**Sanjai Kanna CM**  
Business & Data Analytics Portfolio Project
