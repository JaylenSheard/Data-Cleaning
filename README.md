# Data-Cleaning Repository 🗑️

## Overview

This repository is dedicated to projects focused on data cleaning. The primary goal is to clean and prepare datasets for further analysis, visualization, or modeling. Data cleaning is a critical step in the data science pipeline, ensuring that the data is accurate, consistent, and usable for analysis.

## Project 1: Financial Data Cleaning

### Description

The first project in this repository involves cleaning a financial dataset. The dataset includes various financial metrics such as sales, costs, and profits, along with dates and other relevant information. The goal was to clean the data to make it ready for analysis.

### Key Steps:

1. **Data Loading and Inspection**:
    - The dataset was loaded using Pandas, and an initial inspection was conducted to understand its structure and content.

2. **Cleaning Column Names**:
    - Whitespace was removed from column names to ensure consistency and avoid issues in further analysis.

3. **Data Transformation**:
    - Values in parentheses, typically representing negative numbers, were converted to their correct numerical form.
    - Unwanted characters like dollar signs and commas were removed from the dataset.

4. **Handling Missing Values**:
    - Missing values in the `Profit` column were filled by calculating the difference between `COGS` (Cost of Goods Sold) and `Sales`.
    - Missing values in the `Discounts` column were replaced with zeroes.

5. **Data Type Conversion**:
    - The `Date` column was converted from string format to datetime format to facilitate time series analysis.

6. **Dropping Unnecessary Columns**:
    - Columns like `Month Number`, `Month Name`, and `Year` were dropped as they were redundant or not needed for the analysis.

7. **Exporting Cleaned Data**:
    - The cleaned dataset was saved as a CSV file for further use.

### Tools and Libraries

- **Pandas**: Used for data manipulation and cleaning.
- **NumPy**: Used for numerical operations and handling missing values.

### Usage

You can run the Jupyter notebook file `Finacials_Cleaned.ipynb` to reproduce the cleaning process. The cleaned dataset is saved as `Financials_Cleaned.csv` and can be used for subsequent analysis.

## Future Projects

This repository will be expanded with more data cleaning projects. Each project will involve different datasets and will showcase various data cleaning techniques.
