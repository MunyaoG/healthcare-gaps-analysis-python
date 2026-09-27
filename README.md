# Mapping Healthcare Access Gaps in Nairobi County

A facility-level analysis of Nairobi County's health infrastructure against Universal Health Coverage (SDG Target 3.8) and related SDG 3 targets — identifying where the county is underserved and what it would take to close the gap.

**[Read the full case study →](https://munyaog.github.io/healthcare-gaps-analysis-python/)**

## What this is

SDG Target 3.8 calls for universal access to quality healthcare. County-level averages hide a lot, so this analysis combines Nairobi's health facility registry with sub-county census population data to benchmark each of the county's ten regions against WHO and county target ratios for:

- Facility density (facilities per 10,000 population)
- Hospital bed and cot availability (beds per 10,000 population)
- Four specific services: inpatient/home-based care, childhood illness management (C-IMCI), HIV treatment (ART), and family planning (FP)

## Key findings

- Of 942 registered facilities, 19 are closed and 6 are pending opening — untapped capacity that could be restored faster than building new facilities.
- Medical clinics and dispensaries make up ~70% of all facilities; district/national referral hospitals are rare, limiting access to specialised care.
- Mathare, Kasarani, and Embakasi are the most underserved regions by facilities-per-capita, all under the 2-per-10,000 target.
- Mathare has zero cots county-wide — a specific, low-cost gap in neonatal/paediatric care.

Full breakdown, region-by-region tables, and recommendations are in the case study write-up linked above.

## Data sources

- [Kenya Master Health Facility Registry](https://open.africa/dataset/health-facilities-in-kenya) (via open.Africa)
- [2019 Kenya Population and Housing Census](https://open.africa/dataset/2019-kenya-population-and-housing-census) — sub-county level
- Targets referenced: WHO and UN SDG 3 indicators (3.2, 3.3, 3.7, 3.8)

## Repo contents

```
├── Nairobi Healthcare Gaps Study.ipynb                                                   # Full analysis: data cleaning, region mapping, gap calculations, charts
├── Presentation - Healthcare Access Gaps in Nairobi.pptx                                  # Slide summary of findings and recommendations
├── ehealth-kenya-facilities-download-21102015.xls                                        # Health facility registry (KMHFR)
├── kenya-population-by-sub-county.csv                                                     # Sub-county population totals
├── distribution-of-population-by-age-sex-county-and-sub-county-kenya-2019-census-volume-iii.csv
├── distribution-of-population-by-sex-and-sub-locations-2019-census-volume-ii.csv
└── README.md
```

## Tools

Python · pandas · numpy · matplotlib · Jupyter

## Running it locally

```bash
git clone https://github.com/MunyaoG/healthcare-gaps-analysis-python.git
cd healthcare-gaps-analysis-python
pip install pandas numpy matplotlib xlrd
jupyter notebook "Nairobi Healthcare Gaps Study.ipynb"
```
