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
## Midterm Report

The notebook conducts an in-depth analysis of the City of Boston's budget allocations, exploring how spending is distributed across departments, programs, and other key financial categories. The primary aim is to understand trends, evaluate spending priorities, and explore relationships within the budget data.

### Datasets Used

#### FY25 Adopted Operating Budget

The main dataset analyzed is the **FY25 Adopted Operating Budget**, sourced from Boston’s Open Data Portal. This dataset provides comprehensive information on budget allocations and spending for the fiscal years from FY22 to FY25 across various city departments and programs. Key fields in this dataset include:

- **Cabinet**: Identifies the overarching city government cabinet to which a department belongs (e.g., Public Health, Education, Housing).
- **Department (Dept)**: Specifies the department or agency receiving funds.
- **Program**: Further delineates the department’s budget into specific programs or initiatives.
- **Expense Category**: Groups expenses into categories, such as personnel, contracted services, supplies, current charges, and equipment.
- **FY22 Actual Expense**: Reflects actual expenditures made in FY22.
- **FY23 Actual Expense**: Reflects actual expenditures made in FY23.
- **FY24 Appropriation**: Shows the allocated budget for FY24.
- **FY25 Budget**: The current budget amount allocated for FY25.

#### FY25 Capital Budget Data

In addition to the operating budget, an **FY25 Capital Budget** dataset is also examined, which outlines authorized funding and expenses related to long-term projects. This dataset provides insight into capital-intensive projects across Boston neighborhoods, including transportation improvements, community facilities, and public safety enhancements. Key columns include:

- **Department**: The department managing the capital project.
- **Project Name**: Name of the capital project.
- **Scope of Work**: Describes the work and objectives of each project.
- **Neighborhood**: Indicates the specific neighborhood or area affected by the project.
- **Authorization Existing/FY/Future**: Lists existing, FY-specific, and future authorizations of funds.
- **GO Expended and Grant Expended**: Details expenses from general obligation (GO) funds and grants.
- **Capital and Grant Yearly Spending**: Shows yearly spending plans for capital projects over the next few years.
- **Total Project Budget**: Total budget amount planned for the entire project.

---

### Data Preparation and Cleaning

#### Handling Missing Values
Both datasets were initially examined for missing or incomplete values. For easier processing, placeholders such as `#Missing` were replaced with `NaN` values, allowing for consistent handling in subsequent analysis steps.

#### Data Formatting
Column headers were standardized for readability, and numeric columns were converted to appropriate data types to facilitate analysis.

---

### Exploratory Data Analysis (EDA)

The analysis begins with several key exploratory steps to understand the budget allocation structure and trends across the fiscal years:

1. **Top 10 Departments by Budget**:
   - A pie chart was generated to show the proportions of the FY25 budget allocated to the top 10 departments. This helps highlight which departments receive the highest funding, with all remaining departments grouped into an “Other” category.

2. **Overall Budget Change Analysis**:
   - The notebook examines budget changes across FY22 to FY25, comparing year-over-year budget increases. This analysis highlights the growth trend and overall spending increases in percentage terms over the years.

3. **Expense Category Breakdown**:
   - A breakdown of the budget by expense category (e.g., personnel, contracted services, supplies) is analyzed to identify where most funds are being directed, offering insights into Boston’s operational cost structure.

4. **Capital Projects by Neighborhood**:
   - Using the capital budget data, spending on projects across Boston neighborhoods is explored. This dataset provides the opportunity to map budget allocation geographically, allowing for a better understanding of area-specific investments.

---

### Additional Insights and Visualizations

The notebook presents various visualizations to enhance the understanding of Boston’s budget data:

- **Year-over-Year Budget Change**: Bar charts showing how budget allocations have shifted annually.
- **Interactive Mapping**: With plans to use `GeoPandas` and `Folium`, this analysis aims to provide an interactive view of capital spending across Boston neighborhoods, making it easier to visualize and compare spending geographically.

https://youtu.be/0-sRxWNKfJg
---

Project by:  
Ryan Gilbert, Kae Chi, Oscar Mo, Chris Min, Alan Lin  
Boston University  
CS506 Fall 2024
