PPOL 670 Final Project
By Lucas Fox, Nathalie Kirsch, Vanaaisha Pamnani, and Cuong Pham Vu
https://github.com/nakirsch/PPOL670_FinalProject


This project uses data from Open Data DC on crime incidents in DC from 2010 to 
2022, as well as demographic data from the Census's 5-year surveys, to study 
how DC's crime rates and types of crime have changed over the course of the 
COVID-19 pandemic and over the ten years leading up to the pandemic. In this 
analysis, we first explore DC's crime counts and rates through data 
visualization, then use lasso regression to predict the number of crimes in DC
in a given year. 

Our data visualizations and predictive modeling can provide policymakers a
better understanding of the types, frequency, and patterns of crimes reported 
in DC. More importantly, it provides an in-depth look at what factors contribute
to crime in DC both pre and post pandemic, informing policy makers on potential
ways to address crimes in DC. 

Our folder contains:
1.data_visualizations.Rmd
2.data_visualizations.html
3.data_wrangling.Rmd
4.predictive_modeling.Rmd
5.predictive_modeling.html
6.final_project.Rproj
7. README.md
8. .gitignore
9.  A 'data' folder containing these files below downloaded from Open Data DC,
DC Census Tracts Data, DC Police Station data, and American Community Survey 
5-Year Data:
  a. Census_Tracts_in_2010.geojson
  b. Crime_Incidents_in[2010 - 2022].geojson (12 .geojson files)
  c. Police_Stations.geojson
  d. acs_merged.csv
  e. crime_merged_agg.csv
  f. crime_merrged_agg.geojson

Instructions: 
Our code is distributed across 3 files:
1.data_visualizations.Rmd: code for all libraries, original datasets, and 
cleaned datasets for our data visualizations and, code for all of our data visualizations. 

Note: When we refer to the crime rate, we are using the number of crimes per 1,000 residents. 

2.data_wrangling.Rmd: code for all libraries, original ACS data, and
cleaned ACS data for our predictive model. Creates csv files that the predictive modeling Rmd uses. We did this to reduce the time it takes us to process the data in each individual Rmd. 

3.predictive_modeling.Rmd: code for our lasso predicted model and principal components analysis, that identified specific demographic variables from ACS data that were correlated with crime count per census tract. The first two principal components in our analysis explained ~70% of the variation in the data.

For our data visualizations, first download and run the file, data_wrangling.Rmd, then download and run the file, data_visualizations.Rmd.
To run our predictive model, first download and run the file, data_wrangling.Rmd
and then download and run predictive_modeling.Rmd.

All libraries needed are included in the code, but installing these packages may
still be required. 
