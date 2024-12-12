# Analysis-on-Motor-Theft-in-Toronto-neighbourhoods

## Introduction
This project focuses on analyzing and predicting motor vehicle theft incidents in Toronto. Using open data from the Toronto Police Service, we aim to provide insights into crime patterns and develop predictive models to forecast future thefts, enabling better resource allocation for law enforcement and improved crime prevention strategies.

## Objectives
1. Aggregate and analyze motor theft incidents over time and by location.
2. Develop a 28-day trailing theft count for predictive modeling.
3. Build a regression model to forecast the trailing 28-day theft count at specific locations.

## Dataset
The dataset includes records of motor vehicle thefts in Toronto, sourced from the Toronto Police Service Open Data Portal. Key features include:
- **Location Data**: Longitude and latitude coordinates.
- **Temporal Data**: Report and occurrence dates, hours, and days of the week.
- **Categorical Features**: Location type, premises type, and neighborhood identifiers.

### Data Highlights
- Total records: 96,276 incidents
- Time range: 2014–2024
- Missing values handled for geographic and temporal features.

## Methodology
1. **Data Preprocessing**:
   - Converted dates to datetime format for easier manipulation.
   - Grouped data by location and computed trailing 28-day theft counts.
   - Addressed missing values and aligned data for time-series analysis.

2. **Exploratory Data Analysis (EDA)**:
   - Visualized daily and 28-day theft trends to uncover long-term patterns.
   - Conducted autocorrelation and seasonal decomposition to analyze temporal trends.

3. **Predictive Modeling**:
   - Trained a linear regression model using the following features:
     - Geographic coordinates (longitude and latitude).
     - Temporal data (year, month, day of the week).
   - Evaluated model performance using Mean Squared Error (MSE) and R² metrics.

## Key Findings
1. Motor vehicle theft incidents showed a notable peak in 2020, followed by a decline in recent years (2023–2024).
2. Long-term trends indicate fluctuations in theft rates influenced by broader socioeconomic factors, such as the COVID-19 pandemic.
3. The linear regression model demonstrated limited predictive accuracy, with:
   - **Mean Squared Error (MSE)**: 74.76
   - **R² Score**: 0.12

## Results
- Temporal analysis highlighted significant variations in theft incidents, with no consistent seasonal cycle.
- The regression model showed that geographic and temporal features partially explain theft trends but may require additional variables for better accuracy.
