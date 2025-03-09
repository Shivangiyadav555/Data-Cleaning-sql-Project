# Data-Cleaning-SQL-Project

DATA CLEANING IN MYSQL - LAYOFFS DATASET
This is my first MySQL project, where I performed data cleaning on a dataset related to layoffs. The project focuses on preparing a clean and structured dataset for analysis by addressing common data quality issues.

KEY STEPS PERFORMED:
1.	REMOVING DUPLICATES:
->	Identified and removed duplicate records using ROW_NUMBER() and CTE (Common Table Expressions).
->	Created a staging table to safely handle data modifications.

2.	STANDARDIZING DATA:
->	Trimmed unnecessary spaces from text columns (e.g., company names).
->	Standardized inconsistent values (e.g., updating "crypto" variations to "Crypto").
->  Fixed formatting issues in the date column using STR_TO_DATE() and updated the column data type.

3.	HANDLING NULL/BLANK VALUES:
->	Identified and addressed null or blank values in critical columns like industry.
->	Used self-joins to populate missing industry data based on matching company records.

5.	REMOVING UNNECESSARY COLUMNS:
->	Dropped the temporary row_num column used for duplicate removal.
->	Deleted rows with null values in both total_laid_off and percentage_laid_off columns.
  	
TOOLS USED:
•	MySQL for querying, cleaning, and transforming the dataset.

------  WHAT I LEARNED:
•	Practical techniques for data cleaning and preparation.
•	How to handle duplicates, null values, and inconsistent data.
•	Using SQL functions like ROW_NUMBER(), STR_TO_DATE(), and TRIM() effectively.



