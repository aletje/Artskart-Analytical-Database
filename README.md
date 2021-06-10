# Redlisted specie observations in Norway and nearby weather stations close to the specie observation geo-location
### Data Engineering Capstone Project

#### Project Summary
The project aims to provide a SQL query interface of Redlisted Species in Norway. Every redlisted specie observation is enriched with weather station metadata close to the specie observation geo-location point. Data pre-processing and ETL is done with Python, PySpark and Spark SQL. The final datasets are stored as parquet tables hosted on AWS S3.

#### Data sources

- #### Artskart
Artskart is a Norwegian Citizen science project for recording species on maps into a national and freely accessible database. Artskart is owned by The Norwegian Biodiversity Information Centre. You may read more about Artskart here: https://www.biodiversity.no/Pages/135580/About_Norwegian_Biodiversity_Information_Centre?Key=1435226530 

- #### MET Norway
The Norwegian Meteorological Institute (MET Norway) forecasts weather and monitors the climate. Data from MET Norway is gathered from their free API service here: https://api.met.no/. You may read more about MET here: https://www.met.no/en/About-us/About-MET-Norway