# COVID-19 Cases Analysis (2020-2023) - Power BI Project

## Project Overview
This Power BI project involved analyzing global COVID-19 case data from 2020 to 2023. The goal was to visualize the spread and growth of COVID-19 cases, providing insights into cumulative and daily growth rates across different countries and time periods.

## Objectives
- Analyze trends in cumulative COVID-19 cases over time.
- Visualize daily growth rates and identify significant changes.
- Provide an interactive dashboard for exploring data by country and date.

## Data Sources
- **Primary Data Source:** COVID-19 case data (daily reports).
- **Data Transformation:** Cleaned and transformed using Power Query in Power BI.

## Data Model
The data model was designed using a star schema:
- **Fact Table:** `FactCovid19Cases`
  - Fields: `Case-cumulation`, `KeyCountry`, `KeyDate`
- **Dimension Tables:**
  - `DimDate`: Date, Day, DayNumberOfMonth
  - `DimCountry`: Country, KeyCountry

### Relationships
- `FactCovid19Cases[KeyDate]` -> `DimDate[KeyDate]`
- `FactCovid19Cases[KeyCountry]` -> `DimCountry[KeyCountry]`

## DAX Measures
Custom DAX measures were created for:
- **MTD Total Cases**
- **YTD Total Cases**
- **Total Daily Cases**
- **Non-Cumulative Cases**

## Dashboard and Visualizations
The dashboard consists of:
1. **Cumulative Cases Over Time** - A line chart showing the total cases growth from 2020 to 2023.
2. **Daily Growth Rate** - A line chart displaying daily changes in case numbers.
3. **Interactive Filters** - Slicers for country and date range selection.

## Key Insights
- **Peak Periods:** The visualizations highlight significant peaks in case numbers, indicating waves of the pandemic.
- **Growth Rate Trends:** The daily growth rate analysis reveals how quickly the virus spread during different phases.
- **Regional Analysis:** Country-specific filtering allows for localized trend analysis.

## Conclusion
This project demonstrates proficiency in:
- **Data Modeling:** Creating relationships between fact and dimension tables.
- **DAX:** Developing measures for time-based calculations.
- **Data Visualization:** Designing interactive and insightful dashboards.

For any inquiries or further discussion about this project, please feel free to contact me.

