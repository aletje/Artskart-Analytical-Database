# Artskart Analytical Database
### Data Engineering Capstone Project

#### Project Summary
Making a query optimized analytical database of Redlisted Species in Norway with Artskart. Further, enrich data with population growth and deforestation. Artskart is a Citizen science project for recording species on maps into a national and freely accessible database. Artskart is owned by The Norwegian Biodiversity Information Centre. You may read more about Artskart here: https://www.biodiversity.no/Pages/135580/About_Norwegian_Biodiversity_Information_Centre?Key=1435226530

The project follows these steps:
* Step 1: Scope the Project and Gather Data
* Step 2: Explore and Assess the Data
* Step 3: Define the Data Model
* Step 4: Run ETL to Model the Data
* Step 5: Project Write Up

### Step 1: Scope the Project and Gather Data

#### Scope 

- Explore and clean data using Apache Spark (PySpark) and validate that all data is in the expected format
- Partition data into .csv files using PySpark and load them into a data lake in Amazon S3
- Load data into an analytical datatabase in Postgres using parallell ETL with Python and AWS boto3 library

#### Gather Data  
* I've got an Artskart database-snapshot (.bak-file) containing all species observation until the 7. march 2021. 
* Artskart itself is a Microsoft SQL server relational datatabase where data is broken down into multiple different tables in 3NF.
* The `pre-process-data.ipynb` loads data from SQL Server into S3 using pyspark and AWS CLI:
![schematics](https://github.com/aletje/Artskart-Analytical-Database/blob/main/schematics.jpg "schematics")