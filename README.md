# Nhs-outpatient-performance-analysis
I have analyzed 113 million NHS outpatient appointments to identify strategic opportunities for capacity expansion and efficiency improvement.
## Approach
This project uses **Business Analysis** with Python for data processing 
and Power BI for visualization.

### Phase 1: Data Understanding
- Extract 113M appointment records
- Assess data quality (79% have diagnosis codes)
- Identify data gaps & anomalies

### Phase 2: Exploratory Analysis
- Diagnose distribution (top 15 conditions)
- Appointment type patterns (first vs. follow-up)
- Telehealth adoption by diagnosis

### Phase 3: Diagnostic Analysis
- Follow-up ratio by diagnosis (0.7 to 14.1 range)
- Priority score distribution
- Identify outliers & opportunities

### Phase 4: Telehealth Suitability Scoring
- Scored each diagnosis 0-100 based on:
  - Exam requirements (-30)
  - Acuity level (-20)
  - Patient-reported symptoms (+25)
  - Monitoring capability (+20)
- Classified into: Safe, Hybrid, In-Person

### Phase 5: Capacity Projections
- If data quality improved: +15K-30K appointments
- If follow-ups optimized: +22K-44K appointments
- If telehealth expanded: +50K+ appointments
- Total opportunity: 87K-114K appointments

## phase 6: visualisations and insights
- Dashboard using powerbi
-   Executive summary

<img width="591" height="332" alt="image" src="https://github.com/user-attachments/assets/05a52363-8072-4fb3-8e2c-3f0c5afbc35c" />

- Demand analysis

<img width="590" height="330" alt="image" src="https://github.com/user-attachments/assets/f347c0d0-9b07-4d58-81e2-f5aa0e498aca" />

-Operational Efficiency

<img width="595" height="332" alt="image" src="https://github.com/user-attachments/assets/8949ac5d-ff85-49b1-9879-96a448dd11b0" />

-Tele-health opportunities

<img width="592" height="336" alt="image" src="https://github.com/user-attachments/assets/ddda1ae0-b48f-4bd8-b813-72cbece24d56" />

## Tools
- **Python:** pandas, numpy
- **Visualization:** matplotlib, seaborn
- **Power BI:** Data modeling, DAX calculations

## Validation
- Data quality checks (null values, duplicates, outliers)
- Spot-checks against raw data
- Peer review with clinicians
- Sensitivity analysis on assumptions

## Limitations
- Analysis is retrospective (historical data)
- Assumes trends continue (may not)
- Doesn't account for external factors (policy changes.)
- Telehealth projections based on diagnosis suitability (actual adoption may vary)

## Recommendations
- Monitor projections against actual results
- Update analysis quarterly
- Validate assumptions with clinical team
