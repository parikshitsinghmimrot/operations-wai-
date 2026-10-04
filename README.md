# AI-Based Service Capacity Planning for Ola Electric

Working with AI (WAI) project · Operations & Supply Chain Management (OM-I) · IIM Ranchi
Student: Stephin (PGP 2026–28) · October 2026

## Problem statement
Ola Electric is experiencing a growing after-sales service backlog and long repair turnaround times because service-centre capacity and spare-parts availability have not kept pace with its installed base of scooters. This project uses AI-based demand forecasting, service-centre clustering, complaint text analysis and a breach-prediction model to locate the bottlenecks and recommend targeted technician rebalancing and spare-parts actions.

## Important disclosure
**All quantitative data in this project is synthetic** (simulated by `03_Code/01_generate_synthetic_data.py`, seed 42). It is not Ola Electric's data. The findings demonstrate the method.

## Folder structure
| Folder | Contents |
|---|---|
| 01_Report | Project report (Word) |
| 02_Prompt_Logbook | Prompt logbook (Word) |
| 03_Code | Three commented Python scripts, requirements.txt, outputs/results.json |
| 04_Dashboard | dashboard.html (6 visual insights) and figures/ |
| 05_Slide_Deck | Slide deck (10 slides) |
| 06_Video | 3-minute video or its link (to be added) |
| 07_Data | synthetic_raw/, processed/, data dictionary, data source log, data preparation note |
| 08_Screenshots | Screenshots for the annexures (to be added) |

## How to run the code
1. Install Python 3.10 or later, then `pip install -r 03_Code/requirements.txt`
2. From this folder run, in order:
   `python 03_Code/01_generate_synthetic_data.py`
   `python 03_Code/02_analysis.py`
   `python 03_Code/03_build_dashboard.py`
3. Open `04_Dashboard/dashboard.html` in a browser.

## AI tools used
Claude (generative AI: planning, coding support, drafting; all prompts in the logbook); Python with pandas, scikit-learn and matplotlib.

## Key results (synthetic data)
- Weekly tickets up 46.1%; backlog about 2,122; 35.0% of centre-weeks over the 7-day target in the last 12 weeks.
- Forecast 2,486 tickets a week for the next 12 weeks against capacity 3,141; forecast error 1.9% (baseline 3.0%).
- 4 clusters of centres; breach model accuracy 93.8%.

## Known limitations
Synthetic data; template-based complaint text; cost–benefit figures are assumptions; some references still to be verified (see REFERENCES_TO_VERIFY.md).
