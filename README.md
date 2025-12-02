# Exploratory Data Analysis - Air Quality Index (AQI)

## Overview
This project conducts an Exploratory Data Analysis (AQI) on an Air Quality dataset. It focuses on analyzing various air quality indicators, such as Nitrogen Dioxide (NO2) and Fine Particles (PM 2.5), across different geographic locations and time periods.

## Dataset
The dataset includes the following key columns:
-   **Unique ID**: Unique identifier for each data point.
-   **Indicator ID**: ID representing the specific air quality indicator.
-   **Name**: Name of the air quality indicator (e.g., Nitrogen dioxide (NO2), Fine particles (PM 2.5)).
-   **Measure**: The unit of measurement (e.g., Mean).
-   **Measure Info**: Additional information about the measurement (e.g., ppb).
-   **Geo Type Name**: The type of geographic area (e.g., UHF42).
-   **Geo Join ID**: ID used for joining geographic data.
-   **Geo Place Name**: Name of the specific place or neighborhood (e.g., Jamaica and Hollis).
-   **Time Period**: The time period the data represents (e.g., Annual Average 2017).
-   **Start_Date**: The start date of the data collection period.
-   **Data Value**: The recorded value for the indicator.

## Analysis Steps
The Jupyter Notebook (`EDA-Air_Quality_Index.ipynb`) covers the following steps:

1.  **Data Loading and Cleaning**:
    -   Importing the dataset and inspecting column data types.
    -   Checking for and handling missing values.

2.  **Descriptive Statistics**:
    -   Calculating mean, standard deviation, min, and max for the `Data Value` column.
    -   Identifying the most frequent indicators and geographic locations.

3.  **Data Visualization and Exploration**:
    -   **Indicator Analysis**: Comparing the average data values for different air quality indicators.
    -   **Geographic Analysis**: Identifying locations with the highest and lowest air quality values.
    -   **Temporal Trends**: Analyzing how air quality indicators change over different time periods.

## Key Insights
-   The dataset tracks multiple pollutants, with **Nitrogen dioxide (NO2)** and **Fine particles (PM 2.5)** being among the most frequent indicators.
-   Analysis reveals variations in air quality across different neighborhoods (e.g., East Harlem, Manhattan).
-   The data allows for the identification of areas with potential air quality issues based on high indicator values.

## Requirements
To run this analysis, ensure you have the following installed:
-   pandas
-   numpy
-   matplotlib
-   seaborn

## Usage
Run the `EDA-Air_Quality_Index.ipynb` notebook to reproduce the analysis and view the generated plots.

# Exploratory Data Analysis - Property Dataset

## Overview
This project performs an Exploratory Data Analysis (EDA) on a property sales dataset. The goal is to understand the characteristics of property sales, including assessed values, sale amounts, and sales ratios across different towns and property types.

## Dataset
The dataset contains the following columns:
- **Serial Number**: Unique identifier for the record.
- **List Year**: The year the property was listed.
- **Date Recorded**: The date the sale was recorded.
- **Town**: The town where the property is located.
- **Address**: The address of the property.
- **Assessed Value**: The value of the property as assessed for tax purposes.
- **Sale Amount**: The amount the property was sold for.
- **Sales Ratio**: The ratio of the Assessed Value to the Sale Amount.
- **Property Type**: The category of the property (e.g., Residential, Commercial).
- **Residential Type**: Specific type of residential property (e.g., Single Family, Condo).

## Analysis Steps
The analysis in the Jupyter Notebook (`EDA-propertydataset.ipynb`) includes:

1.  **Data Loading and Inspection**:
    -   Loading the dataset and checking for data types and missing values.
    -   Summary statistics to understand the distribution of numerical features.

2.  **Data Cleaning**:
    -   Handling missing values in columns like `Date Recorded`, `Property Type`, and `Residential Type`.
    -   Converting date columns to appropriate datetime formats.

3.  **Exploratory Data Analysis**:
    -   **Correlation Analysis**: Calculating and visualizing the correlation matrix to understand relationships between numerical variables (e.g., Assessed Value vs. Sale Amount).
    -   **Distribution Analysis**: Using histograms and boxplots to visualize the distribution of Sale Amounts and Assessed Values.
    -   **Categorical Analysis**: Analyzing the frequency of sales by Town and Property Type.
    -   **Time Series Trends**: Examining sales trends over the years.

## Key Findings
-   There is a positive correlation between `Assessed Value` and `Sale Amount`, as expected.
-   The `Sales Ratio` provides insight into how properties are valued relative to their market price.
-   The dataset covers various towns, allowing for geographic comparison of real estate markets.

## Requirements
To run the notebook, you need the following Python libraries:
-   pandas
-   numpy
-   matplotlib
-   seaborn

## Usage
Open `EDA-propertydataset.ipynb` in Jupyter Notebook or JupyterLab to view the code and visualizations.