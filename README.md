# 📊 Exploratory Data Analysis (EDA) Portfolio

Welcome to the **Exploratory Data Analysis** repository. This collection serves as a comprehensive portfolio of data analysis projects, demonstrating rigorous techniques in data cleaning, statistical visualization, and insight extraction using the Python ecosystem.

## � Project Structure

```text
EDA--Exploratory-Data-Analysis/
├── EDA 1_Air_Quality_Index/
│   ├── EDA-Air_Quality_Index.ipynb   # Main analysis notebook
│   └── (Dataset files)
├── EDA 2_propertydataset/
│   ├── EDA-propertydataset.ipynb     # Main analysis notebook
│   └── (Dataset files)
└── README.md                         # This documentation
```

## �🔍 Overview
Exploratory Data Analysis is the critical first step in any data science workflow. It involves summarizing the main characteristics of a dataset, often with visual methods. The projects in this repository aim to:
*   **Uncover Patterns**: Detect underlying structures and relationships in complex datasets.
*   **Ensure Quality**: Identify and handle anomalies, outliers, and missing data.
*   **Validate Assumptions**: Test hypotheses before applying predictive modeling.
*   **Inform Strategy**: Provide actionable insights based on historical data.

---

## 📂 Projects

### 1. 🌍 Air Quality Index (AQI) Analysis
*   **Focus**: Environmental Data Science & Public Health
*   **Location**: [`EDA 1_Air_Quality_Index`](EDA%201_Air_Quality_Index/)
*   **Description**: This project investigates urban air quality data, focusing on pollutants like Nitrogen Dioxide ($NO_2$) and Fine Particulate Matter ($PM_{2.5}$). It tracks these levels across different geographic regions and time periods to understand pollution dynamics.
*   **Key Questions Answered**:
    *   Which neighborhoods suffer from the highest pollution levels?
    *   How do pollutant levels correlate with specific time periods (seasonal trends)?
    *   What is the distribution of different air quality indicators?

### 2. 🏠 Property Sales Analysis
*   **Focus**: Real Estate Economics & Market Valuation
*   **Location**: [`EDA 2_propertydataset`](EDA%202_propertydataset/)
*   **Description**: A deep dive into property transactions to understand market valuation. This analysis explores the discrepancy between government-assessed property values and actual market sale prices.
*   **Key Questions Answered**:
    *   How well do assessed values predict actual sale prices?
    *   Which towns have the highest sales ratios (indicating potential undervaluation or overvaluation)?
    *   What are the price distributions for different property types (Residential vs. Commercial)?

---

## 📉 Dataset Specifications

| Feature | Air Quality Dataset | Property Sales Dataset |
| :--- | :--- | :--- |
| **Domain** | Environmental Science | Real Estate |
| **Key Variables** | `Indicator Name`, `Geo Place Name`, `Data Value`, `Time Period` | `Assessed Value`, `Sale Amount`, `Sales Ratio`, `Town` |
| **Data Size** | ~1,000 records | ~10,000 records |
| **Data Types** | Time-series, Categorical, Numerical | Numerical, Categorical, Temporal |
| **Missing Data** | Minimal | Present in `Date Recorded`, `Property Type` |

---

## 🔬 Methodology
Each project follows a structured data science lifecycle:

1.  **Data Ingestion**:
    *   Loading data from CSV/Excel formats using Pandas.
    *   Initial inspection of shape, data types, and sample rows.

2.  **Data Cleaning & Preprocessing**:
    *   **Handling Nulls**: Imputing missing values or removing incomplete records based on impact analysis.
    *   **Type Conversion**: Converting date strings to `datetime` objects for temporal analysis.
    *   **Normalization**: Standardizing column names for consistency.

3.  **Exploratory Analysis (EDA)**:
    *   **Univariate**: Distribution plots (Histograms, KDE) for single variables.
    *   **Bivariate**: Scatter plots and Box plots to compare variables (e.g., *Price vs. Location*).
    *   **Correlation**: Heatmaps to identify linear relationships between numerical features.

4.  **Visualization**:
    *   Using **Matplotlib** and **Seaborn** to create publication-ready charts.
    *   Focus on clear labeling, color-blind friendly palettes, and interpretability.

---

## 🚀 Getting Started

### Prerequisites
*   Python 3.8+
*   Jupyter Notebook or JupyterLab

### Installation
1.  **Clone the repository**:
    ```bash
    git clone <repository-url>
    cd EDA--Exploratory-Data-Analysis
    ```

2.  **Install dependencies**:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```

3.  **Launch the Notebooks**:
    ```bash
    # For Air Quality Analysis
    cd "EDA 1_Air_Quality_Index"
    jupyter notebook EDA-Air_Quality_Index.ipynb

    # For Property Sales Analysis
    cd "../EDA 2_propertydataset"
    jupyter notebook EDA-propertydataset.ipynb
    ```

---

## 🛠️ Technologies Used
*   **Python**: Primary programming language.
*   **Pandas**: Data manipulation and aggregation.
*   **NumPy**: Numerical computing.
*   **Matplotlib**: Static plotting library.
*   **Seaborn**: Statistical data visualization.

---

## 💡 Key Learnings
*   **Real-world Data is Messy**: A significant portion of the project time was dedicated to cleaning data (e.g., handling missing property types or standardizing location names).
*   **Domain Knowledge**: Understanding the difference between "Assessed Value" and "Sale Amount" was crucial for interpreting the real estate data correctly.
*   **The Power of Visualization**: Simple box plots revealed outliers in property sales that summary statistics missed.

## 🔮 Future Improvements
*   **Interactive Dashboards**: Incorporate tools like Plotly or Streamlit for interactive data exploration.
*   **Predictive Modeling**: Build regression models to predict property prices or forecast air quality index.
*   **Geospatial Mapping**: Use Folium or Geopandas to visualize data on actual maps.

---
*Created by [Your Name/Username]*
