# Geospatial data science – Antwerp Airbnb analysis


## Overview

<div align="justify">This is a project I carried out for the exam of "Geospatial analysis and representation for data science", which is part of my Master programme in Data Science. 
The work consists of geospatial analyses on Airbnb data about a chosen city (Antwerp in Belgium, in my case). To be more specific, the project offers:</div>

* Analysis and visual representation of neighbourhoods population data
* Identification of the top 5 neighbourhoods for Airbnb price and number
* Tourist activities by neighbourhood 
* Retrieval of the 3 closest Airbnbs with respect to one of the most popular museums of the city (street network analysis)
* Services around the Airbnbs identified in the previous point
* Analysis of the spatial autocorrelation of Airbnbs' prices
* Visualization of the results with static and web maps


## Data
<div align="justify">
The data used during the analysis comes from different sources. Data about the neighbourhoods of Antwerp, its population density and its museums are geojson files retrieved from the [city data portal] (https://portaal-stadantwerpen.opendata.arcgis.com/) . Additional data about the population come from an .xlsx file downloaded from the [database of the city](https://stadincijfers.antwerpen.be/databank). [Inside Airbnb](http://insideairbnb.com/get-the-data.html) offers data about all the Airbnb of Antwerp and, in particular, I used the listings.csv file. From export.hotosm.org I created and extracted the .pbf [bounding box of Antwerp](https://export.hotosm.org/en/v3/exports/b0f5f5b5-935b-45d6-a890-22d521e4c9de) in order to retrieve data about the tourist activities and other services of the city from Openstreetmap. Finally, for the analysis of the spatial autocorrelation of price I created a .shp file with data about the neighbourhoods of the city and its Airbnb price coming from the previous analyses.</div>


## Requirements

The Code is written in Python 3.8.5 and in R 4.0.3.
Python libraries:
* pandas==1.1.3
* geopandas==0.8.1
* folium==0.11.0
* branca==0.4.1
* geopy==2.0.0
* osmnx==0.16.1
* Shapely==1.7.1
* pyproj==2.6.1.post1
* pyrosm==0.5.3
* matplotlib==3.3.2
* contextily==1.0.1

R libraries:
* rgdal 1.5.23
* spdep 1.1.5


## Author

* Marta Fattorel (marta.fattorel@studenti.unitn.it)


## Licence

This work is available under the Creative Commons Attribution-ShareAlike License. Read more about this license from [https://creativecommons.org/licenses/by-sa/3.0/](https://creativecommons.org/licenses/by-sa/3.0/).
