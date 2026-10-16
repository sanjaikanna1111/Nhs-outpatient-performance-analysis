# NHS Outpatient Performance Analysis

This project analyses NHS outpatient appointment data at diagnosis level to identify opportunities for capacity expansion and efficiency improvement.

It focuses on three questions:

1. Where is demand concentrated, and which conditions drive the highest volume?
2. How efficient is the current mix of first appointments vs follow-ups?
3. Which diagnoses look most suitable for telehealth, and what capacity could that unlock?

## Data

- Source: NHS outpatient activity data (diagnosis-level summary)
- Working dataset: ~7,300 diagnosis codes with attendance counts
- Total attendances represented in the data: ~113 million
- Note: This is aggregated summary data, not 113 million individual patient records.

## Approach

| Phase | Focus | What I did |
|-------|-------|------------|
| 1 | Data understanding | Loaded and cleaned the diagnosis-level data, checked quality |
| 2 | Exploratory analysis | Looked at diagnosis volumes, appointment types, telehealth use |
| 3 | Diagnostic analysis | Calculated follow-up ratios and flagged high-burden pathways |
| 4 | Telehealth suitability | Built a simple 0–100 scoring approach based on clinical factors |
| 5 | Capacity estimates | Estimated potential slots that could be freed |
| 6 | Visualisation | Built a Power BI dashboard |

## Key Findings

- Top diagnosis by volume is Malignant neoplasms (~214k attendances).
- Current telehealth adoption across the data is about 18%.
- Follow-up ratios vary widely (from under 1 to over 14 follow-ups per first appointment).
- Highest follow-up burdens appear in conditions such as degeneration of macula, prostate cancer and breast cancer.
- Improving coding completeness, reducing unnecessary follow-ups, and expanding telehealth on suitable pathways could free a meaningful number of appointment slots (estimates range from tens of thousands to low hundreds of thousands depending on assumptions).

## Tools

- Python (pandas, numpy)
- Matplotlib / Seaborn
- Power BI

## How to explore

1. Clone the repository
2. Open the `analysis` folder for the notebook
3. Review the Power BI dashboard file

## Limitations

- The analysis uses aggregated diagnosis-level data, not individual appointment records.
- Telehealth suitability scores are based on a simple model and would need clinical review.
- Capacity estimates depend on assumptions and should be treated as directional.
- External factors (staffing, policy, estate) are not modelled.

## Recommendations

- Focus first on high-volume diagnoses that also have high follow-up ratios.
- Pilot telehealth on pathways that score well on the suitability model.
- Improve diagnosis coding completeness where it is currently incomplete.
- Re-run the numbers after any pathway changes to check impact.

## Author

Sanjai Kanna CM  
Business & Data Analytics Portfolio Project
