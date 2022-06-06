# Map of Happiness - final project
This repository contains all of the code and data related to the final project for Laura Louise Rokkjær and Sofie K. Lloyd Thomsens exam in the Spring 2022 module **Spatial Analytics** which is a part of our tilvalg in Cultural Data Science at Aarhus University.  


## Assignment description 
Our hypothesis is that the ten most happy countries in the world has a similar climate.   
In order to investigate this hypothesis we have created a leaflet map with the HPI (Happy Planet Index) score as the legend value. We have further created a temperature map with the annual mean temperature across the globe.   
To compare the two maps, we have found the ten most happy countries and plotted them into the temperature map in order to visualise how they geographically is located.  


## Method
First, we have used ```tidyverse``` and ```dyplyr``` to do some data wrangling in order to get some data that we could work with.   
Second, we have used ```leaflet``` to plot an interactive map with the values from our HPI dataset, which where used to add a legend into our leaflet map. The other three parameters (GDP, Family and Health) were used to add some labels into our polygon data to give a pop-up infobox on each country.  
Third, we used ```raster``` to get the world climate in order to create a simply map with the annual mean temperature across the globe.  


## Usage
In order to reproduce this code, you'll need to uploade your own data into the ```input``` folder.   
We have used five dataset, that can be found [here](https://www.kaggle.com/datasets/unsdsn/world-happiness).    
For our polygon data with the countries, we have used the 'countries' dataset from [datahub](https://datahub.io/core/geo-countries#resource-countries). 

You'll also have to install the needed packages, which can be found in ```requirements.txt```. 


### Repo Structure  
This repository has the following directory structure:  

| **Folder** | **Description** |
| ----------- | ----------- | 
| ```input``` | Input data |
| ```output``` | Output data |
| ```src``` | R scripts |


- The ```input``` folders are empty and this is where you should upload your own data, if you want to reproduce the code.

- The ```output``` folders contains my results and it is this folder that you should save your own results when replicating the code. 

- The ```src``` folders contains the code written in ```.Rmd``` scripts. 


## Discussion of results 
### Results 

### Further development 


