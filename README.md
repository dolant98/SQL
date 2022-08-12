# Business Case Analysis for Prospective Healthcare Employer

## Population Analysis Using SQL 

### Overview

#### Case Study Includes 4 Prompts: 

  - What are the top 3 Practices with the most patients?
  - What NPI & Practice has the highest volume of Diabetic Patients? (Having Diabetes at any point in time)
  - Calculate the Per Member Per Month Paid $ amount of Diabetic Patients vs. Non-Diabetic Patients.
  - Explore the relationship between patient demographic (age, gender, and race_eth) and patient disease with total cost of care. Is there any type of  trend you can identify?
 
#### Three tables provided including the following information: 

  - Total Cost of Care
  - Eligibility Period
  - Practice/Provider Affiliation
  - Conditions (Disease States)
  - Demographics (Age, Race/Ethnicity)
 
### Method of Analysis 
 
  - Data loaded into SQL Server, Queries done using SQL in Azure Data Studio
  - Tables joined, data summarized, and new fields calculated
  - Python used for correlation analysis (Question 4)
  - Tableau used for basic visualization
  - Code and output included in Jupyter Notebook

### Findings

  - 80 Unique Members in subset
    - Distributed across 50 Practices and 4 Lines of Business (LOB)
    - The top 3 practices are located in Long Island and Staten Island
  - Over half (51%) diagnosed with Diabetes with a PMPM 2.5 times greater than members without Diabetes
    - Diabetes PMPM - $2,485
    - No Diabetes PMPM - $961
  - 65% have at least one chronic condition and a PMPM 6x than members without a chronic condition
    - Chronic Condition - $2,433
    - No Chronic Condition - $396

  - By Comparison, the population mean is $1,723
  
  - Initial analysis of the conditions (independent variables) and total cost of care (target) shows: 

    1. Having at least 1 chronic condition contributes to total cost of care
    2. While all conditions have a positive coefficient, CHF and Vascular Disease appear to contribute more to cost
 
  
 
