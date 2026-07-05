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

# Housing Market Analysis Dashboard

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

The storyboard was created in Tableau to present the housing market analysis in a clear and logical sequence. Each story point focuses on a specific aspect of the dataset, allowing users to explore the relationship between different housing features and sale prices.

The storyboard includes:

- Average Sale Price vs Number of Bedrooms
- Average Sale Price vs Overall Grade
- Average Sale Price vs Flat Area
- Final Housing Market Analysis Dashboard

This sequential approach helps users understand individual trends before viewing the complete dashboard, making the analysis more organized and easier to interpret.
