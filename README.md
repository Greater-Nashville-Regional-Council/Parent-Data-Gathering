# **Parent-Data-Gathering**

## *Table of Contents*  
+ Overview
+ APIs  
+ Data Downloads  
+ Exports and Data Storage
+ File Structure  
+ Data Bank   

## Overview  
This repository outlines the process for gathering frequently requested data through the most efficient methods we can, and building on this library over time. In the APIs folder there is code for pulling data from various public APIs and formatting it uniformly so that data can be joined for various analyses. There is a notebook for each data series (and year, if needed) to ensure that there is no variable confusion. Additionally, data that must be downloaded from the internet or shared by staff is stored and formatted uniformly here. This information is saved and ready to be filtered for various comprehensive plans and data requests.  

## APIs  
+ Census Bureau  
+ Census TIGER Files
+ Center for Disease Control  
+ Bureau of Economic Analysis  
+ Bureau of Labor Statistics  

## Downloaded Data Sources  
+ Woods and Poole Projections  
+ Department of Housing and Urban Development Residential Permits  
+ TN State Data Center  
+ Historical Census Population  

## Formatting, Calculations, Exports and Data Storage  
As this process is developed as an outline for all data pulls and formatting, exports from API calls and download formatting are standardized and stored to be pulled into other projects and filtered appropriately. Frequently used formatting/calculations from raw data are performed for all geographies in the GNRC region and many adjacent geographies simultaneously. The raw data is catalogued, but dropped at this point. For every data source and year, requested data points are accumulated here over time. All files are available to be catalogued, or deleted and reproduced using the same process when needed for other projects for storage efficiency.

## File Structure  

#### **Data Guides**  
Contains: Various lists of variables, column names, and descriptions that are imported and run through APIs to call the listed data   

#### **Notebooks**  
Contains: The following folders  

*API Pulls*: This folder contains notebooks for each respective data series and year. Accepting the ACS 1YR estimates, each has its own data guide. The 1YRs are not large amounts of data and currently the variables are all the same year over year, if more data is added from these estimates they will be split as well.  
+ ACS 2010 5YR  
+ ACS 2020 5YR  
+ ACS 2017 1YR  
+ ACS 2018 1YR  
+ ACS 2019 1YR  
+ ACS 2021 1YR  
+ Decennial 2020 PL  
+ Decennial 2000 SF1  
+ Decennial 2010 SF1  
+ Decennial 2000 SF3  
+ Subject Tables 2010, 2020 5YR  
+ TIGER Files 2000, 2010, 2020  

*Download Formatting*: This folder contains notebooks for the data downloaded from the web or provided by GNRC staff  
+ Historical and Projected Population  

*Calculations*: This folder contains notebooks transforming the raw data into frequently requested metrics. Note that the subject tables, ACS 1YRs, and TIGER files are currently transformed in the "pull" documents because of their brevity. The download formatting documents bring the data to this point as well.  

#### **Data**  
Contains: The data that is pulled and ready to be run through calculations    

#### **Outputs**  
Contains: Formatted data that is ready to be pulled into other projects/repositories for filtering and analysis.

*The "data" and "outputs" folders can be empty if storage space is needed, and then duplicated with the notebook files at anytime.*

The following data is collected (**Data Bank**):  


## Data Bank
+ TIGERS2000, TIGERS2010, and TIGERS2020 shapefiles containing the geometry and geoid for each geography collected   
+ TIGERS2000, TIGERS2010, and TIGERS2020 csv files containing square miles and square acres of land area for each geography collected and calculated  
+ 2010Subject, 2020Subject csv files containing the median travel time to work for each geography collected  
+ 2017ACS1YR, 2018ACS1YR, 2019ACS1YR, 2021ACS1YR csv files containing the geographic mobility in the past year dataset for each geography collected and calculated  
+ HIST_PROJECT_PopulationSUFFIX csv containing historical and projected population data from 1800 to 2045 with each column tagged with the year  
+ HIST_PROJECT_PopulationTIDY csv containing historical and projected population data tidy data from 1800 to 2045 formatted with real and percent change between years  
+ 2000SF3 csv: 1,703 raw variables --> 535 data points  
+ 2000SF1 csv: 88 raw variables --> 116 data points  
+ 2010SF1 csv: 79 raw variables --> 116 data points
+ 2010 ACS5YR: 1,694 raw variables --> 565 data points  
+ 2020 PL: 25 raw variables --> 62 data points
+ 2020 ACS5YR: 2,371 raw variables --> 617 data points  
+ HUDResidentialPermits_2021: residential permit data for single and multifamily for all counties, unincorporated counties, and places  
+ LAUS: 2 csv files containing the unemployment rate from the BLS's Local Area Unemployment Series one with the most recent annual avereage rate and one with monthly unadjusted rates from 2019 to the most recent (preliminary) month. Geographies include all counties in the region as well as incorporated places with population over 25,000  
+ 
