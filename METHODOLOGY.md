# Methodology:

## cases.csv:
Each day, any new cases announced by the Government of Saskatchewan are added. Usually, the region of each new case is indicated in the press release or news conference; however on days where this information is not released, the aggregate region totals are compared to the previous days’ and the resulting difference per region is used to determine the region of the new case(s) announced. On days where a single case is reported, age data for the new case can be determined by comparing the aggregate ages to the previous day. In addition, if any reputable news media reports any further details, they are added to case details.

## cases_aggregate.csv:
Basic case data is added using the same methodology as cases.csv; however, in order to expand the available details, aggregate data published to Saskatchewan.ca is compared to prior days and utilized to determine the ages and sexes of new cases added. While the overall additions of age groups and sex for each day will be accurate, as the data provided is only aggregate, this data is simply added to one of the days’ case arbitrarily. This arbitrary assignment is indicated with a ‘*’ following each uncertain datapoint. In addition, there is much greater uncertainty for determining the sex of new cases as the values released are percentages (i.e. 50% male, 50% female). In order to determine the sex, the total number of cases is independently multiplied by the percentage of sex in order to determine the total number of cases per sex. These values are compared to the previous day and the resultant change indicates the number of new cases for each sex.

On occasion, reported changes in the percentage of cases for each sex are impossible. For example on May 17, although only a single additional case was added (equivalent to 0.17% of all cases), the sex distribution was reportedly changed 2% from 51% male and 49% female to 49% male and 51% female. In such situations, our previously published data where distribution was very close is reviewed and potentially slightly modified in order to maintain overall accuracy using aggregate values. 

It is important that any values followed by a ‘*’ are not taken as certain and accepted to be an approximate, arbitrarily assigned indicator to assist in the recognition of any long-term trends.

## fatalities.csv
Fatality data is collected almost exclusively from news media sources. While information provided by the government regarding fatalities is quite sparse, the families of victims in Saskatchewan have been willing to share further information with the media. Region and sub-region are based on the residences of the fatalities. Because the government reports based on where their health cards are registered which may not have been the current residence of each fatality, there may be regional discrepancies.

## hospitalizations.csv
Hospitalization data is collected directly from Saskatchewan.ca daily for each region. Data is reported exactly as it appeared on the day reported. Additional historical data may occasionally be added from news media reports.

## recoveries.csv
Recoveries data is collected directly from Saskatchewan.ca daily for each region. Data is reported exactly as it appeared on the day reported. Additional historical data may occasionally be added from news media reports.

## testing.csv
Testing data is collected directly from Saskatchewan.ca daily for each region. Both the number of people tested and the total number of tests are recorded. Data is reported exactly as it appeared on the day reported. Additional historical data may occasionally be added from news media reports.
