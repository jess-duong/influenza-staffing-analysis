# Data Directory

This folder contains the integrated datasets and documentation for the Influenza Staffing Analysis.

## Contents

### Final Datasets
- **Intermediate_Workbook_FINAL.xlsx** - Integrated dataset combining CDC mortality, Census population, and vaccination data (2009-2017)
- **Provider_Reallocation.xlsx** - Staffing allocation model based on elderly population distribution

### Documentation
- **Influenza_Interim_Report_FINAL.pdf** - Complete statistical analysis report including:
  - Data integration methodology
  - Descriptive statistics
  - Hypothesis testing results (t-test comparing 65+ vs Under 65 mortality)
  - Vaccination coverage analysis

## Data Sources

1. **CDC Influenza Deaths**: State-level mortality data by age group (2009-2017)
2. **U.S. Census Population Data**: State demographics by age and year
3. **CDC Vaccination Coverage**: Flu vaccination rates for 65+ population
4. **CDC Influenza Visits**: CDC Weekly U.S. Influenza Surveillance Report

## Key Variables

- **State-Year**: Concatenated identifier (e.g., "Alabama_2009")
- **Age Groups**: High Risk (65+), Low Risk (Under 65)
- **Death Rate**: Deaths per 100,000 population
- **Vaccination Rate**: Percentage of 65+ population vaccinated

**Note**: Raw source datasets not included; analysis uses integrated data only.
