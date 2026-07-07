# Housing-Market-Analysis


# Housing Market Analysis using Tableau

## 📌 Project Overview

This project analyzes housing market data using Tableau to identify trends and relationships between property features and sale prices. The workflow includes data collection, data cleaning, dashboard creation, and interactive storytelling.

---

## 📂 Dataset Collection

- Downloaded the housing dataset from Kaggle/provided source.
- Stored the dataset locally for easy access.
- Verified the dataset format (CSV) and ensured data integrity before analysis.

---

## 📥 Loading the Dataset

- Imported the dataset into Tableau.
- Verified column names and data types using the **Data Source** tab.
- Checked for missing values and formatting inconsistencies before visualization.

---

## 🧹 Data Cleaning

The dataset was preprocessed using **Python (Pandas & NumPy)** before importing it into Tableau.

### Cleaning Steps

- Removed missing values.
- Removed duplicate records.
- Standardized column names.
- Checked for outliers using boxplots.
- Exported the cleaned dataset as **housing_data_cleaned.csv**.

### Technologies Used

- Python
- Pandas
- NumPy
- Tableau

### Sample Code

```python
import pandas as pd

# Load dataset
df = pd.read_csv("housing_data.csv")

# Handle missing values
df = df.dropna()

# Remove duplicate records
df = df.drop_duplicates()

# Standardize column names
df.columns = (
    df.columns
      .str.strip()
      .str.lower()
      .str.replace(" ", "_")
)

# Save cleaned dataset
df.to_csv("housing_data_cleaned.csv", index=False)
```

---





## 📊 Project Workflow

1. Dataset Collection
2. Data Loading
3. Data Cleaning
4. Dashboard Development
5. Storyboard Design
6. Data Visualization & Analysis


# Tableau Data Visualization Project



### Technical Framework & Overview

This project documentation explains the three Tableau sheets created in the workbook. The project analyzes core business parameters of a Real Estate Housing Dataset by balancing Dimensions and Measures while following an optimized workflow.

**Technology**
- Tableau Desktop / Tableau Public (Version 2026.1)

**Data Source**
- Real Estate Housing Dataset (Structured Fields)

**Core Methodology**
- Discrete Dimension Mapping
- Measure Aggregations
- Custom Marks Card Formatting
- Interactive Subset Filtering

---

#  Distribution of House Age by Renovation Status

## Description & Purpose

The objective of this sheet is to analyze the distribution of houses across different age groups and identify properties with an active renovation status. A pie chart is used to clearly visualize the proportional distribution.

### Fields Used
- Age of House (in Years)
- SUM(Ever Renovated Yes)

### Implementation Steps

1. Changed the visualization type to **Pie Chart**.
2. Converted **Age of House (in Years)** into a **Discrete Dimension** and placed it on the **Color** shelf.
3. Added the same field to the **Label** shelf to display age values.
4. Added **SUM(Ever Renovated Yes)** to both **Angle** and **Size** shelves.
5. Applied filters using the **Age of House** field for better data control.

---

# House Age Distribution by Number of Bathrooms, Bedrooms, and Floors

## Description & Purpose

This sheet compares major architectural metrics such as bedrooms, bathrooms, and floors across different house age groups using a grouped bar chart.

### Fields Used
- Age of House (in Years)
- Measure Names
- Measure Values

### Implementation Steps

1. Added **Age of House (in Years)** to the **Columns** shelf as a discrete field.
2. Added **Measure Names** beside it on the Columns shelf.
3. Placed **Measure Values** on the **Rows** shelf.
4. Retained only:
   - SUM(No of Bathrooms)
   - SUM(No of Bedrooms)
   - SUM(No of Floors)
5. Applied **Measure Names** to the **Color** shelf.
6. Added filters to improve chart readability and formatting.

---

# Price Distribution by Zipcode

## Description & Purpose

This visualization analyzes property prices across different zip codes to identify location-based pricing trends.

### Fields Used
- Zipcode
- SUM(Price)

### Implementation Steps

1. Added **Zipcode** to the geographic axis.
2. Added **SUM(Price)** to the **Rows** shelf.
3. Optimized the visualization using the **Marks Card**.
4. Changed the worksheet display from **Standard** to **Entire View** for maximum visibility.

---

# Analytical Summary

The project applies Tableau visualization best practices across all three sheets. Every worksheet is optimized using **Entire View**, ensuring better space utilization and readability. Discrete color mapping, proper data labeling, and interactive filtering improve the overall analytical experience and make the visualizations clear, accurate, and professional.



# Housing Market Analysis Dashboard


## Tableau URL:- https://public.tableau.com/app/profile/siddhi.mishra5827/viz/Dashboard_tableau_17832458807500/Dashboard1?publish=yes

## Project Overview
This project presents an interactive Tableau dashboard to analyze housing market trends using cleaned housing data.

## Dashboard Features
- Average Sale Price by Overall Grade
- Flat Area vs Sale Price (Scatter Plot)
- Average Sale Price by Number of Bedrooms

## Tools Used
- Tableau Public
- Excel (Data Cleaning)
- GitHub

## Key Insights
- Higher overall grades generally have higher average sale prices.
- Larger flat areas are associated with higher sale prices.
- Houses with more bedrooms generally have higher average sale prices.

## 📖 Storyboard


##Tableau URL:- **Provided in demo link**


The storyboard was created in Tableau to present the housing market analysis in a clear and logical sequence. Each story point focuses on a specific aspect of the dataset, allowing users to explore the relationship between different housing features and sale prices.

The storyboard includes:

- Average Sale Price vs Number of Bedrooms
- Average Sale Price vs Overall Grade
- Average Sale Price vs Flat Area
- Final Housing Market Analysis Dashboard

This sequential approach helps users understand individual trends before viewing the complete dashboard, making the analysis more organized and easier to interpret.




## 📊 Performance Testing – Amount of Data Loaded

The **Amount of Data Loaded** test was performed to verify that the housing dataset was successfully imported into Tableau and was ready for analysis. The cleaned dataset was loaded without any errors, and Tableau correctly recognized all available fields and records.

The successful loading of the dataset ensured that the data was available for creating worksheets, dashboards, and storyboards. A preview of the imported data confirmed that the required rows and columns were accessible for further visualization and analysis.

### Results

- **Dataset:** Cleaned_Housing_Data.csv
- **Rows Loaded:** 10,000
- **Fields Loaded:** 32
- **Loading Status:** Successfully Loaded
- **Performance:** Passed

> **Note:** The dataset was successfully loaded into Tableau and validated using the Data Source preview before proceeding with dashboard and storyboard development.



## 🔍 Performance Testing – Utilization of Filters

Interactive filters were implemented in the Tableau dashboard to improve data exploration. Users can filter housing data based on the **Number of Bedrooms**, allowing the dashboard to dynamically update and display only the relevant records. The filtering functionality responded correctly and enhanced the overall usability of the dashboard.

### Results

- Filter Applied: Number of Bedrooms
- Dashboard Response: Dynamic
- Data Updated Successfully
- Performance: Passed





**overall documentation file is provided **

