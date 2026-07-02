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
