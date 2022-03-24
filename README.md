# Traffic Accident Geospatial Analysis using US-Accidents (2016-2021) Open Data


## Brief Rationale

  Around 1.2 million road traffic fatalities are recorded annually around the globe (World Health Organization, 2009, 2013, 2015), while road crashes resulting in non-fatal injuries range from 20 to 50 million (World Health Organization, 2009, 2013). Additionally, road traffic accidents are the ninth leading cause of death across all ages globally based on the Global Burden of Disease update 2004 and sixth among the middle-income countries (Mathers & WHO, 2008). With that, this study investigates the spatial pattern and temporal trends of the traffic accidents and fatalities in Dallas, Texas, through Geospatial analysis using Spatial Data Science techniques and workflows with ArcGIS. Current studies directed at the City or County level have either utilized small-scale and homogenous data or outdated datasets, worse with insufficient data at all. Thus, this study will delve into the US-Traffic accident open data (2016-2021), a heterogenous but sparse dataset with 2.8 million records (Moosavi et al, 2019), to propose an adaptable workflow from a data science perspective that aims to help policy-makers create data-driven decisions and regulations. The Geospatial Analysis will be conducted through multiple hotspots and space-time statistical analyses using ArcGIS and python libraries. 
  

## Objectives

The overarching goals of this project are to 
  - Investigate the heterogeneous and sparse data of Dallas Traffic Accidents from 2016 to 2021,
  - Determine Spatial Autocorrelation of the traffic accidents in Dallas
  - Identify statistically significant hot spots and cold spots of the traffic accidents,
  - Find and visualize traffic accident spatial patterns and temporal trends using ArcGIS,
  - Provide recommendations on effective resource allocation for traffic incidents and to promote data-driven decisions,
  - Propose adaptable Geospatial Analysis workflow that may benefit underdeveloped cities in their process of data gathering for conducting this kind of  incident data analysis

## Methodology

  This study methodology consists of different stages: (1) Data Collection, (2) Data Preprocessing, (3) Spatial Autocorrelation (Global Moran’s I), (4) Modeling Spatial Relationships, (5) Hot Spot Analysis (Getis-Ord Gi*), and (6) Space-Time Statistical Analysis. 
   
   First is the mapping of the study area, which is Dallas. And as the most actively updated open data, the US-Accidents will be used in this study. Moosavi et al. (2019) created a large-scale US-Accidents open data through their deep-neural-network model called Deep Accident Prediction (DAP), which includes a variety of data attributes such as traffic events, weather-related information, points-of-interest, and time. The dataset has been continuously collected from 2016 and was recently updated to December 2021, last March 12, 2022. However, since the study area will be Dallas, Texas, the traffic accident data that specifically happened in Dallas will be extracted from the 2.8 million records from 2016 to 2021.  The extracted data will then undergo data preprocessing to conform to the required format before conducting the analysis, including georeferencing and digitization. Next, using the Spatial Autocorrelation tool of ArcGIS, which applies the Global Moran’s autocorrelation coefficient I, calculate the spatial autocorrelation of the data. Spatial relationships must be set and modeled before conducting the Hotspot and Space-Time Statistical Analyses. 
    The Hot Spot Analysis tool, which applies Getis-Ord Gi* statistics, will be used to identify the statistically significant hot spots and cold spots with its resultant z-score, p-values, and Gi-bin confidence values. Conducting the space-time analysis will narrow down the insights from the data to find temporal trends and analyze patterns that may not have been detected during the hotspot analysis without considering time.  
