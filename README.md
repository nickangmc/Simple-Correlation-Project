## Social Benefits and Crime Rate in Victoria

This study was a part of my assessment for COMP20008: Element of Data Processing at the University of Melbourne - Semester 1, 2018. More in-depth explanations and data analyses can be found in the _"report.pdf"_ in this repo. 

### Goal

#### "Can the rate of offences be reduced by giving helps and benefits through social programs to those in need?"
This is a small study to identify the correlations between social benefits, specifically Department of Social Services (DSS) payments, and crime offences rate in Victoria. DDS payments are benefits or helps allocated by the government to specific groups of residents, for example, in forms of age pensions, youth allowance, low income card, etc. Finding the appropriate correlations could potentially help the government to better manage their funds and policies in hope of minimizing the offence rate of the local communities.

---
### Data Pre-processing
Pre-processing of the datasets was done by using **pandas** library in Python. The data recorded in the datasets were stored and processed as the **DataFrame** object in Python, which it is designed to work with large matrices of data. The following processes were done to prepare the datasets to ensure successful integration:
- _Removing unnessary data_
- _Removing missing values_
- _Handling outliers_
- _Normalization_
- _Concatenating and averaging records from different timeline_

### Integration
Pre-processed data were then integrated through selected data records so that different datasets can be linked together to produce insights.

### Visualisation
There were two main methods used to visualize the results: scatter plots and heatmaps.

E.g.
##### A Heatmap showing all the correlations between different types of social benefits vs crime rate in Victoria: 
![correlation-heatmap](https://raw.githubusercontent.com/nickangmc/social-benefits-vs-crime-rate/master/Visualizations/correlation-heatmap-between-social-benefits-and-crime.png)

---
### Dataset Resources
- Department of Social Services - DSS Payments by 2014 Local Government Area: Contains attributes of 25 different types of DSS payments and the number of recipients of each type of DSS payment in all Victoria LGA. The data in it are recorded quarterly between 2016-2017. It is a comprehensive dataset and is sufficiently detailed to provide an accurate analysis.
Link: "https://data.gov.au/dataset/dss-payments-by-local-government-area"
- Crime Statistics Agency - LGA Number of offences in Victoria by offence type 2008- 2017: Includes attributes of 35 different types of offences and the offence counts recorded of each type of offence in all Victoria LGA. The data are recorded from 2008- 2017. As this dataset is provided by the CSA, it can be relied upon to be accurate and correct. Link:
"https://data.aurin.org.au/dataset/vic-govt-csa-lga-vic-crime-stats-2008-2017- lga2011"
- Australian Bureau of Statistics - Estimated Resident Population by LGA (ASGS 2016), 2001 - 2016: Contains the total number of estimated resident population (ERP) of each LGA in Australia. It covers the data from year 2001-2016. Only the data in year 2016 are required for the normalization of data values in the datasets schema. Link: "http://stat.data.abs.gov.au/Index.aspx?DataSetCode=ABS_ERP_LGA2016"

