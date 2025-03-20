### TASK DESCRIPTION ✍🏻

Company X aims to extract valuable insights from the dataset Uncleaned_DS_jobs.csv, which contains job postings from a Kaggle dataset. The focus is on answering key questions:

- Which job roles pay the highest and least?
- What size companies pay the best?
- Where do job roles or job titles pay the best and least in a specific state?

### DATASET BEFORE CLEANING AND TRANSFORMATION
![Clean Data](https://github.com/silerio06/EDM-Portfolio-Dave/blob/main/Midterm%20Task%202/Images/RAW_DATA.png)

## STEPS AND
# Step 1: Load the Data
- Import the dataset into Power Query Editor.
# Step 2: Clean Salary Column
- Remove unnecessary characters and extract Min/Max salary values.
# Step 3: Categorize Job Roles
- Group job titles into predefined categories such as Data Scientist, Data Analyst, etc.# 
# Step 4: Split Location Column
- Extract state abbreviations for consistency in location data.
# Step 5: Fix Data Issues
- Replace incorrect values, remove duplicates, and clean company names.
# Step 6: Split Company Size
- Separate min and max company size values for better analysis.
# Step 7: Handle Negative Values
- Filter and replace missing or incorrect data (e.g., -1 values in competitors and industry columns).
# Step 8: Remove Unneeded Columns
- Drop descriptions and redundant fields to keep relevant data.
# Step 9: Group Data
- Summarize salary data by job role, company size, and state.
# Step 10: Map State Names
- Merge with external data to add full state names.
# Step 11: Verify Query Dependencies
- Ensure all queries and transformations are correct and properly linked.

