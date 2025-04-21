# Task 1: Data Cleaning and Preprocessing - Superstore Sales Dataset

## Overview:
This project focuses on data cleaning and preprocessing of the **Superstore Sales Dataset**. The objective was to clean the dataset by handling missing values, standardizing text, formatting dates, and ensuring consistent data types. The dataset was cleaned using **Power Query** in Excel to make it suitable for analysis.

### 1. **Handling Missing Values in Postal Code**:
   - The postal code column had some missing values. I used **Power Query** to create a custom column and added a missing "0" in front of postal codes that were 4 digits long. The formula used in Power Query was:
     ```powerquery
     = if Text.Length([Postal Code]) = 4 then "0" & [Postal Code] else [Postal Code]
     ```
   - This ensured that all postal codes were in the correct format.

### 2. **Converting Date Formats**:
   - I standardized the date formats to a consistent **dd-mm-yyyy** format for uniformity, ensuring the dataset can be used effectively for time-based analysis.

### 3. **Renaming Column Headers**:
   - Column headers were inconsistent, so I renamed them to be uniform and easy to work with. This included:
     - Converting all column names to lowercase.
     - Removing spaces and special characters for cleaner names.

### 4. **Checking and Fixing Data Types**:
   - I verified and corrected the data types for each column to ensure that:
     - Date columns were recognized as **Date** type.
     - Numeric columns were set as **Number** type.
     - Text columns were recognized as **Text** type.

## What I Learned:
   - **Power Query**: Learned how to clean data, handle missing values, and automate the process of data transformation using Power Query.
   - **Text Handling**: Learned to standardize text values for consistency and better data handling.
   - **Data Formatting**: Ensured consistent date formats and fixed data types to make the dataset easier to analyze.
   - **Handling Missing Data**: Gained experience in handling missing data, such as adding leading "0"s to postal codes.
