# ID Variables
# Dataset Vars to selectss
## Gini index
1. gini_index
## QOL
2.'2020PopulrVoteParty': 'political_party', 'Cost of Living':'cost_of_living'; '2022 Median Income': 'median_income', 'Diversity Rank (Race)', 'Diversity Rank (Gender)', 'NMCNTY':'county, 'FIPS':'fips', 'LSTATE':'state_abbr'

    a. clean col and median income: remove '$' and ','
    b. create col_to_income_ratio = 'cost_of_living'/'median_income'
## County rankings
1. 'fips', 'county', 'state_abbr', 'hs_diploma_percentage',
       'unemployed_percentage', 'population', 'median_income',
       'school_segration_index', 'gender_pay_gap', 'uninsured__percentage',
       'school_funding_gap', 'residential_segregation', 'premature_death',
       'income_inequality', 'child_poverty_percentage', 'life_expectancy',
       'child_mortality', 'high_housing_cost_percentage', 'firearm_fatalities',
       'child_care_cost_burden'

# Socioeconomic markers