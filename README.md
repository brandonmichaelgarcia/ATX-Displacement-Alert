# ATX-Displacement-Alert
A Tool to identify displacement risk in Austin, TX.


## MISSION:
Through this project, we will develop a tool for on-the-ground activists, who can use the geographic information to cut turf, create walk lists, and canvass door-to-door, connecting  Austin residents at risk of displacement with useful resources and information they can utilize to prevent or fight back against eviction.


## SOLUTION:
We are looking to create an interactive map web application, with multiple layers overlayed on the map to describe the risk of resident/tenant displacement. Because the real-time eviction filings provide only zip code level data and represent only a part of all displacements, we have sought to use multiple data sources that provide both a higher level of resolution (i.e. we want data that is localized on areas smaller than zip code level) and a more complete sketch of the factors that correlate with displacement.

Currently, we aim to describe the risk of displacement using the following risk factors:
1. recent eviction filings (zip code resolution)
2. new building sales (street address resolution)
3. new building construction permits (street address resolution)
                        +
4. eviction rates from 2000-2016 (block group resolution).
5. poverty rates from 2000-2016 (block group resolution).
6. median property value from 2000-2016 (block group resolution).
7. percent renter occupied from 2000-2016 (block group resolution).
8. population size from 2000-2016 (block group resolution).

It is clear that just overlaying each of the above risk factors on a map may not be the most useful or user-friendly way to describe the risk of displacement. Thus, each risk factor may need to be restricted to exclude irrelevant data, or weighted by other factors to highlight subsets that most clearly are associated with displacement risk.

*FOR MORE INFORMATION ABOUT THESE DATA SOURCES, LOOK AT THE README HERE: https://github.com/brandonmichaelgarcia/ATX-Displacement-Alert/blob/master/Data%20Source%20Planning/README-DataSources.md*


## CURRENT TASKS/CHALLENGES:
* Identify data source for new building sales.
* Identify new building sales that are most relevant to displacement risk.
* Identify building construction permits that are most relevant to displacement risk.
* Idenfity methods to best weight/adjust risk factors to improve relevance.
* Identify risk formula to best combine risk factors.
* Build script to use for regular web-scraping of recent eviction filings from a dynamically generated webpage.
* Build script to use for regular web-scraping of new building sales from a dynamically generated webpage.
* Build database supporting querying for relevant data to display in a heat map layer.
* Build web application that supports viewing multiple heat map layers describing risk. 
* Build functionality to provide animated time-lapse of historical data.
