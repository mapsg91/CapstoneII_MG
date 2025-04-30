# Overview
The ongoing joke amongst young and young-ish adults (under 40) is that we will never own a home, regardless of our level of education or promising job history. Reaching financial milestones such as homeownership, at least for the "middle class" seem further and farther away with a growing gap between home costs and median household incomes (Home Price-to-Income Ratio Reaches Record High | Joint Center for Housing Studies), resulting in a record number of young adults moving back into their childhood homes (Cole). The problem might not be avocado toast, as some billionaires of a foregone era might claim. 
	Though innumerable socio-economic factors shape these realities; a notable backdrop is the ever-growing wealth gap (NCRC) and regress in upward mobility (Manduca et al.). Given these socioeconomic trends are well-documented, my questions center around what communities are being hit the hardest and how? In 2024, how is socioeconomic inequality related to well -being at a county-level in the US, and what areas are most affected (unemployment, poverty, premature mortality, other metrics)? Are there metrics of inequity that standout when looking at social outcomes? If so, which ones?
# Methodology
1. Select metrics of inequity as independent variables and metrics of socioeconomic vulnerability (across multipel sectors) as dependent variables.
2. Feature selection- run Pairwise Mutual Information to identify most signficant variables
3. Select 1-2 leading independent vars and 3-5 dependent
4.Models and tests
	1. correlation 
	2. multivar regression
	3. apply to categrories 
		a. race 
		b. party
		c. quantiles
	4. run kl divergence between groups
# Questions for Exploration
### 1.	What geographies see the highest income inequality indexes? Gender Pay gaps? Segregation? School-finding gaps?
### 2.	Looking across social outcome variables, what trends, if any, exist in places with the highest levels of income inequality? Are there any intersections, if so, which?
### 3.	 Are certain racial groups disproportionately affected? If so, which groups and across what metrics?
a.	Are these trends (better or worse) under particular circumstances (geographic, inequity quantile, political party elected (2020)?
### 4.	In areas with at least moderate levels of racial diversity (30% minority populations), what areas show the highest and lowest segregation indices)?
a.	Are there trends along other inequity metrics?
b.	along social vulnerability metrics?
# References 
1. Cole, Maggie. Why Are so Many More Young People Living with Their Parents? Gen Z on Their Struggle to Move out - CBS New York. 30 Jan. 2024, https://www.cbsnews.com/newyork/news/why-are-so-many-young-people-living-with-their-parents/.

2. Home Price-to-Income Ratio Reaches Record High | Joint Center for Housing Studies. 22 Jan. 2024, https://www.jchs.harvard.edu/blog/home-price-income-ratio-reaches-record-high-0.

3. Manduca, Robert, et al. “Measuring Absolute Income Mobility: Lessons from North America and Europe.” American Economic Journal: Applied Economics, vol. 16, no. 2, Apr. 2024, pp. 1–30. DOI.org (Crossref), https://doi.org/10.1257/app.20210137.

4. NCRC. The New York Times: Study Shows Income Gap between Rich and Poor Keeps Growing, with Deadly Effects » NCRC. 12 Sept. 2019, https://ncrc.org/the-new-york-times-study-shows-income-gap-between-rich-and-poor-keeps-growing-with-deadly-effects/.
