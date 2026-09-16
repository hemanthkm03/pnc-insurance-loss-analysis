# P&C Insurance Claims & Loss Ratio Analysis

## Problem Statement
Analyzing claims and policy data to identify loss ratio drivers, claim risk 
patterns, and revenue leakage opportunities for a P&C insurer.

## Dataset
PnC Insurance Practice Dataset (Kaggle) — includes policy, claims, region, 
coverage type, claim amount, and earned premium data.

## Approach
1.⁠ ⁠**Data Cleaning** (Python/pandas) — handled missing values, standardized 
   date formats, validated claim/policy date logic, flagged data quality issues

2.⁠ ⁠*Analysis* (SQL) — JOINs, GROUP BY, CASE statements, window functions, 
   and CTEs to calculate loss ratios by segment, region, and coverage type

3.⁠ ⁠*Statistical Analysis* (Python) — claim frequency distribution, severity 
   trends, correlation analysis, hypothesis testing across segments
   built to support pricing and underwriting decisions

4. *Dashboard* (Tableau) - KPI cards, product and region loss ratio breakdowns 
   built to support pricing and underwriting decisions

## Key Findings
- **Overall portfolio loss ratio is 158%**, well above the healthy 60-70% benchmark, 
  indicating the book as a whole is unprofitable
- *Auto is the single biggest driver of losses*, with a loss ratio of 404.2% — 
  claims paid out are 4x the premium collected for this line
- *Home is the second-worst performer* at 295.9%, also far above sustainable levels
- *Commercial Auto (89.6%) and Commercial Property (30.0%)* are comparatively 
  healthy, with Commercial Property actually profitable — these lines are 
  correctly priced and not contributing to the portfolio's losses
- *Geographically, the South (191%) and Midwest (178.1%)* carry the highest loss 
  ratios, while the Northeast (114.8%) is the best-performing region, though still 
  above benchmark
- *West (149.9%)* sits in between — elevated, but less severe than South/Midwest

## Recommendations
- *Immediate rate review for Auto and Home*: At 404% and 296% loss ratios, these 
  two personal lines are the primary source of portfolio losses — a rate adequacy 
  review and repricing is the top priority
- *Regional underwriting tightening in South and Midwest*: These regions show 
  loss ratios 20-35 points above the Northeast, suggesting geographic risk 
  concentration — tighten underwriting criteria or adjust rates by region
- *Preserve current pricing on Commercial lines*: Commercial Auto and especially 
  Commercial Property are performing well (30-90% loss ratio) — no immediate 
  action needed here, and these lines could offset losses if the book is rebalanced 
  toward them
- *Consider non-renewal or reinsurance for the worst-performing segment*: Given 
  Auto's severity, evaluate excess-of-loss reinsurance or selective non-renewal 
  for the highest-risk Auto policies while repricing takes effect

 ## Repo Structure
├── data/ # raw_claims.csv, cleaned_claims.csv

├── pnc_insurance_analysis.ipynb  # Data cleaning + loss ratio analysis

├── Images/   # Dashboard screenshot

└── README.md


## Dashboard
   **View the live interactive dashboard**
   ![Dashboard](![Dashboard](images/Dashboard.png)
  https://public.tableau.com/views/PCInsuranceLossRatioAnalysis/PCInsuranceLossRatioAnalysis?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
