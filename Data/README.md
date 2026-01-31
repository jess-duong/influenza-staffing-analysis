# Data Directory

This folder contains the integrated datasets and documentation for the Influenza Staffing Analysis.

## Contents

### Final Datasets
- **Influenza_workbook.xlsx** - Integrated dataset combining CDC mortality, Census population, and vaccination data (2009-2017)
- **Provider_reallocation.xlsx** - Staffing allocation model based on elderly population distribution and visit patterns

### Documentation
- **Influenza_Interim_Report_FINAL.pdf** - Complete statistical analysis report including:
  - Data integration methodology
  - Descriptive statistics
  - Hypothesis testing results (t-test comparing 65+ vs Under 65 mortality)
  - Vaccination coverage analysis

## Data Sources

1. **CDC Influenza Deaths**: State-level mortality data by age group (2009-2017)
   - Source: https://wonder.cdc.gov/ucd-icd10.html

2. **U.S. Census Population Data**: State demographics by age and year (2009-2017)
   - Source: U.S. Census Bureau surveys

3. **CDC Vaccination Coverage**: Flu vaccination rates for 65+ population (2009-2016)
   - Source: https://data.cdc.gov/Flu-Vaccinations/

4. **CDC Influenza-Related Healthcare Visits**: Monthly influenza visit data by state
   - Used for seasonal pattern analysis and provider reallocation modeling
   - Source: CDC surveillance data

## Key Variables

- **State-Year**: Concatenated identifier (e.g., "Alabama_2009")
- **Age Groups**: High Risk (65+), Low Risk (Under 65)
- **D
