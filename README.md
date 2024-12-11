# City of Boston Budget Analysis

## Executive Summary
This project analyzes the City of Boston's operating and capital budgets to provide actionable insights into spending patterns, resource allocation, and per capita expenditures. Using data from fiscal years FY22 to FY25, the project explores trends in spending across departments, neighborhoods, and programs, and examines discrepancies between projected and actual budgets. The analysis includes a linear regression modeling, data visualizations, and geographical insights to inform strategic decision-making for budget allocations. 

**Key Findings Include:**
- Education and transportation departments dominate funding, while some neighborhoods receive significantly less capital project investment.
- Discrepancies between projected and actual spending highlight areas for improved budget forecasting.
- Per capita spending varies significantly across services, with notable disparities in education and housing investments.

The results are presented through clear visualizations, a regression model, and an interactive website. 

---
## Introduction

### Project Goals
The primary objectives of this project are:
1. Analyze the city's annual operating and capital budgets across departments, programs, and geographies.
2. Examine discrepancies between projected and actual spending.
3. Explore per capita spending in areas such as education and housing.
4. Provide clear and actionable visualizations to support strategic improvements in resource allocation. 

### Motivation
Efficient budget allocation is critical for addressing the diverse needs of Boston's residents. This project aims to uncover patterns in spending, identify areas of inequity, and provide tools for better decision-making. By leveraging data science appraoches, we aim to enhance transparency and accountability in the city's budgeting process. 

--- 
## Data Description
We utilized the following datasets for analysis:
1. **Operating Budget Data**  
	- **Source**: [FY24 Recommended Operating Budget](https://data.boston.gov/dataset/operating-budget/resource/8f2971f0-7a0d-401d-8376-0289e3b810ba)  
	- **Description**: Provides a detailed breakdown of departmental expenses, programs, and expense categories from FY22 to FY25.

2. **Capital Budget Data**  
	- **Source**: [FY24 Recommended Capital Budget Plan](https://data.boston.gov/dataset/capital-budget/resource/c62d666e-27ea-4c03-9cb1-d3a81a1fb641)  
	- **Description**: Includes funding authorizations, expenditures, and project details for capital investments across neighborhoods.

3. **Supplementary Socio-Economic Data**  
	- **Source**: Boston’s Social Vulnerability Index and Census data  
	- **Description**: Socio-economic indicators for Boston neighborhoods used to explore correlations with spending patterns.

---
## Methodology

### Data Preparation and Cleaning
1. **Missing Values**: Missing data were replaced with `NaN` and handled using imputation or removal, depending on the context.  
2. **Data Standardization**: Column headers were standardized, and numeric fields were converted for analysis.  
3. **Geographic Mapping**: Neighborhood-level data were geocoded for visualization.  


### Exploratory Data Analysis (EDA)
We conducted a comprehensive analysis of budget allocations and spending trends:  

1. **Top Departments by Budget**: Identified the top 10 departments by FY25 budget allocation.  
2. **Expense Categories**: Examined personnel costs, contracted services, and other expense categories.  
3. **Neighborhood Spending**: Analyzed the distribution of capital projects across Boston neighborhoods.  
4. **Year-over-Year Changes**: Evaluated trends in budget growth from FY22 to FY25.  

### Modeling Approach
1. **Linear Regression**: Modeled discrepancies between projected and actual spending to identify key drivers.  
2. **Time Series Analysis**: Analyzed spending trends over time for departments and programs.  
3. **Clustering**: Grouped neighborhoods based on socio-economic indicators and spending patterns.  
4. **Feature Engineering**: Included variables like department, expense category, and neighborhood socio-economic data.  

### Visualization Techniques
1. **Bar and Line Charts**: For department-level and year-over-year spending analyses.  
2. **Choropleth Maps**: Visualized capital funding distribution across neighborhoods.  
3. **Scatter Plots**: Explored per capita spending by department and program.  
4. **Interactive Visuals**: Developed interactive graphs and maps for the accompanying website.

---

## Results and Insights

1. **Spending by Department**  
	- Education and transportation dominate the budget, receiving over 50% of total funding.  
	- Smaller departments, such as Arts & Culture, receive significantly less funding, highlighting potential disparities.  

2. **Geographic Disparities**  
	- Capital projects are concentrated in certain neighborhoods (e.g., Chinatown, Charlestown), while others (e.g., Mission Hill, Hyde Park) receive less investment.  
	- Socio-economic factors correlate strongly with capital spending, suggesting inequities in funding distribution.  

3. **Projected vs. Actual Spending**  
	- Discrepancies between projected and actual spending reveal consistent underutilization in some areas, particularly in housing and public health.  
	- Regression analysis identifies personnel costs and grant dependencies as significant predictors of discrepancies.  

4. **Per Capita Spending**  
	- Education sees the highest per capita spending, while housing and public health lag behind.  
	- Visualization of per capita spending highlights areas where resources may need to be reallocated.

---

## Visualization Highlights
The following visualizations were created to support the analysis:  

1. **Departmental Spending**: A stacked bar chart showing budget allocations by department.  
2. **Capital Project Distribution**: A choropleth map highlighting neighborhood-specific investments.  
3. **Projected vs. Actual Spending**: A line graph overlaying projections and actual expenditures over time.  
4. **Per Capita Analysis**: Scatter plots comparing spending across departments and programs.  
5. **Interactive Dashboard**: Available on the project website, allowing further exploration of key metrics.  

---

## Challenges and Limitations  
1. **Data Gaps**: Missing data in some fields limited the scope of analysis.  
2. **Model Assumptions**: Linear regression assumes relationships that may not fully capture the complexity of budget allocations.  
3. **Granularity**: Some datasets lacked detailed program-level information, limiting deeper dives into specific initiatives.  

---

## Conclusion
The City of Boston's budget analysis highlights critical patterns and disparities in resource allocation. Education and transportation receive the majority of funding, but geographic disparities in capital investment and underfunding of key areas like housing need attention. The linear regression model and visualizations provide actionable insights to improve future budget planning and allocation.  

---

## Future Work
1. Incorporate real-time budget tracking to address discrepancies early.  
2. Expand socio-economic analysis to include more granular neighborhood-level data.  
3. Explore machine learning models for more accurate budget forecasting.  

---

## Deliverables
1. **Code Repository**: Includes cleaned datasets, analysis notebooks, and modeling scripts.  
2. **Final Report**: A professional document summarizing the analysis and findings.  
3. **Website**: Interactive visualizations and graphs, including the regression model output.  

---

Project by:  
Ryan Gilbert, Kae Chi, Oscar Mo, Chris Min, Alan Lin  
Boston University  
CS506 Fall 2024
