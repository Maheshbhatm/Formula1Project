# Formula1Project
<div id="header" align="center">
  <img src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif" width="100"/>
</div>

<div id="badges">
  <a href="https://www.linkedin.com/in/maheshbhatm/">
    <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
  </a>
</div>
 

<h3>Overview</h3>

Formula One is the highest class of international racing for open-wheel single-seater formula racing cars. Every season happened once a year, each race happened over weekends (Friday to Sunday). Each race is conducted in individual circuits. 10 Teams/Constructors will be participated. 2 Drivers will be assigned in a team. Saturday will be a qualifying round for the Sundays match. 50-70 Laps will be there on each race. Pitstop will be available to change tire or damages. Race results included driver standing and constructure standing.


<h3>Source Date Files</h3>
We are referring open-source data from website Ergast Developer API. Data available from 1950 till 2022.


| File Name  | File Type |
| ------------- | ------------- |
| Circuits  | CSV  |
| Races | CSV |
| Constructors  | Single Line JSON  |
| Drivers | Single Line Nested JSON |
| Results  | Single Line JSON  |
| PitStops | Multi Line JSON |
| LapTimes  | Split CSV Files  |
| Qualifying | Split Multi Line JSON Files | 

Qualifying 	Split Multi Line JSON Files

Data Model (http://ergast.com/images/ergast_db.png)

![Azure Architecture](https://user-images.githubusercontent.com/44454642/201458776-a8f93591-848a-41b1-b9a0-9d1c52ad5d7b.png)


<h3>Data Ingestion Requirement</h3>
<ul>
  <li>Ingest All 8 Files into the data lake </li>
  <li>Ingested data must have the schema applied </li>
  <li>Ingested data must have audit columns </li>
  <li>Ingested data must be stored in a columnar format</li>
  <li>Must be able to analyze the ingest data </li>
  <li>Ingestion logic must be able to handle incremental load</li>
</ul> 

<h3>Data Transformation Requirements</h3>
<ul>
  <li>Join the key information required for reporting to create a new table</li>
  <li>Join the key information required for analysis to create a new table </li>
  <li>Transformed tables must have audit columns </li>
  <li>Must be able to analyze the transformed data via SQL</li>
</ul> 

<h3>Reporting Requirements</h3>
<ul>
  <li>Driver Standing </li>
  <li>Constructure Standing</li> 
</ul> 

<h3>Analysis Requirements</h3>
<ul>
  <li>Dominant Drivers </li>
  <li>Dominant Teams </li> 
  <li>Visualize the output </li>
  <li>Create Databricks Dashboard</li> 
</ul> 

<h3>Scheduling Requirements</h3>
<ul>
  <li>Scheduling to run every Sunday 10PM</li>
  <li>Ability to monitor pipelines </li> 
  <li>Ability to re-run failed pipelines </li>
  <li>Ability to set-up alerts on failures </li> 
</ul>  

<h3>Technologies/Tools Used:</h3>
<ul>
  <li>Pyspark</li> 
  <li>Spark SQL</li> 
  <li>Delta Lake</li> 
  <li>Azure Databricks </li> 
  <li>Azure Data Factory</li> 
  <li>Azure Date Lake Storage Gen2</li> 
  <li>Azure Key Fault</li> 
  <li>Power BI</li> 
</ul>  
