Overview

This Jupyter notebook (Task1.ipynb) documents the data cleaning and preparation process for a sales dataset. 
The dataset contains 2,823 records with 25 columns of sales transaction data, including order details, customer information, and geographic data.

Key Steps Performed:

1. Data Loading and Initial Inspection Loaded the dataset from a CSV file using pandas.
Examined the first few rows to understand the data structure
Checked dataset dimensions (2,823 rows × 25 columns)
Reviewed data types and missing values.

2. Handling Missing Values
Addressed missing values in several columns:
ADDRESSLINE2: Filled with empty strings (since 2,521 of 2,823 values were missing)
STATE: Filled missing values with "Unknown"
POSTALCODE: Filled missing values with the mode (most frequent value)
TERRITORY: Filled missing values with "Not Assigned".


3. Data Type Conversion:
Converted ORDERDATE from string to datetime format for better time-based analysis.

4. Duplicate Check:
Verified there were no duplicate rows in the dataset.

5. Column Standardization:
Standardized column names to lowercase and consistent formatting
Renamed columns for better readability (e.g., ORDERNUMBER → order_number)
Removed the address_line2 column as it contained mostly empty values

6. Final Dataset Structure:
Cleaned dataset contains 2,823 rows and 24 columns
All missing values addressed
Consistent naming conventions applied
Appropriate data types assigned



















