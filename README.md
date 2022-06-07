# Map of Happiness - final project
This repository contains all of the code and data related to the final project for Laura Louise Rokkjær (201908876) & Sofie Kathleen Lloyd Thomsen (201908339)'s exam in the Spring 2022 module **Spatial Analytics** which is a part of our tilvalg in Cultural Data Science at Aarhus University.  


## Assignment description 
Our hypothesis is that the ten most happy countries in the world has a similar climate.   
In order to investigate this hypothesis we have created a leaflet map with the HPI (Happy Planet Index) score as the legend value. We have further created a temperature map with the annual mean temperature across the globe.   
To compare the two maps, we have found the ten most happy countries and plotted them into the temperature map in order to visualise how they geographically is located.  


## Method
First, we have used ```tidyverse``` and ```dyplyr``` to do some data wrangling in order to get some data that we could work with.   
Second, we have used ```leaflet``` to plot an interactive map with the values from our HPI dataset, which where used to add a legend into our leaflet map. The other three parameters (GDP, Family and Health) were used to add some labels into our polygon data to give a pop-up infobox on each country.  
Third, we used ```raster``` to get the world climate in order to create a simply map with the annual mean temperature across the globe.  


## Usage
The code can be run in R or Rstudio.

### Repo Structure  
This repository has the following directory structure:  

| **Folder** | **Description** |
| ----------- | ----------- | 
| ```input``` | Input data |
| ```output``` | Output data |
| ```src``` | R scripts |


- The ```input``` folders contains five .csv files with data from 2015-2019 and a .geojson file with the polygon data for the countries. The .csv files can also be downloaded from [kaggle](https://www.kaggle.com/datasets/unsdsn/world-happiness) and the .geojson file can be downloaded from [datahub](https://datahub.io/core/geo-countries#resource-countries). 

- The ```output``` folders contains our results (see more under 'Results')

- The ```src``` folders contains the code written in ```.Rmd``` scripts. 


## Discussion of results 
### Output
In our ourput folder can be found two html files; HPI_map.html and happiness_map.html. The former being our interactive leaflet map and the latter being our code in a more user-friendly format. 

### Results 
We can't conclude a direct correlation between happiness and temperature, but there seems to be a coherece between the two. The top ten countries were Denmark, Norway, Finland, Switzerland, Iceland, Netherlands, Canada, Sweden, New Zealand and Australia. Most of these countries are located in northern europe, where Canada has a similar climate. Australia and New Zealand stands out as countries been sightly warmer than the rest of the top ten. This is were we believe that other parameters are interesting to look into, like economy, health and family. When looking at these parameters, the top ten countries are very similar. The top ten countries are also plotted as points on our temperature map.   

When we look overall at our map of happiness, South America stands out as being quite happy despite of a lower GDP. This is not what we expected, but will be interesting to look into for furture investigation. Africa and Asia on the other hand are, as we expected, the least happy contitents. North America, Europe and Oceania are the most happy. 

