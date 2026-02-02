# Yield Curve & Spread Analysis (US)

This project uses **FRED** macro-financial data to analyze the US yield curve and key spreads:
- **2s10s** = 10Y − 2Y
- **3m10y** = 10Y − 3M

We overlay **NBER recession periods** (USREC) and relate yield curve dynamics to inflation (CPI).

## Notebook
- `notebook/01_yield_curve_spreads.ipynb`

## What this shows
- Yield curve regimes over time (3M, 2Y, 10Y)
- Spread inversions and how they align with recessions
- Basic inflation context using CPI YoY

## Data sources
All data is downloaded directly from FRED:
- DGS3MO, DGS2, DGS10 (Treasury yields)
- CPIAUCSL (CPI)
- USREC (NBER recession indicator)

## How to run
1) Create and activate an environment (conda or venv)
2) Install dependencies:
```bash
pip install -r requirements.txt
