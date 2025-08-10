# Loan-Default Dashboard


### Dashboard Link : https://app.powerbi.com/links/P8WQUKdFm0?ctid=36e917dc-1abe-43f4-b189-f92196a6b4ad&pbi_source=linkShare 


## Problem Statement

Financial institutions face significant risks when borrowers fail to repay loans on time. Identifying potential defaulters early is critical to reducing financial losses, optimizing recovery processes, and ensuring long-term profitability.

This dashboard provides a comprehensive view of loan performance, enabling stakeholders to analyze borrower demographics, repayment history, credit scores, and default patterns. By visualizing these factors, the organization can identify high-risk customer segments, monitor portfolio health, and take proactive measures to reduce defaults.

Through dynamic filtering, KPIs, and interactive visuals, the dashboard helps in:

- Detecting trends in default rates across loan types, customer profiles, and regions.

- Analyzing the impact of credit score ranges on default probability.

- Monitoring overdue amounts, recovery percentages, and average repayment delays.




### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : Handled missing values — nulls in Default Date and Credit Score were replaced or removed depending on business logic.
- Step 5 :  Created calculated columns for segmentation, including Income Bracket, Year, Credit Score Bins, and Age Group.
- Step 6 : In the report view, under the view tab, theme was selected.Built three measures tables containing the following DAX measures:
    # Measures Table 1:
        - Average Income by Employment Type

        - Average Loan by Age Group

        - Default Rate by Employment Type

        - Default Rate by Year

        - Loan Amount by Purpose

    # Measures Table 2:
        - Average Loan Amount (High Credit)

        - Loans by Education Type

        - Median by Credit Score Bins

        - Total Loan (Middle Age Group)

        - Total Loan (Credit Bins)

    # Measures Table 3:
        - YOY Default Loan Change

        - YOY Loan Amount Change

        - YTD Loan Amount




# Key Insights

A three page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Loan Default & Income

- There is a positive correlation between Income and Loan Default count.

- Higher income groups still experience defaults, suggesting other influencing factors.
           
### [2] Average Ratings

- High Income borrowers maintain a relatively steady percentage of the total interest rate over time.

- For Low Income groups, interest rates show seasonality. 
  
### [3] Income Bracket Distribution 
  
- High Income accounts for the majority of total income.

- This dominance is consistent across marital statuses like Divorced and Medium credit score bins.

 ### [4] Months Employed & Interest Rate
 
- Notable outliers in the relationship between months employed and interest rate on specific loan dates.

- No significant consistent trend overall.
 
 ### [5] Age Group Analysis
 
- Senior citizens and Middle Age Group have noticeably higher average age values in loans.

- Adults have a relatively steady percentage of the total credit score.
         
### [6] Loan Purpose

For Married individuals, loan purposes show seasonal patterns over the years.

### [7] Credit Score & Employmentl

- There is a positive correlation between Months Employed and Credit Score for high credit score bins.

- Some outliers exist in certain years

### [8] Education & Income
- Education for Adult and Medium Income shows seasonal trends.

- PhD holders maintain a steady percentage of total age distribution.

### [9] Credit Score & Income
- Positive correlation between Income and Credit Score for full-time employees.

- Medium and High credit score bins contribute more income.
 
### [10] Outlier Detection
- Specific dates show anomalies in Months Employed vs. Credit Score and Months Employed vs. Age relationships

### [11] Income by Age Group

- Adult and Middle Age Group contribute the most to total income.

### [12] Interest Rate vs. Age
- For Medium credit score bins, there is a correlation between interest rate and age (slightly negative trend).
