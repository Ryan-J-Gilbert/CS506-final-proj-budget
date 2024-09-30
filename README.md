# City of Boston Budget Analysis

## Description of the Project
This project aims to analyze the City of Boston's operating and capital budgets over time. The focus will be on understanding spending patterns by department, geography, program, and budget category. Additionally, we will explore discrepancies between projected and actual spending, identify per capita spending in areas such as education and housing, and provide visual insights to help inform strategic decisions for the city's resource allocation.

## Goals
- Analyze the city’s annual operating and capital budgets across different departments and geographies.
- Examine how actual spending differs from projected budgets.
- Explore per capita spending for specific services like schools and housing.
- Provide clear visualizations that help the City of Boston make strategic improvements to their budget allocations.

## Data Collection
The following datasets will be used for analysis:

1. **Operating Budget Data**: A detailed breakdown of city spending across departments, services, and personnel expenses.
   - **Source**: [FY24 Recommended Operating Budget](https://data.boston.gov/dataset/operating-budget/resource/8f2971f0-7a0d-401d-8376-0289e3b810ba)
  
2. **Capital Budget Data**: Information on capital projects, including funding sources such as bonds and grants.
   - **Source**: [FY24 Recommended Capital Budget Plan](https://data.boston.gov/dataset/capital-budget/resource/c62d666e-27ea-4c03-9cb1-d3a81a1fb641)
   
### We may also explore extensions to the analysis by incorporating additional datasets:  
3. **Supplementary Socio-Economic Data**: Socio-economic indicators for neighborhoods and districts to explore correlations with budget allocations.
   - **Source**: Boston's Social Vulnerability Index, Census data.

4. **Revenue Analysis**: How has revenue shifts impacted different departments, programs, geographies?
   - **Source**: [Boston Revenue Budget](https://data.boston.gov/dataset/revenue-budget#:~:text=The%20FY24%20Adopted%20Budget%20is,million%20in%20non%2Drecurring%20revenue.)

5. **Housing Cost**: How does housing cost impact budget allocation?
   - **Source**: [Boston Housing Cost](https://library.bu.edu/c.php?g=1151960&p=8408504)



## Data Modeling Plan
The analysis will incorporate the following modeling techniques:

- **Time series analysis**: To assess spending trends over time.
- **Regression analysis** or **Clustering**: To identify patterns in discrepancies between projected and actual spending.
- **Decision tree based models (e.g. RandomForest, XGBoost, LightGBM)** and/or **linear models**: To model relationships between socio-economic factors and spending patterns by geography and program.

## Data Visualization Plan
Visualizations will be created to present key findings:

- **Spending by department**: Bar charts or stacked area charts for department-level analysis.
- **Spending by geography**: Choropleth maps to visualize how funding is distributed across different neighborhoods.
- **Projected vs. actual spending**: Line graphs showing trends in budget allocations over time, with overlays for forecast vs. actual spending.
- **Per capita spending**: Scatter plots with color and size encoding to show spending variations across departments and programs.

## Test Plan
- Data for models will be split into **training** and **testing** sets. For example, 20% of the data will be withheld as a validation set to evaluate model performance.
- Model performance will be assessed by comparing predicted spending patterns with actual spending on the test set.

## Repository
The complete code, datasets, and documentation will be uploaded to this repository.

## Deliverables
1. **Code and cleaned datasets**: Uploaded to the repository.
2. **Documentation**: A detailed README with instructions on how to run the code and descriptions of methodologies.
3. **Final Report**: Addressing the project goals and presenting insights from the analysis, including visualizations.
4. **Presentation**: A summary of key findings with the best visualizations supporting the insights.

---

Project by:  
Ryan Gilbert, Kae Chi, Oscar Mo, Chris Min, Alan Lin  
Boston University  
CS506 Fall 2024
