---
Note_Type: Dataset
File Type: .csv
Link: https://www.kaggle.com/datasets/valbauman/student-engagement-online-learning-supplement
---
- Split into 'date interval' cycles and use these cycles as sampling distributions for individual counties, states and US as a whole 
# Tables and Columns
## Key Cols for all
1. FIPS
2. County
3. State
4. several codes define city/town size (metro, urban, rural)- use only one metric for this

### General cleaning steps
1. set indexing to state and county 
	1. FIPS?
	[indexing DataFrames](indexing%20DataFrames.md)
2. change datatypes
	1. 'str' : FIPS
	2. 'category': 
		1. UIC_code 
		2. State


## Education
#### Look-up/define
- [Rural-urban Continuum Code](https://www.ers.usda.gov/data-products/rural-urban-continuum-codes/documentation)
- [Urban Influence Code](https://www.ers.usda.gov/data-products/urban-influence-codes/documentation)
### Cleaning Steps
### Dates: 1970-2000 (each decade), 2015-2019
### Vars repeated at  cycle: 
- Less than a high school diploma
- High school diploma only
- Some college (1-3 years)
- Four years of college or higher
- *Percent of adults with less than a high school diploma*
- *Percent of adults with a high school diploma only*
- *Percent of adults completing some college (1-3 years)*
- *Percent of adults completing four years of college or higher*
### Variables
|   |   |
|---|---|
|**Variable**|**Data Type**|
|FIPS Code|int64|
|State|object|
|Area name|object|
|2003 Rural-urban Continuum Code|float64|
|2003 Urban Influence Code|float64|
|2013 Rural-urban Continuum Code|float64|
|2013 Urban Influence Code|float64|
|City/Suburb/Town/Rural 2013|object|
|Less than a high school diploma, ==1970==|object|
|High school diploma only, 1970|object|
|Some college (1-3 years), 1970|object|
|Four years of college or higher, 1970|object|
|Percent of adults with less than a high school diploma, 1970|float64|
|Percent of adults with a high school diploma only, 1970|float64|
|Percent of adults completing some college (1-3 years), 1970|float64|
|Percent of adults completing four years of college or higher, 1970|float64|
|Less than a high school diploma, ==1980==|object|
|High school diploma only, 1980|object|
|Some college (1-3 years), 1980|object|
|Four years of college or higher, 1980|object|
|Percent of adults with less than a high school diploma, 1980|float64|
|Percent of adults with a high school diploma only, 1980|float64|
|Percent of adults completing some college (1-3 years), 1980|float64|
|Percent of adults completing four years of college or higher, 1980|float64|
|Less than a high school diploma, ==1990==|object|
|High school diploma only, 1990|object|
|Some college or associate's degree, 1990|object|
|Bachelor's degree or higher, 1990|object|
|Percent of adults with less than a high school diploma, 1990|float64|
|Percent of adults with a high school diploma only, 1990|float64|
|Percent of adults completing some college or associate's degree, 1990|float64|
|Percent of adults with a bachelor's degree or higher, 1990|float64|
|Less than a high school diploma, ==2000==|object|
|High school diploma only, 2000|object|
|Some college or associate's degree, 2000|object|
|Bachelor's degree or higher, 2000|object|
|Percent of adults with less than a high school diploma, 2000|float64|
|Percent of adults with a high school diploma only, 2000|float64|
|Percent of adults completing some college or associate's degree, 2000|float64|
|Percent of adults with a bachelor's degree or higher, 2000|float64|
|Less than a high school diploma, ==2015-19==|object|
|High school diploma only, 2015-19|object|
|Some college or associate's degree, 2015-19|object|
|Bachelor's degree or higher, 2015-19|object|
|Percent of adults with less than a high school diploma, 2015-19|float64|
|Percent of adults with a high school diploma only, 2015-19|float64|
|Percent of adults completing some college or associate's degree, 2015-19|float64|
|Percent of adults with a bachelor's degree or higher, 2015-19|float64|
## Unemployment
### Dates:
Original: 2003-2020 
Updated: - 2023
cycle: annual 
Vars per cycle:
- Civilian_labor_force
- Employed
- Unemployed
- *Percents*...

2019 only: 
- Median_Household_Income_2019
- Med_HH_Income_Percent_of_State_Total_2019
### Cleaning Steps
1. delete all 'percent' cols
2. split  'area_name' by comma
3. rename area_name to 'county'

### Variables
|   |   |
|---|---|
|**Variable**|**Data Type**|
|FIPS_Code|int64|
|State|object|
|Area_name|object|
|Rural_urban_continuum_code_2013|float64|
|Urban_influence_code_2013|float64|
|City/Suburb/Town/Rural|object|
|Metro_2013|float64|
|Civilian_labor_force_2000|object|
|Employed_==2000==|object|
|Unemployed_2000|object|
|Unemployment_rate_2000|float64|
|Civilian_labor_force_2001|object|
|Employed_==2001==|object|
|Unemployed_2001|object|
|Unemployment_rate_2001|float64|
|Civilian_labor_force_==2002==|object|
|Employed_2002|object|
|Unemployed_2002|object|
|Unemployment_rate_2002|float64|
|Civilian_labor_force_==2003==|object|
|Employed_2003|object|
|Unemployed_2003|object|
|Unemployment_rate_2003|float64|
|Civilian_labor_force_==2004==|object|
|Employed_2004|object|
|Unemployed_2004|object|
|Unemployment_rate_2004|float64|
|Civilian_labor_force_==2005==|object|
|Employed_2005|object|
|Unemployed_2005|object|
|Unemployment_rate_2005|float64|
|Civilian_labor_force==_2006==|object|
|Employed_2006|object|
|Unemployed_2006|object|
|Unemployment_rate_2006|float64|
|Civilian_labor_force_==2007|==object|
|Employed_2007|object|
|Unemployed_2007|object|
|Unemployment_rate_2007|float64|
|Civilian_labor_force_==2008==|object|
|Employed_2008|object|
|Unemployed_2008|object|
|Unemployment_rate_2008|float64|
|Civilian_labor_force_2009|object|
|Employed_2009|object|
|Unemployed_2009|object|
|Unemployment_rate_2009|float64|
|Civilian_labor_force_2010|object|
|Employed_2010|object|
|Unemployed_2010|object|
|Unemployment_rate_2010|float64|
|Civilian_labor_force_2011|object|
|Employed_2011|object|
|Unemployed_2011|object|
|Unemployment_rate_2011|float64|
|Civilian_labor_force_2012|object|
|Employed_2012|object|
|Unemployed_2012|object|
|Unemployment_rate_2012|float64|
|Civilian_labor_force_2013|object|
|Employed_2013|object|
|Unemployed_2013|object|
|Unemployment_rate_2013|float64|
|Civilian_labor_force_2014|object|
|Employed_2014|object|
|Unemployed_2014|object|
|Unemployment_rate_2014|float64|
|Civilian_labor_force_2015|object|
|Employed_2015|object|
|Unemployed_2015|object|
|Unemployment_rate_2015|float64|
|Civilian_labor_force_2016|object|
|Employed_2016|object|
|Unemployed_2016|object|
|Unemployment_rate_2016|float64|
|Civilian_labor_force_2017|object|
|Employed_2017|object|
|Unemployed_2017|object|
|Unemployment_rate_2017|float64|
|Civilian_labor_force_2018|object|
|Employed_2018|object|
|Unemployed_2018|object|
|Unemployment_rate_2018|float64|
|Civilian_labor_force_2019|object|
|Employed_2019|object|
|Unemployed_2019|object|
|Unemployment_rate_2019|float64|
|Civilian_labor_force_==2020==|object|
|Employed_2020|object|
|Unemployed_2020|object|
|Unemployment_rate_2020|float64|
|Median_Household_Income_2019|object|
|Med_HH_Income_Percent_of_State_Total_2019|float64|
## UIC Codes
### Cleaning Steps
### Variables
|   |   |
|---|---|
|**Variable**|**Data Type**|
|FIPS|int64|
|State|object|
|County_Name|object|
|Population_2010|object|
|UIC_2013|int64|
|Description|object|
|City/Suburb/Town/Rural|object|
### Var definitions/notes
- 'UIC_2013'  corresponds to category described in 'Description'
- City/Suburb/Town/Rural- categorical to column name items
## Citation:
### unemployment rate and education level data by county:
kaggle: "County-level Data Sets." USDA Economic Research Service, US Department of Agriculture. Access date: Sept 8, 2021. URL: https://www.ers.usda.gov/data-products/county-level-data-sets/

most recent: 
U.S. Department of Agriculture, Economic Research Service. (2025, January 31). _County-level data sets_.

### Urban Influence Codes by county:  
"Urban Influence Codes." USDA Economic Research Service, US Department of Agriculture. Access date: Sept 8, 2021. URL: https://www.ers.usda.gov/data-products/urban-influence-codes/#:~:text=The%202013%20Urban%20Influence%20Codes,to%20metro%20and%20micropolitan%20areas.&text=An%20update%20of%20the%20Urban,is%20planned%20for%20mid%2D2023