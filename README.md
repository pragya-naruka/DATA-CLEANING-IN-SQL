# Data Cleaning with SQL - Layoffs 2022 Project

## Project Overview
This project is focused on cleaning and transforming a dataset containing global layoffs data from 2022, sourced from Kaggle. The dataset includes details such as company name, industry, total employees laid off, percentage of layoffs, date, and other related fields.

In this project, we use SQL techniques to:
1. **Remove duplicates** to ensure data integrity.
2. **Standardize and correct data** in fields such as industry, country, and date formats.
3. **Handle null values** and decide which should be filled or remain.
4. **Clean and drop unnecessary rows and columns** to refine the dataset for further analysis.

## Dataset
The dataset used for this project can be found on Kaggle: [Layoffs 2022 Dataset](https://www.kaggle.com/datasets/swaptr/layoffs-2022).

## Key Steps
1. **Create a staging table** to preserve the raw data for reference and experimentation.
2. **Identify and remove duplicate entries** by creating a row number partition.
3. **Standardize data** fields like `industry`, `country`, and `date` to ensure consistency across the dataset.
4. **Fix null values** by checking for empty fields and filling them where appropriate.
5. **Drop columns and rows** that are irrelevant or have incomplete data (e.g., rows with nulls in key fields like `total_laid_off` and `percentage_laid_off`).

## Key SQL Operations
- `ROW_NUMBER()` for identifying duplicate rows.
- `JOIN` and `UPDATE` to fill missing values based on other rows in the dataset.
- `TRIM` to standardize text fields (e.g., removing trailing periods).
- `STR_TO_DATE` to convert text date fields into the proper date format.

This project serves as an introduction to core SQL data cleaning techniques, ensuring the dataset is clean, consistent, and ready for analysis.
