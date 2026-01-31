# Influenza Staffing Analysis

**Statistical analysis of CDC influenza mortality data (2009-2017) to optimize medical staffing allocation during flu season.**

[![View Dashboard](https://img.shields.io/badge/Tableau-Interactive_Dashboard-orange)](https://public.tableau.com/app/profile/jess.duong/viz/InfluenzaBurdenVaccinationCoverage/InfluenzaStaffingAnalysis)
[![View Report](https://img.shields.io/badge/View-Analysis_Report-blue)](Data/)

## Project Overview

A medical staffing agency needed data-driven guidance for deploying temporary healthcare workers during influenza season. This analysis examined CDC mortality data, U.S. Census population demographics, and vaccination coverage records to identify which states and populations require prioritized staffing resources.

### Business Problem
Medical staffing agencies face the challenge of efficiently allocating limited temporary staff during flu season peaks. This project analyzes mortality patterns and population demographics to determine where additional healthcare capacity would have the greatest impact.

### Key Questions
- Which populations face the highest influenza mortality risk?
- Which geographic areas require priority staffing deployment?
- How do seasonal patterns inform optimal timing for resource allocation?
- Does vaccination coverage reduce staffing demand?

### Key Findings
- **Adults 65+ face 5.2x higher influenza mortality** compared to under-65 population (statistically significant, p<0.0001)
- **Deaths peak December through March**: Requiring proactive pre-winter staffing deployment
- **High-risk states identified**: CA, PA, TX, NY, FL show highest absolute death counts
- **Vaccination coverage shows minimal impact** on state-level mortality (R²=0.15); should not reduce staffing allocation

## Tools & Techniques

**Tools**: Excel, Tableau, Statistical Analysis (Welch's t-test)  
**Skills**: Data integration, hypothesis testing, correlation analysis, interactive dashboard design, public health analytics

### Analytical Approach
- Integrated 4 datasets using State-Year concatenated keys
- Calculated death rates per 100,000 population for standardization
- Conducted statistical hypothesis testing (65+ vs Under 65 mortality)
- Analyzed correlation between elderly population size and death counts (R²=0.88)
- Built interactive Tableau dashboard for geographic and temporal visualization
- Developed staffing allocation model prioritizing high-elderly-population states

## 📁 Repository Contents
```
├── Data/                       # Integrated datasets and statistical report
├── Visualizations/             # Tableau dashboard (link) and Excel charts
├── Analysis/                   # Statistical methodology documentation
└── README.md                   # Project documentation
```

## Strategic Recommendations

### Prioritize Elderly-Serving Facilities
- Deploy temporary staff to hospitals and clinics with high 65+ patient concentration
- Focus resources in states with largest elderly populations (CA, PA, TX, NY, FL)
- Scale staffing levels based on state-specific elderly population forecasts

### Optimize Seasonal Timing
- **Pre-position workers before December surge** (deaths peak Dec-Mar)
- Maintain elevated staffing capacity through early spring
- Use monthly visit patterns to anticipate demand spikes

### Geographic Allocation Strategy
- Elderly population size is the strongest predictor of staffing need (R²=0.88)
- Deaths scale linearly with 65+ population across all states
- Vaccination rates should NOT reduce allocation estimates (weak correlation)

### Support Preventive Efforts
- Coordinate with vaccination outreach programs in high-risk areas
- Allocate staff to support early intervention initiatives
- Focus on facilities serving vulnerable elderly populations

## 📈 Data Scope & Methodology

**Datasets Integrated**:
- CDC Influenza Mortality (2009-2017): State-level deaths by age group
- U.S. Census Population Data: Demographics by state, year, age
- CDC Vaccination Coverage: Flu vaccination rates for 6 months+ (https://www.cdc.gov/fluvaxview/interactive/general-population-coverage.html)
- CDC Healthcare Visits: Monthly influenza-related visits by state

**Time Period**: 2009-2017  
**Geographic Coverage**: 50 states + District of Columbia  
**Final Dataset**: 458 state-year observations

### Statistical Analysis
- **Hypothesis Test**: Welch's t-test (unequal variances)
- **Result**: 65+ population shows significantly higher mortality (mean death rate 120.8 vs 23.1 per 100k, p<0.0001)
- **Correlation Analysis**: Strong positive correlation between elderly population and deaths (R²=0.88)
- **Vaccination Impact**: Minimal correlation with mortality rates (R²=0.15)

### Data Limitations
- **Incomplete 2017 data**: Partial year; excluded from trend analysis
- **Missing geographic data**: Florida influenza visit data unavailable
- **CDC suppression**: Small death counts (<10) suppressed in less populous states
- **State-level aggregation**: Ecological fallacy may affect individual-level interpretation

## Interactive Dashboard

🔗 **[View Full Tableau Dashboard](https://public.tableau.com/app/profile/jess.duong/viz/InfluenzaBurdenVaccinationCoverage/InfluenzaStaffingAnalysis)**

### Dashboard Features
- **Geographic Heatmap**: Influenza mortality rates by state
- **Seasonal Patterns**: Monthly healthcare visit trends
- **Age Group Comparison**: 65+ vs Under 65 mortality visualization
- **Priority States**: Ranked by elderly population and death counts
- **Vaccination Analysis**: Coverage rates vs outcomes

## 📚 Documentation

- **[Complete Statistical Report](Data/)**: Hypothesis testing, descriptive statistics, correlation analysis
- **[Data Integration Methodology](Data/)**: Detailed documentation of merge process and calculated fields
- **[Interactive Visualizations](Visualizations/)**: Tableau dashboard and Excel charts

## Project Context

This project was completed as part of CareerFoundry's Data Analytics program, demonstrating proficiency in:
- Multi-source data integration and cleaning
- Statistical hypothesis testing and interpretation
- Public health analytics and resource allocation modeling
- Interactive dashboard design for stakeholder decision-making
- Translating analytical findings into actionable business strategy

### Technical Notes
- **Data Integration**: Used State-Year concatenated keys to merge 4 datasets
- **Age Grouping**: Combined CDC age categories into High Risk (65+) and Low Risk (Under 65)
- **Rate Calculation**: Deaths per 100,000 population for cross-state comparability
- **Visualization Tool**: Tableau Public for interactive geographic and temporal analysis
- **Statistical Software**: Excel for hypothesis testing and correlation analysis

## Next Steps & Future Analysis

### Recommended Enhancements
- **Validate with complete 2017+ data**: Update analysis with recent complete years
- **Expand age stratification**: Explore 55-64 age group (preliminary analysis suggests elevated risk)
- **Incorporate healthcare infrastructure**: Add hospital capacity and rural/urban distribution metrics
- **Develop predictive models**: Build forecasting tools using historical patterns and population projections
- **Real-time integration**: Connect to live CDC surveillance data for dynamic staffing adjustments

## Author

**Jess Duong**  
Data Analyst | [LinkedIn](https://linkedin.com/in/jessica-duong-35690847/) | [GitHub](https://github.com/jess-duong) | duong.t.jess@gmail.com

---

*For questions about methodology or to discuss this analysis, please reach out via [LinkedIn](https://linkedin.com/in/jessica-duong-35690847/) or open an issue in this repository.*
