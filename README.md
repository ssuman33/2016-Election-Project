# 2016-Election-Project
We used results of the 2016 election to answer questions and draw insights about a county's economy and overall health based on how the county voted in the 2016 election.

We chose this to understand how an area's political makeup correlates to their overall well-being as a society. 
From our analysis, we hoped to draw correlations between poverty, unemployment and health based on how democratic or republican an area is. With the presidential election only a few days away, it's important to us to understand why certain communities vote the way they do. 

One insight we hoped to see is whether primarily democratic or republican communities are prone to unemployment and educational deficits. Furthermore, we hope to draw coorelations between these ifgures and current coronavirus rates in each county to determine if any of the factors mentioned above contribute significantly to spread. We will use metadata such as income and disease rates to back our findings. We also hope to see how democratic and republican counties compare in regards to poverty levels, specifically underage poverty.

Datasets:

*Downloaded CSV - this is incredibly detailed poverty information over the course of five years for counties throughout the US including every county in Georgia - the filename is ACSST5Y2015.S1701_data_with_overlays_2020-10-26T184714.csv, imported into this notebook as data.csv (rename the file). Be sure to download the 2015, 5 year zip folder. The downloaded data set is here.

*Web HTML - this is the election information for every county in GA for the last election, how many people voted Democrat and Republican, respectively. This information can be found here.

*Web API - this dataset provides information about the past three election as well as numerous other demographic factors such as the county's demographics, education and school enrollment. This information can be found here.

*Web API - used an API that provides information about how much the Covid-19 pandemic has affected every county in Georgia. This information can be found here.

All of these data sets provide detailed information for every county in Georgia. The key dataset will be Web Collection Requirment 1 as it contains voter information for Georgia's counties. We will then cross this information with county demographics, Covid-19 effects, poverty and other factors which can be found through the other three data sets in order to identify specific correlations between these factors and the county's political leanings. 
