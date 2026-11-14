# The Hidden Wait: Healthcare Claims Denial Analysis

## Project Overview

The Hidden Wait is a healthcare data analytics portfolio project exploring in-network health insurance claims denial rates and data reporting completeness across 30 states.

Using publicly available CMS Transparency in Coverage data, this project examines how denial rates vary by state and evaluates the completeness of plan-level claims reporting.

The analysis focuses on individual Marketplace medical Qualified Health Plans (QHPs), using claims data reported for calendar year 2024.

The project was inspired by questions about the healthcare billing experience. However, the dataset measures claims denials rather than actual patient billing wait times.

## Project Objectives

- Calculate the overall claims-weighted in-network denial rate.
- Compare in-network claims denial rates across 30 states.
- Identify states with the highest and lowest reported denial rates.
- Evaluate plan-level data completeness and missing or suppressed values.
- Build an Excel dashboard to communicate key findings and data-quality limitations.

- ## Dataset Information

Source: Centers for Medicare & Medicaid Services (CMS)

Dataset: 2026 Transparency in Coverage Public Use File (PUF)

Reporting Period: Calendar year 2024

Coverage: Individual Marketplace medical Qualified Health Plans (QHPs)

Geographic Scope: 30 states represented in the analysis workbook

Key Fields: State, insurance issuer, plan identifier, in-network claims received, and in-network claims denied.

Data Notes: The dataset contains insurer-reported information. Missing, suppressed, and nonapplicable values were not treated as zero.

## Tools & Techniques

### Microsoft Excel
- Data cleaning and validation
- IF, IFERROR, COUNTIFS, SUMIFS, INDEX, MATCH, MIN, and MAX formulas
- PivotTables and claims-weighted calculations
- Data completeness analysis
- State-level comparison charts
- Dashboard development

### GitHub
- Project documentation
- Portfolio file organization
- Version control

  ## Key Findings

  Overall in-network claims denial rate: 19.04% (claims-weighted, based on valid plan-level records).
  Total reported claims received: 344,346,696.
  Total reported claims denied: 65,578,278.
  Highest state denial rate: Hawaii (HI) — 26.85%.
  Lowest state denial rate: South Dakota (SD) — 6.82%.
  Overall plan data completeness: 60.76%.
  States with below 50% plan data completeness: 9.

These findings are descriptive and should be interpreted alongside reporting completeness and data-quality limitations.

## Methodology

1. Reviewed CMS plan-level in-network claims data for calendar year 2024.
2. Identified valid records with numeric claims received and denied, where claims received were greater than zero.
3. Excluded suppressed, missing, and nonapplicable values from denial-rate calculations rather than treating them as zero.
4. Calculated claims-weighted denial rates by dividing valid denied claims by valid received claims.
5. Aggregated results by state and evaluated plan-level reporting completeness.
6. Created an Excel dashboard to present the findings and data-quality notes.

## Limitations

- CMS data are issuer-reported and may contain missing or suppressed values.
- The analysis includes 30 states represented in the workbook and is not a nationwide estimate.
- Reporting completeness varies across states and can affect comparisons.
- Claims may be denied for different reasons; denial rates alone do not establish insurer quality.
- The dataset does not measure how long patients wait for a final medical bill.
- Results are descriptive and do not establish causation.

  ## Project Files

- `Healthcare_Claims_Analysis_Working.xlsx` — Excel workbook containing the source data, state-level analysis, calculations, and dashboard.
- `The_Hidden_Wait_Healthcare_Claims_Dashboard.pdf` — PDF export of the Excel dashboard, including findings and data-quality notes.
- `README.md` — Project overview, methodology, findings, and limitations.

## Future Enhancements

- Develop an interactive Power BI dashboard.
- Explore SQL-based analysis.
- Use Python for additional data validation and visualization.
