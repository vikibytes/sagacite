## Character Development for your Data Story

- Tools are great but elementary principles are crucial
- Data Cleaning - Good Investment
- Data Management
    - Keep a backup of raw Data
    - Make a note of any transformations done to Data, missing variables etc (Data Changes Doc)
    - the goal is reproducibility
- 10 basic steps to clean Data
    1. Reformat or reshape the data, 
        - remove metadata rows from Excel
        - check if data is in tidy format. (first row columns and others rows are individual data points)

    2. What data in in each column
        - What type (numeric / non-numeric)

    3. Numeric Data
        - format numeric data in Excel (both floats and integers) so that other tools detect it easily.

    4. Non-numeric variables
        - Use the Data -> Text To Columns feature to separate out text data to multiple columns
        - Note: record these transforms in your Data Changes Doc

    5. Look at Dates in your data 
        - Make sure all the dates are in a standard format. 
        - Use Python or R or other tools if required to make this task easy

    6. Missing Data  
        - Check what type of 'missingness'
        - Change data accordingly to type of 'missingness'

    7. Not Applicable Data
        - 'Not Applicable' vs 'Missing' 
        - Change 'Not Applicable' data to NULL or equivalent.

    8. Make sure words are spelled consistently. (for factors)
        - Things like names of places / things etc.
        - Fix for slight variations in spellings (most probably in free-form entries)

    9. Units of measurement for numeric variables
        - Make sure they are consistent
        - Standardize across different units (e.g., convert all currency to USD etc..)

    10. Check for impossible / unlikely values
        - Remove impossible values
        - If unlikely values, try to find out if it is just an outlier or plain wrong