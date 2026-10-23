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
<img width="592" height="332" alt="image" src="https://github.com/user-attachments/assets/59e952ce-8a04-4c94-b14f-7893acf36cad" />

-  Top diagnosis by volume is Malignant neoplasms (~214k attendances).

<img width="599" height="334" alt="image" src="https://github.com/user-attachments/assets/34c70a7c-6956-4b53-8c0d-c571f49e14a5" />

- Current telehealth adoption across the data is about 18%.
- Follow-up ratios vary widely (from under 1 to over 14 follow-ups per first appointment).
- Highest follow-up burdens appear in conditions such as degeneration of macula, prostate cancer and breast cancer.
- Improving coding completeness, reducing unnecessary follow-ups, and expanding telehealth on suitable pathways could free a meaningful number of appointment slots (estimates range from tens of thousands to low hundreds of thousands depending on assumptions).

Demand analysis:
<img width="599" height="338" alt="image" src="https://github.com/user-attachments/assets/e8bce30f-80f9-4c0d-8a0d-5747a2a42901" />

operational efficiency:
<img width="601" height="328" alt="image" src="https://github.com/user-attachments/assets/b923afe0-a58b-40c7-977c-a4811dcdf4e3" />

## Tools

- Python (pandas, numpy)
- Matplotlib and Seaborn
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
