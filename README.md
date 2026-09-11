# P&C Insurance Claims & Loss Ratio Analysis

## Problem Statement
Analyzing claims and policy data to identify loss ratio drivers, claim risk 
patterns, and revenue leakage opportunities for a P&C insurer.

## Dataset
PnC Insurance Practice Dataset (Kaggle) — includes policy, claims, region, 
coverage type, claim amount, and earned premium data.

## Approach
1.⁠ ⁠*Data Cleaning* (Python/pandas) — handled missing values, standardized 
   date formats, validated claim/policy date logic, flagged data quality issues
2.⁠ ⁠*Analysis* (SQL) — JOINs, GROUP BY, CASE statements, window functions, 
   and CTEs to calculate loss ratios by segment, region, and coverage type
3.⁠ ⁠*Statistical Analysis* (Python) — claim frequency distribution, severity 
   trends, correlation analysis, hypothesis testing across segments
4.⁠ ⁠*Dashboard* (Power BI) — KPI cards, trend lines, and segment drill-downs 
   built to support pricing and underwriting decisions

## Key Findings
•⁠  ⁠Auto and Home product lines show loss ratios of 400%+ and 296% respectively, 
  far above the healthy 60-70% benchmark

## Recommendations
•⁠  pricing adjustments, underwriting rule changes, fraud review triggers

## Repo Structure
