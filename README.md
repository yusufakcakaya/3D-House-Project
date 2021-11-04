# 3D HOUSE 🏠
### Get ready to create 3D houses : 🏡 

![giphy](https://user-images.githubusercontent.com/46165841/140303832-57cb30ff-7928-4de4-af32-ab6e07eeee88.gif)

## 

The main mission of the project is creating a model which is a house in 3D with only a home address.These 3D models are created for _LIDAR PLANES_, active in the Geospatial industry. At the end of the project you can give an address from Vlanderen in Belgium and you can take a 3D out put of your address building.

While saving the datasets, used python libraries like ;
 - import requests
 - import matplotlib.pyplot as plt
 - import pandas as pd
 - import rasterio
 - from rasterio.mask import mask
 - import shapely.geometry as geo
 - import plotly.graph_objects as go
 - import numpy as np

I recieved the coordinate informations from this API address [API](https://docs.basisregisters.vlaanderen.be/docs/api-documentation.html#section/Technische-Info/Foutmeldingen)
 
#### What is LIDAR ?

LIDAR is a method to measure distance using light. The device will illuminate a target with a laser light and a sensor will measure the reflection. Differences in wavelength and return times will be used to get 3D representations of an area.

Here is a LIDAR segmentation :

With those points clouds we can easily identify houses, vegetation, roads, etc...

The results we're interested in are DSM (Digital Surface Map) and DTM (Digital Terrain Map).

Which are already computed and available here :

- [DSM](http://www.geopunt.be/download?container=dhm-vlaanderen-ii-dsm-raster-1m&title=Digitaal%20Hoogtemodel%20Vlaanderen%20II,%20DSM,%20raster,%201m)
- [DTM](http://www.geopunt.be/download?container=dhm-vlaanderen-ii-dtm-raster-1m&title=Digitaal%20Hoogtemodel%20Vlaanderen%20II,%20DTM,%20raster,%201m)

Canopy Height Model
The DSM and the DTM are combined together to create a Canopy Height Model (CHM) which is required for the 3D model.

![chm](https://user-images.githubusercontent.com/46165841/140337622-3f9abada-0d21-4413-a549-7aa436009bd5.png)



## Installation

- Pull requests are welcome.
- or ```git clone https://github.com/yusufakcakaya/3D_houses.git```
- 

## Repo Architecture 

```
3D_houses
│
│   README.md              : explains the project
│   
│__   
│   3D_HOUSE.ipynb         : main file
│   
│__ 
│   url_generator.ipynb    : to create a .csv file to save bounds and urls
│  
│__ list_of_bounds.csv     : csv file of bounds
│

```

## Visuals

Examples of outputs.

Address : Sint-Pietersvliet 7, 2000

![newplot (2)](https://user-images.githubusercontent.com/46165841/140322187-6a5820bc-4277-4f13-a6a8-2fe03fb1612f.png)

Address : Hanzestedenplaats 1, 2000 

![newplot (2)](https://user-images.githubusercontent.com/46165841/140325954-edd15765-eb27-44b7-955e-e6f59b958f88.png)


![voow](https://user-images.githubusercontent.com/46165841/140304494-444740b8-49c5-42b4-9dc6-1a9e68338855.gif)

## Timeline

- Repository: `3D_houses`
- Type of Challenge: `Learning & Consolidation`
- Duration: `2 weeks`
- Deadline: `04/11/21 17:00 PM`
- Deployment strategy :
  - GitHub page
  - PowerPoint
  - Jupyter Notebook
  - Webpage
  - App
- Team challenge : `solo`

## Good Luck!
