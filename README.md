# The COVID Community Profile Report FAQ

### Where can I get the data?
The data can be downloaded from
https://healthdata.gov/National/COVID-19-Community-Profile-Report/gqxm-d9w9

Here is the annoucenment from CDC on Healthdata.gov: https://healthdata.gov/stories/s/Blog-COVID-19-Open-Data-Our-Data-is-Your-Data/9c45-dw4i

### Other resources I can use to understand this data

The COVID Tracking project is listing this as one of the datasets to rely on as it ceases operations. 
[This blog post from the COVID Tracking Project](https://covidtracking.com/analysis-updates/simple-covid-data) covers this data and is a good summary of how it ties in with other datasets to get a comprehensive picture. 

### What is this data and why is this data release important?
The “Community Profile Report” is made up of two components: a PDF and an Excel spreadsheet. Both are snapshots of how COVID is affecting our states and communities.This is a critical open data release because these reports and the data within them are aggregated and prepared by our federal government to guide the national response.


These reports contain data elements that are new, and some that can be found in Public Use Files (PUF) available on https://healthdata.gov/, the CDC’s [COVID Data Tracker](https://covid.cdc.gov/covid-data-tracker/), and the datasets from the [HHS Protect portal](https://protect-public.hhs.gov/). 


While many other external COVID dashboards exist that replicate some of the data available in the Community Profile Report, this report is authoritative, and is one of the more popular means of viewing the pandemic data among the Federal Employees making critical decisions inside the Federal Government. From the perspective of the Federal Government, the Community Profile Report is the “dashboard that drives the pandemic response strategy”.


### What does it mean if a column is “green” does that mean COVID is safe in my community?
No “green” cell in this or graphic in this data report should be interpreted to mean that COVID is not a problem in your region, or that CDC recommendations should not be strictly followed. The [CDC Recommendations for COVID are clear and easy to follow ](https://www.cdc.gov/coronavirus/2019-ncov/your-health/need-to-know.html) and even when a particular city or region is doing well for COVID, it is only safe to stop following the COVID protocols when the CDC makes that determination. 

### How reliable is this data?
This data reflects the raw reporting that has been provided to the HHS Protect database and other central COVID-19 databases. Before going into the HHS Protect database, this reporting data is modified only to correct obvious errors. For instance, if a hospital has been reporting that they have 10 available and staffed ICU beds for months, and then, suddenly are reporting that they have 23456789 beds, this value is reset to 10, based on the presumption that this was an accidental data entry error on the part of hospital personnel. Data correction efforts typically involve contacting the reporting hospitals/labs/states/etcs and ensuring that data fixes are in fact correct. 
Beyond these data corrections, it is improbable that modifications or censoring of the contents of the underlying data has occurred. The COVID Tracking Project and other contributors to this dataset have examined past data releases from the central HHS Protect database that is the source for many of these reports
The data release is not perfect, and expectations that the resulting data will be perfect are not reasonable. The right answer to the question “is the data reliable?” is not yes or no. The data has been reliable enough to be used in Federal response planning for some time and continues to improve each day. The reporting consistency is high enough for broad release to the public for dozens of purposes.
Expect data restatements. Given that hospitals will update past reporting to HHS, HHS will update the data with some kind of restatements. This will maintain transparency as to how reporting data capture changes over time. 

### What specific data warnings and caveats exist for this data?
There are several places that specifically document data issues with the current “edition” of the report. These warnings frequently change as reporting quality improves day to day. The data snapshot is the “last seven days, updated today”, and the data warnings cover data problems that were known within that time period. 

In particular, the testing data in the report comes with a few crucial asterisks. It should be approached with caution for purposes of calculations such as test positivity. For one, not all state health departments report data directly to the federal government. Second, the HHS warns that testing data from the most recent seven day period is provisional and may not represent the extent of all testing in the state. Negative tests, in particular, can take longer for states to process than positive tests, leading to artificially high test positivity until those tests are retroactively added to the totals. Finally, sometimes states will not submit testing data, leading to potentially large underestimates of the testing volume in those states during the most recent 7 day period. This will cause specific rows of data to be greyed out in the report. Seeing this means that the reporting was not reliable enough to generate data that can be considered fully reliable. 


As a result, it is critical to ensure that these data warnings are considered before relying on a specific edition of the Community Profile Report. You can find these warnings on: 


* The “User Notes” tab of the Excel version under the “High Visibility Data Notes” and “Caveats on interpreting the data in the Community Profile Report” heading
* On the last page of the pdf
* The “Data Notes” tab of the Excel version

### Where does this data come from?
The data presented in the PDF and Excel spreadsheet come from the HHS Protect system. The system aggregates data collected by the various operating divisions, including CDC, CMS, HRSA, and others. According to the HHS Protect website, the system currently brings together 200 data sources.
There are many “tabs” of data inside the excel spreadsheet and many pages of data in the pdf report. Each of these has different data sources. Some of them potentially have multiple data sources. In many cases, documentation for the meaning of data is included in the file. 


Generally speaking, aggregations and calculations on a few data sources form the bulk of the report: 


* Cases
 * Aggregated county and state-level case data reported by states to the CDC  
* Tests
 * If possible, reports submitted by state health departments to the CDC’s COVID-19 Electronic Laboratory Reporting system (CELR) are used for total tests at both the state and county level. When CELR is not available, the governments will instead source data directly from the underlying labs at lab testing companies, labs within hospitals etc etc.  To be used at the state level, HHS requires that the departments can disaggregate serology tests in their totals so they can be excluded from the report. To be used at the county level, the state’s lab data must include information about the recipient’s county of residence or health provider’s location.
 * Where health department data cannot be used, the community reports substitute testing data submitted directly by laboratories to HHS Protect, which undercounts the total number of tests in counties or states.
 * At the county level, the data in ME, MO, OH, OK, PR, WA, WY rely on the direct-to-Federal government pipeline.
 * At the state level, the data in ME, MO, OK, PR, WA comes from this pipeline.
* Hospitalizations
   * These data come from data reported by hospitals directly to the Federal government or through states via Teletracking or HHS Protect. 


National release of county-level testing data has never been made available before in any dataset, nor compiled by an outside organization. 

### Can we get raw files for the underlying data?
Currently, there are raw file versions of the underlying data available for the following types of data. Most of these can be found on the “Data Notes” section of the Excel version of the report, or the final pages of the PDF version of the document.

There are some portions of the spreadsheet that have no raw data equivalent. We expect that these will become available as raw data over the course of the coming weeks.
 
#### Demographics Data
* County Population/Demographic Data Census 2019: [https://www.census.gov/data/datasets/time-series/demo/popest/2010s-counties-total.html](https://www.census.gov/data/datasets/time-series/demo/popest/2010s-counties-total.html)
* US Territory Population/Demographic Data Census 2010 (or 2020) hard to tell: [https://www.census.gov/newsroom/press-releases/2020/2020-island-areas-populations.html](https://www.census.gov/newsroom/press-releases/2020/2020-island-areas-populations.html)
* Puerto Rico Population/Demographics 2019 [https://www.census.gov/data/datasets/time-series/demo/popest/2010s-detail-puerto-rico.html](https://www.census.gov/data/datasets/time-series/demo/popest/2010s-detail-puerto-rico.html)
* Core based statistical areas (CBSAs), metropolitan divisions, and combined statistical areas (CSAs) from 2020: [https://www.census.gov/geographies/reference-files/time-series/demo/metro-micro/delineation-files.html](https://www.census.gov/geographies/reference-files/time-series/demo/metro-micro/delineation-files.html)
* National Center for Education Statistics (NCES) Integrated Postsecondary Education Data System (IPEDS) for Institutions of Higher Learning Data: [https://nces.ed.gov/ipeds/datacenter/DataFiles.aspx?goToReportId=7](https://nces.ed.gov/ipeds/datacenter/DataFiles.aspx?goToReportId=7)


#### Case and Death Data
* Puerto Rico Case and Death data from Center for Systems Science and Engineering (CSSE) at Johns Hopkins University (JHU) which is sourcing it through this ESRI link https://bioseguridad.maps.arcgis.com/apps/opsdashboard/index.html#/d7308c1abb4747e584329adf1215125e
* Previous versions of the Case and Death data were sourced through [USAfacts.org](https://usafacts.org/) Specifically:
   * Known Cases: https://static.usafacts.org/public/data/covid-19/covid_confirmed_usafacts.csv
   * Deaths: https://static.usafacts.org/public/data/covid-19/covid_deaths_usafacts.csv


* State-level Case Data comes from the CDC: https://data.cdc.gov/Case-Surveillance/COVID-19-Case-Surveillance-Public-Use-Data/vbim-akqf
   * The national level case data is aggregated from the state level data


#### Testing Data
* Testing data is sourced either through the COVID-19 Electronic Laboratory Reporting (CELR) system or directly from labs. Data from CELR is not available itself as raw data, but the progress of CELR implementation is available here: https://www.cdc.gov/coronavirus/2019-ncov/lab/electronic-reporting-map.html


#### Hospitalization Data
* Generally COVID Hospitalization data is available from the public HHS Protect portal here: https://protect-public.hhs.gov/pages/covid19-module
* There is meta-data available for the rate at hospitals report successfully into HHS protect. This data is available here: https://protect-public.hhs.gov/datasets/9f70e309bb324d3f96c49a3ead7be776/data
* Facility level Hospital COVID capacity data is also available, and you find out more on the [FAQ for that data](https://github.com/CareSet/COVID_Hospital_PUF)


### What is included in the excel edition of this report?
#### What is in the User Notes tab?
The User Notes tab provides a summary on the objectives of the Community Profile Report, as well as technical information to ensure ease of use and interpretation of the data points provided in the excel document. 


This tab prominently shows the date that the report was originally generated. 


#### What is in the Overview tab?
The Overview tab presents national summary statistics on cases, deaths, and testing, along with percentage change calculations and historical comparisons. It also includes the percentage of FEMA regions, CBSAs (see the question on “What is a CBSA?”), and counties that have hit certain per-capita thresholds for these metrics. The color-coding scheme is explained in the Color Thresholds tab. 


#### What is in the Regions tab?
The Regions tab, aggregated by the 10 FEMA Regions, presents case, death, testing, hospitalization, and skilled nursing facility data as of the latest week. For each of the data points, the file contains absolute, and or relative percentage differences from the previous week. 


Note: Insert FEMA Regions image here.  
#### What is in the States tab?
The States tab presents case, death, testing, hospitalization, and skilled nursing facility data aggregated by state. For each of the data points, the file contains absolute, and or relative percentage differences from the previous week. Data at state-level is also augmented with Area Health Metrics such as historical flu vaccination rate by age groups (0-4; 5-12; 13-17; 18-64; 65+).




#### What is in the CBSAs tab?
The CBSAs tab presents case, death, testing, hospitalization, and skilled nursing facility data aggregated by local metropolitan or micropolitan region. For each of the data points, the file contains absolute and or relative percentage differences from the previous week. Examples of demographic data points in this tab include but not limited to population size, proportion of higher education enrollment to population size, poverty rate, and race/ethnicity demographics. This tab also presents an “Area of Concern” calculated column that identifies “hotspots.” The decision tree used to generate these designations can be found on page 23 of the Community Profile Report PDF document.

#### What is in the Counties tab?
The counties tab presents case, death, testing, hospitalization, and skilled nursing facility data aggregated by county. For each of the data points, the file contains absolute and or relative percentage differences from the previous week. This tab also presents an “Area of Concern” calculated column that identifies “hotspots.” Like the CBSAs tab, it also includes demographic data about each county. It adds two forecasting columns drawn from the CDC Ensemble Forecast, which synthesizes the many forecasts submitted to the agency. 


#### What is in the Weekly Categories tab?
Each week, every State in the US is rated on testing positivity. The definition of “red/yellow/green” categories can be found in the “Color Threshold Tabs” as well as headers in the tables. 




#### What is in the National Peaks tab?
For each month, this tab lists the day which had the highest value for a particular critical data field. This chart starts in April (i.e. near the dawn of reliable data).


A pattern to note is that the “worst day” for a particular column is the same day as other columns “worst days”, but not always. 


For things that are generally improving over time (i.e. testing rates, etc) the worst day is frequently the first day of the month. 

#### What is in the National Historic tab?
This has a week-by-week progression (ending on Mondays) of the cases, deaths and testing. Using this chart, it is possible to see how the pandemic has been playing out since data started to be captured on the week of 02/03/2020.

#### What is in the Data Notes tab?
This tab is a static tab that contains meta-data about the underlying data sources and multiple notes. Many of these are static data imports and will not change from day to day. 


In this section the “Dynamic Data Notes” are critically important because they detail when testing data has not been provided from state health departments—whether because the state health department has not yet been onboarded to submit data to the federal government, or because onboarded states have not recently submitted testing data at all. It is difficult to correctly interpret testing data without considering these factors since they can lead to an underestimate of the number of tests performed. 


#### What is in the Color Thresholds tab?
The color thresholds tab is a static tab that explains how colors are applied in other tabs. 
This is a meta-data tab and details how the spreadsheet functions, rather than containing any specific data. 


The purpose of the Color Thresholds tab is described in the Data Notes tab.


### What is included in the pdf edition of this report?

#### PDF Page 1: Cover page
The first page prominently shows the date that the file was generated, and lists the table of contents for the report, listed by page number. 


#### PDF Page 2: National time series Page 3: Regional time series
These time series show the core progression of the COVID-19 pandemic over time. The specific data displayed is: 
* History of New Cases Total Volume
* History of New Deaths Total Volume
* History of Percent Test Positivity 
* History of Hospital Admissions Total Volume ( which includes breakouts for “confirmed” and “suspected” COVID cases. ) 


The regional time series exists to demonstrate regional impacts that might otherwise be hidden in national data. Make note, that these charts also switch from total volume analysis to per-100k analysis, with the exception of the percent test positivity chart, which remains by total volume. 
 
* History of New Cases per 100k cases
* History of New Deaths per 100k cases
* History of Percent Test Positivity Total Volume and regional lines for positive test percent
* History of Hospital Admissions Total Volume ( which includes breakouts for “confirmed” and “suspected” COVID cases. ) 


Using this chart you can see multiple effects: 


* The national data shows clearly the “summer surge” and the “winter surge” of the Pandemic in all three of the major measures of the pandemic, cases, deaths, and admissions. 
* At the beginning of the pandemic case and hospitalization reporting was less reliable than death reporting, so we see many more deaths, relatively speaking, than reported cases or hospital admissions. Once this reporting anomaly is accounted for, it is clear that the Cases, Deaths and Hospital Admissions data all show three different “surges” of pandemic infection. 
* Interpreting the “percent test positivity” has to be done with a grain of salt. At the beginning of the pandemic, testing was difficult and rare. As more tests became available, and could be given to more people overall, which drops the percentage returning positive. Later increases in positive percentages, as tests became widely available will continue to mirror the other 3 datasets. 
* Using the regional time series, you can see clearly how much harder NY and other parts of the Northeast were hit at the beginning of the pandemic. You can see the south having two phases and you can see how much more the current surge is impacting the Midwest. 

#### PDF pages 4-9 Geo Analysis Pages
These represent several county-level Geographic data heat maps, which detail specific data on a granular regional basis. 


* Page 4: New Cases and Deaths in the Last 7 days
* Page 5: Case incidence and whether it is improving recently
* Page 6: Mortality rate and whether it is improving recently
* Page 7: Test positivity rate and whether it is “improving” recently Page 8: The Area of Concern Continuum 
* Page 9: The Area of Concern Continuum


For pages 4-6 we will not comment much on analysis because these are relatively simple to interpret and any patterns that we point out here will be invalid within a week. 


For page 7, this is another case where it  is harder to measure improvement here because of a denominator effect. More testing will lower this score, which is good, but the total number of people testing positive could still be sky-rocketing… so this is just hard to know exactly how to interpret this on an ongoing basis. 


Page 8-9 are dependent on an epidemiological analysis method that is carefully described in page 23. Essentially, this is a merged view which is informed by examining very specific patterns in new cases in a particular region. 

#### PDF pages 10-12 National, Regional and State historical metrics
This is the “historical” tabular analysis for the pdf version of the data. 
There is slightly more data available in the Excel edition of the report, but the pdf version does include helpful [sparkline](https://en.wikipedia.org/wiki/Sparkline) charts for each row of data, which quickly visualizes the last 8 weeks of progression for that data row. 


#### PDF pages 13-17 State Level history sparkline charts
This is another use of the [sparkline](https://en.wikipedia.org/wiki/Sparkline) concept, but this time each tiny trend line is roughly positioned where a US state would be on the page. Each sparkline is positionally associated with the corresponding state. The labels for the states are small, but this gives a quick way to summarize the “regional history” of the area. 


* Page 13: Trends in case incidence over the last 8 weeks
* Page 14: 4 week mortality trend and 4 week mortality forecasts
* Page 15: Trends in percent positivity (again hard to interpret these as good/bad)
* Page 16: Trends in hospital admissions per 100 beds. This chart has two lines, for both confirmed and suspected admissions. (i.e. whether it is known for certain that an admitted patient had COVID-19 on admission)
* Page 17: Trends in hospital inpatient bed utilization


Note: accurate ICU utilization (as opposed to general bed utilization data) is available in the COVID-19 Facility Capacity Public Use File.




The word “forecast” should be emphasized here. As in predicting the weather, forecasts become less and less reliable further into the future. There is a good reason why this chart does not go “12 weeks back and 12 weeks forward”. The method used to conduct this forecast is a “cubic spline fit” and is described carefully on page 22. 


#### PDF pages 18-19 Age analysis for test-positivity and also by region.
This data shows how the testing approach has been taken. Perhaps counter-intuitively, the test positivity rate in recent months is much higher in 12-17 year olds. Of course, the reason is that if someone is given the test in this age group, it is likely that they have severe symptoms, given that this is not an at-risk age group. So this reflects a policy that tests people who are very old and very young at a greater rate. 


#### PDF pages 20-21 Cases by CBSA in high and increasing burden regions
This is another page of the pdf edition of the report, where the equivalent Excel version may have more information. But this version again has sparklines that provide additional historical information. 


Again the “burden” concept for these pages uses the Areas of Concern Continuum (AAOC) algorithm described on page 23 of the pdf. 


### Where are the population denominators from?
Most of the denominators are from Census data. You can find out which specific census datasets were used in the Data Notes tab. 


Note that most of the census data is very recent, and therefore likely to be reflective of real populations, but the Territory Populations (for Guam etc) are from 2010 and populations could have changed substantially in that time. 




### What is a CBSA and why is that chosen as an aggregation level?
CBSA stands for Core-based Statistical Area and is managed by the Office of Management and Budget focused on regions of the country that are connected via commuting. The [wikipedia page for CBSA](https://en.wikipedia.org/wiki/Core-based_statistical_area) is short but accurate and a good place to get details. You can find a [zoomable map poster available from census.gov](https://www2.census.gov/geo/maps/metroarea/us_wall/Sep2018/CBSA_WallMap_Sep2018.pdf)


One of the main benefits of CBSA over state-level regional aggreagtions is that it gets the “Twin cities problem” correct. For instance [Kansas City, Missouri](https://en.wikipedia.org/wiki/Kansas_City,_Missouri) and [Kansas City, Kansas] are in CBSA 28140


Generally, when aggregating on the “city and state” field for Geo analysis is ineffective, because it ignores the fact that large cities tend to blend in with other large cities (i.e. Dallas/Ft Worth) and there are frequently very small cities that exist within the borders of large cities. 


CBSAs have an implicit hierarchy of “ [Metropolitan Statistical Area](https://en.wikipedia.org/wiki/Metropolitan_statistical_area) (MSA)” and a Micropolitan Statistical Area (a small town). 


But for rough analysis it is enough to say that one row in a “CBSA” excel spreadsheet represents “one area within which people regularly commute, even if it crosses state lines”. 


As a result of the fact that many CBSA data rows cross state lines, it is not possible to aggregate CBSA encoded regional data back into state level data aggregations. 


### Why is there a “weekend effect” on new cases and deaths?
Many of the charts, especially on the pdf version of the Community Profile Report have a data pattern that appears to clearly be a “weekend effect”. There is a weekly pattern to many of the COVID data patterns, but it is actually a pronounced decrease in the number of deaths/cases/test/etc on Sunday and Monday. It is hard to see this on the charts on the pdf, but it is easy enough to detect in the underlying data. 


This pattern has been discussed extensively at the COVID Tracking Project and the blog post [Daily COVID-19 Data Is About to Get Weird](https://covidtracking.com/blog/daily-covid-19-data-is-about-to-get-weird) is the best place to start reading and understanding this data pattern. The other important article to read is the [Is There a Right Way to Chart COVID-19 Deaths Over Time?](https://covidtracking.com/blog/is-there-a-right-way-to-chart-covid-19-deaths-over-time) post which discusses this and other problems that occur due to counting deaths as they are reported, rather than by the date of the actual death. 


### What data is currently missing from this report?
There are at least two critical datasets that we believe might be included in future versions of this report: 


* Influenza (Flu) rate data
* Vaccination rates (obviously the data pipeline for this is still in development)


These datasets might be made available in this centralized data report or it might be made available as distinct data releases. 


### What does “IHE” stand for?
In this context it stands for “Institute of Higher Education”


###  Is there data on the availability of PPE and critical care supplies for healthcare workers? 
Some states may have these data on their dashboards, for instance (https://mn.gov/covid19/data/response-prep/response-capacity.jsp)  but this data release does not include it.




### What other “COVID Dashboards” and data are available?
There dozens of sites that allow for browsing COVID data. However, there are several critical resources that attempt to combine and clean raw datasets from scratch. 


These include: 


* The COVID Tracking Project [https://covidtracking.com](https://covidtracking.com)
   * Data Download [https://covidtracking.com/data/download](https://covidtracking.com/data/download)
   * Data API [https://covidtracking.com/data/api](https://covidtracking.com/data/api)
   * Data Sources are available by drilling down on a per state basis on the “main data page” [https://covidtracking.com/data/](https://covidtracking.com/data/)   
* COVID-19 Dashboard by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University (JHU). [https://coronavirus.jhu.edu/map.html](https://coronavirus.jhu.edu/map.html)
   * Underlying data sources [https://github.com/CSSEGISandData/COVID-19/blob/master/README.md](https://github.com/CSSEGISandData/COVID-19/blob/master/README.md)
   * Data Download [https://github.com/CSSEGISandData/COVID-19](https://github.com/CSSEGISandData/COVID-19)
* COVID-19 Hospitalization Tracking Project The Medical Industry Leadership Institute (MILI) and the Management Information Systems Research Center (MISRC) at the Carlson School of Management at the University of Minnesota: [https://carlsonschool.umn.edu/mili-misrc-covid19-tracking-project](https://carlsonschool.umn.edu/mili-misrc-covid19-tracking-project)
   * [Data Sources Google Spreadsheet](https://docs.google.com/spreadsheets/d/1ir6MK_WFQwnuboa5sKVWtliHktkKOWDw3rUH7aiYTXU/edit#gid=0)
*  [COVID Act Now](https://www.covidactnow.org/)
   * Local Dashboard [https://www.covidactnow.org/]
   * API & Download [https://apidocs.covidactnow.org/]




Note that these dashboards are collaborative and frequently collaborate to ensure that data is properly gathered and shared. As an example, the CSSE at JHU uses the COVID Tracking Project as its source for its recovered cases data. 


### Why do states sometimes fail to submit recent testing data
There are lots of reasons and they change frequently. Many times this is due to technical challenges are at the heart of this and this can occur at both states and labs. 


There are efforts to give more context on data reporting issues that will likely be part of future transparency efforts.


### What kinds of diagnostic tests are included in the report?
For the time being PCR Tests.


As other testing paradigms (i.e. antigen and at-home) this might change. 


### How are dates chosen for tests?
There are several options and we are running this information down.


### How case data sourced?
Previously this was managed by USAFacts and this data pipeline has recently transferred to the CDC. This task is to work with state and local health departments to source this data. 


### What is the deadline for “reporting cutoff”?
The data picture is always based on the data as of the day of the report. 
For each type of data, different data time frames are chosen in consideration of the underlying data reporting lags for the specific data type. 


This relationship between what data period is reported and the daily data snapshot can cause strange results on certain days. For instance, California reports some data on a weekly basis, which can cause strange results when the data is output on a daily basis, and the California report for that time period has not yet been received. To better highlight when data is missing or partially missing, the report will “grey out” rows that have not been adequately reported. 


Getting access to a daily COVID data feed is a huge improvement in the granularity of the COVID data, but it does come at a cost. The data picture fluctuates as different parts of the data pipeline fail or experience lag.  


Note: update this question to detail the typical time-window and lag for each type of data when enough data files have been released to get a solid picture of this. 


### How are testing reporting failures handled?
In the future these rows of data will be greyed out.


### How is test “positivity” calculated?
This can be done on a “per test” basis and a “per person” basis. 
There is a clarifying link, apparently. Add link here!!


### How can test positivity reach more than 100 percent?
The documentation notes that the positivity rate is capped at 100 percent, but why would it be more than 100 percent, before capping. Why might this happen?


### When is the CELR system used?
For context, the COVID-19 Electronic Laboratory Reporting (CELR) pronounced like “sealing” as in “sealing cracks” i.e. like a “person who covers over cracks”. 


The Federal transition to using CELR for a state occurs when a state is capable of isolating their PCR tests from other kinds of diagnostic testing. 


### Which states are using CELR
You can see this here: 
https://www.cdc.gov/coronavirus/2019-ncov/lab/electronic-reporting-map.html


This is also listed as a high priority data note on the cover of the Excel version of the Report.


### Which hospitals are included in this data release
This release excludes psychiatric, rehabilitation, and religious non-medical hospitals.
We are investigating if VA and IHS hospital data is included in the data release, but we currently believe that this data is included. 

### Are there other good resources for understanding this data?

[Liz Essley Whyte](https://twitter.com/l_e_whyte) from the [Center for public integrity](https://publicintegrity.org/) has a [twitter thread tour of the data report](https://twitter.com/l_e_whyte/status/1340323898626289670?s=21). 

### Who wrote this FAQ?
This FAQ is a collaboration between:


* Data Journalists at [Careset Systems](https://www.careset.com)
* Researchers from the [University of Minnesota COVID-19 Hospitalization Tracking Project](https://carlsonschool.umn.edu/mili-misrc-covid19-tracking-project) at the Carlson School of Management - [Medical Industry Leadership Institute (MILI)](https://carlsonschool.umn.edu/faculty-research/medical-industry-leadership-institute) and the [Management Information Systems Research Center (MISRC)](https://carlsonschool.umn.edu/faculty-research/mis-research-center)
* Volunteers from [COVID Exit Strategy](https://www.covidexitstrategy.org) and [COVID Act Now](https://www.covidactnow.org/)
* Researchers from the [COVID Tracking Project](https://covidtracking.com)
