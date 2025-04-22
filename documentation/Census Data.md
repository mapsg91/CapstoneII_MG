---
Note_Type: Dataset
File Type: .xlsx
Source Name: Census
Link: https://www.census.gov/data/tables/
---
# Poverty Change
https://www.census.gov/data/tables/time-series/demo/saipe/change-in-poverty-rates.html
## Variables
  - 'State FIPS' ,'County FIPS' , 'County Name' , 'State Name' ,'Direction of Change'
  - change: 
	  - 'State FIPS': ,'County FIPS': , 'County Name': , 'State Name': ,'Direction of Change':

### Citation:
U.S. Census Bureau, Small Area Income and Poverty Estimates (SAIPE) Program, December 2024, Project No. P-7502872 / Approval CBDRB-FY25-0052

# Gini Index
## Variables
New set: https://api.census.gov/data/2023/acs/acs5?get=NAME,B19083_001E&for=county:*&in=state:*&outputFormat=csv
NAME,B19083_001E,state,count

## clean 
- rename:  'NAME': 'geography', 'B19083_001E': 'gini_index', 'state_fips' , 'county_fips'
- split county and state
- change dtype: 'state_fips': 'str' , 'county_fips': 'str'
- add '00' to beginning of county fips (append)


### Citation
U.S. Census Bureau, U.S. Department of Commerce. "Gini Index of Income Inequality." _American Community Survey, ACS 1-Year Estimates Detailed Tables, Table B19083_, 2023, https://data.census.gov/table/ACSDT1Y2023.B19083?q=B19083&g=010XX00US$0500000_1400000US48201432705&moe=false&tp=true. Accessed on April 16, 2025.

## Poverty rates
http://www.ers.usda.gov/data-products/county-level-data-sets/county-level-data-sets-download-data