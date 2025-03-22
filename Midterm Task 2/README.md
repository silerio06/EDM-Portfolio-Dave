### TASK DESCRIPTION ✍🏻

Company X aims to extract valuable insights from the dataset Uncleaned_DS_jobs.csv, which contains job postings from a Kaggle dataset. The focus is on answering key questions:

- Which job roles pay the highest and least?
- What size companies pay the best?
- Where do job roles or job titles pay the best and least in a specific state?

## STEPS AND SCREENSHOTS

## Step 1: Load the Data
- Import the dataset into Power Query Editor.
- Load the raw file
- Fit Column and row width and height
- TRIM extra spaces
- Remove NULL values
- Remove Duplicates
## Step 2: Clean Salary Column
- Remove unnecessary characters and extract Min/Max salary values.
- Salary Estimate Column:
- In Power Query, select the Salary Estimate column.
- Use Transform > Extract > Text Before Delimiter to remove any characters after the open parenthesis.
1. Create Min and Max Salary Columns:
- Use Add Column > Column from Examples to generate the Min Sal and Max Sal columns from the Salary Estimate column.
2. Add Role Type Column.
- Go to Add Column > Custom Column and use the formula to categorize job titles into roles like Data Scientist, Data Analyst, Data Engineer, etc.
3. Split Location Column:
- Select the Location column and use Transform > Split Column by Delimiter (Comma) to split location into separate columns.
4. Location Correction:
- Create a custom column to correct location values, replacing certain locations (e.g., "New Jersey" to ", NJ", "California" to ", CA").
5. Handle Negative Values:
- Filter out negative values in Competitors and Industry columns.
6. Clean Company Name:
- Remove any unwanted text from the Company Name column using Transform > Replace Values or Remove Text
## Step 3: SCREENSHOTS
**Before Data Cleaning: (See screenshot of raw data before any transformations were made.)*
![Uncleaned Data](https://github.com/silerio06/EDM-Portfolio-Dave/blob/main/Midterm%20Task%202/Images/uncleaned.png)

**After Data Cleaning: (Screenshot of cleaned data post-transformation)*
![Cleaned Data](https://github.com/silerio06/EDM-Portfolio-Dave/blob/main/Midterm%20Task%202/Images/cleaned_data.png)

## STEP 4: FINAL OUTPUT QUERIES
**Here are the final queries after performing all the necessary data transformation*
- Sal By Role Type: A query with  job titles categorize by role type
![Sal By Role Type](https://github.com/silerio06/EDM-Portfolio-Dave/blob/main/Midterm%20Task%202/Images/Sal_By_Role_Type.png)

- Sal By Size: A query focusing on salary data by company size or other metric


