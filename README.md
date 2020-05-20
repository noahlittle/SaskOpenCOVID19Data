# Saskatchewan Open COVID-19 Data
This is a collection of all publicly available case, testing, recovery, hospitalization, fatality and policy data for Saskatchewan during the ongoing COVID-19 Pandemic. Please read this document prior to any use due to some important data notes. If you wish to view the data rather than download it, all data is available to be viewed online [here](https://docs.google.com/spreadsheets/d/e/2PACX-1vSpXwT4tlmuwbCyI-IkkJZNVEYu2IjuxieoNDpW_ibIMY1niFDkn17_ZWYWvz5nq-X6mNLF_gm3U9XL/pubhtml).
## Cases
There are two separate files for case data.
### cases.csv
This file contains the known case data and makes few assumptions, with the exception of some minor regional distribution in March. As very little is officially released about each case, this file mostly includes only the region, subregion (if known) and date of each case.
### aggregate_cases.csv
Using aggregate data provided daily, each case in this file contains detailed information including sex, age and transmission type. It also contains blank fields for potential future additions to the dataset. However, this data is based on daily aggregates which are arbitrarily distributed among the cases of each day. Each individual case involves a high degree of error due to this daily distribution. Overall, the aggregate data for each day should be accurate but individual cases will not be. Age, sex and transmission type are applied to each days' cases arbitrarily and should not be considered in isolation. As such, it is vital that any analysis only involves a single aspect (for example, ages over time) and not multiple (such as ages in each sex over time), as any analysis of which would be completely invalid.
## Fatalities
fatalities.csv contains detailed information on each fatality collected from news media reports along with provided provincial data. Currently, region is based on the location each individual was a resident of. Personal information, such as the name of each individual, is only provided when that data is publically available and if the family consents to the release of such information.
## Testing
testing.csv contains detailed daily testing information for each region of the province. The 'cumulative_people_tested' field refers to the number of people with tests ordered in each region and the 'cumulative_number_tests' field refers to the total number of tests conducted in each region. All values are cumulative.
## Recoveries
recoveries.csv contains daily recovery information for each region of the province. All values are cumulative.
## Hospitalizations
hospitalizations.csv contains daily hospitalization data for each region of the province. The 'current_inpatient' field refers to the number of COVID-19 patients recieving inpatient care on each day in each region and the 'current_critical' field refers to the number of patients currently recieving care in the ICU on each day for each region. Note that 'current_inpatient' is NOT inclusive to the ICU cases and both must be summed in order to determine the total daily hospitalizations in each region.
## Policy
policy.csv contains a list of Public Health policies by date enacted to limit the spread of COVID-19. Refer to key.csv if any shorthand unclear.
# Contributors
Contributors to the project are listed as follows
- Noah Little
# License
This dataset is licensed under a Creative Commons Attribution 4.0 International License. In basic terms, this means that anyone is able to share and/or adapt the dataset for any purpose (even commercially), with the condition that appropriate credit is given. Please see the full license text [here](https://github.com/noahlittle/SaskOpenCOVID19Data/blob/master/license.md).

#### Recommended Citation
Little, N. (2020). SaskOpenCOVID19Data [GitHub repository]. doi: 10.5281/zenodo.3834955

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3834955.svg)](https://doi.org/10.5281/zenodo.3834955)
# Sources
Most data including testing, recoveries and hospitalizations data is collected daily from the Saskatchewan.ca "Cases and Risks of COVID-19 in Saskatchewan" page, an archive of which is available [here](https://publications.saskatchewan.ca/#/products/104914). More detailed data regarding cases and fatalities is collected from a variety of news media sources. In addition, the line-by-line case information is based off of data published to the [COVID-19 Tracker Canada project](https://covid19tracker.ca).
# Acknowledgments
- The Government of Saskatchewan for releasing detailed data in a timely fashion
- Saskatchewan Graphic by Adnen Kadri from the Noun Project
