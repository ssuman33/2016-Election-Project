# 2016-Election-Project

The project's purpose was to pull data from all 159 counties in Georgia using Python in order to map and understand correlations between the 2016 presidential election outcomes, poverty concentrations, educational & economic inequality and COVID-19 transmission rates.

We chose this to understand how an area's political makeup correlates to their overall well-being as a society. 
From our analysis, we hoped to draw correlations between poverty, unemployment and health based on how democratic or republican an area is. With the presidential election only a few days away, it's important to us to understand why certain communities vote the way they do. 

The aim was to determine whether primarily democratic or republican communities are prone to unemployment and educational deficits. Furthermore, we hope to draw coorelations between these figures and current coronavirus rates in each county to determine if any of the factors mentioned above contribute significantly to spread. We will use metadata such as income and disease rates to back our findings. We also hope to see how democratic and republican counties compare in regards to poverty levels, specifically underage poverty.

# Phase I

The first phase of the project revolved around scraping, parsing and cleaning large data sets from all 159 counties in Georgia into usable and understandable quantities.

Modules such as BeautifulSoup, requests and csv were used to collect data. To clean inconsistencies from the data, it was funnelled into dictionaries, with the primary key being the county name, and the values being the data collected on each respective county. This is done rather efficiently using for loops to go through the data and pick out county names, values, etc. This allowed us to standardize and easily access data on a county. For example, county['forsyth']['%_dem'] will show us the percent that voted democratic in the 2016 election for Forsyth County. 

The code, exported data and process on inconsistency removal can be found in 'Phase I.ipynb'. 

# Phase II

The second phase was analysis and visualization. The collected data was consolidated into both a pandas dataframe and an aggregated dictionary for ease of analysis.

The analysis was split into Insights and Visualizations. Insights were hard mathematical data that could be used to draw specific evidence to prove or disprove our hypotheses. Visualization was to observe trends between two variables. Visualization and linear regressions were done using Seaborn, matplotlib and numpy.

The code, data analysis and visualizations can be found in 'Phase II.ipynb'. 

# Datasets

*Downloaded CSV - this is incredibly detailed poverty information over the course of five years for counties throughout the US including every county in Georgia - the filename is ACSST5Y2015.S1701_data_with_overlays_2020-10-26T184714.csv, imported into this notebook as data.csv (rename the file). Be sure to download the 2015, 5 year zip folder.

*Web HTML - this is the election information for every county in GA for the last election, how many people voted Democrat and Republican, respectively. This information can be found here.

*Web API - this dataset provides information about the past three election as well as numerous other demographic factors such as the county's demographics, education and school enrollment. This information can be found here.

*Web API - used an API that provides information about how much the Covid-19 pandemic has affected every county in Georgia. This information can be found here.

All of these data sets provide detailed information for every county in Georgia. The key dataset will be Web Collection Requirment 1 as it contains voter information for Georgia's counties. We will then cross this information with county demographics, COVID-19 effects, poverty and other factors which can be found through the other three data sets in order to identify specific correlations between these factors and the county's political leanings. 
