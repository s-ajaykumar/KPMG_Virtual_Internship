# KPMG_Virtual_Internship
### Goal:
	To recommend which of these 1000 new customers should be targeted to drive the most value for the organization.
## Scope
| **Activity** | **Description** |
| -------- | ----------- |
| Ask	   | Asking SMART questions to understand the context of the project |
| Prepare  | Collecting and organizing the data for ease of access. |
| Process  | Cleaning the data for accurate predictions. |
| Analyze  | Performing sorting, filtering and statistics to analyze data. |
| Share    | Sharing the insights to the client in the form of visualizations. |
| Act      | Making recommendations for effective data driven decisions. |

## Ask

- I try to understand the overall context of business requirements.
- Used SMART strategy.

	- S - Specific
	- M - Measurable
	- A - Action oriented
	- R - Relevant
	- T - Time bound

### Qns:

- To determine who provides the most value, we need to know each new customer’s value.
 But we don't have any prior transactions with the new customers.
- So, how can we determine which customers to target?
### Soln:
- The common data between the old customers database and the new customers database are age, past_3_years_bike_related_purchases, job_title, job_industry_category, wealth_segment,  owns_car, tenure, postcode, country, state.
- So if we find which segment customers in the old customers list provides more value then based on that we can achieve our goal.

## Prepare
- What is the data?
- How to collect it?
- How much data do I need?
- Whether ROCCC rule need to be applied?
- Data security
- Data organization and convention

## Process

### My checklist:

- Change the entire columns into uppercase
- Duplicates
- Whitespace
- Empty cells
- Standardize the column formats
- Outliers
- Unmerge
- Merge
- Cross field validation
- Change units of measurement

### Change Log
#### Transactions table:

- Removed the rows where there are  empty cells in the  online_order column.
- Removed the rows where there are  empty cells in the brand column.
- 915 duplicate values found and removed.
- Splitted transaction_date column into transaction _month and transaction_date columns.

#### New Customer List table
- New customer list table:
- Removed the rows where there are empty cells in the DOB column.
- Removed the rows where there are empty cells in the job_title column.
- Removed the rows where there are n/a values in the job_industry_category column.
- The word Argiculture was replaced with Agriculture in the job_industry_category_column.
- The values in the postcode column are in the form of text so converted them into number format.
- The values in the property value column are in the form of text so converted them into number format.
- Merged the first name and second name column into a single column name.
- The values in the column past_3_years_bike_related_purchases were in text format therefore converted them into number format.
- Added a column age using datedif function.

#### Customer Demographic table
- Merged the first_name and second_name column into single column name.
- Replaced M with male and F with female in the column gender.
- The column DOB contained a wrong value 1843-12-21 therefore changed into 1943-12-21
- Removed the rows where there are empty cells in the job_title column.
- Removed the rows where there are n/a values in the job_industry_category column.
- The word Argiculture was replaced with Agriculture in the job_industry_category_column.
- Removed the rows where there are empty cells in the tenure column.

#### Customer address table:
- Replaced NSW with New South Wales and VIC with Victoria in the state column.

#### Merged tables:
- Merged customer demographic table, customer address table, transactions table into a single table called Old_Customer table

#### Categorization:
- Categorized the age column  into 10 categories like 20 - 29, 30 - 39 up to 90 - 99.

## Analyze
- Analyze using Excel.
- #### Operations:
 - Organize
 - Filter
 - Sort
 - Getting feedback from others
 - Calculations (Pivot table)


















