# NYC Motor Vehicle Collisions Analysis

## Project Overview

The NYC Motor Vehicle Collisions project aims to analyze collision data from New York City to uncover insights related to collision causes, time patterns, and fatality analysis. This project involves data profiling, staging, dimensional modeling, and the creation of business intelligence dashboards.

## Project Components

### 1. Data Profiling

**Objective**: Assess the quality and structure of the motor vehicle collision data to identify any anomalies or issues.

**Procedure**:
- **Tool**: Use [Alteryx](https://www.alteryx.com/) for data profiling.
- **Tasks**:
  - Analyze data for completeness, consistency, and accuracy.
  - Identify missing values, duplicates, and inconsistencies.
  - Document findings and prepare a data quality report.

### 2. Data Staging

**Objective**: Load raw collision data into staging tables to prepare it for further transformation and integration.

**Procedure**:
- **Tool**: Use [Talend](https://www.talend.com/) for ETL processes.
- **Tasks**:
  - Create staging tables in your chosen database (SQL Server, Azure SQL, MySQL).
  - Load the raw data into staging tables using Talend.
  - Follow the [Staging Guidelines](docs/staging_guidelines.md) for accurate data loading.

### 3. Preliminary Dimensional Modeling

**Objective**: Design a preliminary dimensional model to structure the data for analysis.

**Procedure**:
- **List Facts & Dimensions**:
  - **Facts**: Collision count, fatality count, collision severity.
  - **Dimensions**: Time (hour, day, week), Location (borough, precinct), Vehicle (type, make), Road User (pedestrian, cyclist, motorist).
- **Create List of Stage Tables’ Columns**:
  - Document the columns from the staging tables.
  - Map each column to the proposed dimensional model.
  - Create an initial schema diagram showing how staging tables map to the dimensional model.

### 4. Data Integration

**Objective**: Load data from staging tables into the integration schema based on the dimensional model.

**Procedure**:
- **Tool**: Use [Talend](https://www.talend.com/) for ETL processes.
- **Database Options**: SQL Server, Azure SQL, MySQL, or Azure SQL.
- **Tasks**:
  - Design ETL workflows to transform and load data into the integration schema.
  - Ensure that data is aligned with the dimensional model and integrity is maintained.

### 5. Query Integration Schema

**Objective**: Query the integration schema to answer specific business questions related to motor vehicle collisions.

**Procedure**:
- **Business Questions**:
  - **Collision Analysis**: Identify top causes of collisions and fatalities.
  - **Time Series Analysis**: Determine collision frequency by time of day, day of the week, and weekdays/weekends.
  - **Fatality Analysis**: Analyze fatality rates among different types of road users.
- **Tasks**:
  - Write and execute SQL queries to extract relevant insights from the integration schema.
  - Document findings and prepare a summary report.

### 6. Business Intelligence Dashboards

**Objective**: Create interactive dashboards to visualize the data and provide insights into collision patterns and fatality analysis.

**Procedure**:
- **Tableau**:
  - Use [Tableau Desktop](https://www.tableau.com/products/desktop) to design dashboards.
  - Publish the dashboards to [Tableau Online](https://www.tableau.com/products/tableau-online) for access and sharing.
- **Power BI**:
  - Use [Power BI Desktop](https://powerbi.microsoft.com/desktop/) to build visualizations.
  - Publish the dashboards to [Power BI Service](https://app.powerbi.com/) for sharing and collaboration.

## Setup Instructions

### Prerequisites

- **Alteryx Designer**: For data profiling.
- **Talend**: For ETL processes.
- **Database**: Choose SQL Server, Azure SQL, MySQL, or Azure SQL for staging and integration.
- **Power BI Desktop**: For creating Power BI dashboards.
- **Tableau Desktop**: For creating Tableau dashboards.

### Steps

1. **Install Required Tools**:
   - Download and install Alteryx Designer, Talend, Power BI Desktop, and Tableau Desktop from their respective websites.

2. **Configure Databases**:
   - Set up your database environment for staging and integration schemas.

3. **Perform Data Profiling**:
   - Use Alteryx to profile the data and document the quality issues.

4. **Load Data into Staging**:
   - Use Talend to load the raw data into staging tables in your chosen database.

5. **Develop Dimensional Model**:
   - Design the preliminary dimensional model and map staging tables to the model.

6. **Data Integration**:
   - Create ETL workflows in Talend to load data from staging into the integration schema.

7. **Query Data**:
   - Write and execute queries to answer business questions from the integration schema.

8. **Create and Publish Dashboards**:
   - Develop dashboards in Power BI and Tableau, and publish them to their respective services.

## Documentation

- [Staging Guidelines](docs/staging_guidelines.md): Guidelines for staging data.
- [Dimensional Model Design](docs/dimensional_model_design.md): Details of the dimensional data model.
- [ETL Workflows](docs/etl_workflows.md): Instructions for using Talend for ETL processes.
- [Power BI Dashboards](docs/powerbi_dashboards.md): Guide to creating and publishing Power BI dashboards.
- [Tableau Dashboards](docs/tableau_dashboards.md): Guide to creating and publishing Tableau dashboards.


## License

This project is licensed under the MIT License. 
