# waste_truck_data_report
Use data warehouse skills to design and implement a data warehouse that tracks waste collected by major cities in Brazil.

## IBM Data Warehousing and Business Intelligence Analytics Capstone Project
This repository is part of the IBM Data Warehousing and Business Intelligence Analytics project. 

## Scenario
You are a data engineer hired by a solid waste management company. The company collects and recycles solid waste across major cities in the country of Brazil. The company operates hundreds of trucks of different types to collect and transport solid waste. The company would like to create a data warehouse so that it can create reports like below;
<table>
<tr><td>total waste collected per year per city</td></tr>
<tr><td>total waste collected per month per city</td></tr>
<tr><td>total waste collected per quarter per city</td></tr>
<tr><td>total waste collected per year per trucktype</td></tr>
<tr><td>total waste collected per trucktype per city</td></tr>
<tr><td>total waste collected per trucktype per station per city</td></tr>
</table>
You will use your data warehousing skills to design and implement a data warehouse for the company.

## Objectives
* Design a Data Warehouse
* Load data into Data Warehouse
* Write aggregation queries
* Create MQTs
* Create a Dashboard

## Tools and Technologies
* RDBMS: PostgreSql
* Staging - Data warehouse – PostgreSQL
* Business Intelligence Dashboard - IBM Cognos Analytics

## Star Schema for Data Warehouse
### Dimension Tables
1. <b>DimDate</b>
<table>
<tr><td>dateid</td></tr>
<tr><td>date</td></tr>
<tr><td>year</td></tr>
<tr><td>quarter</td></tr>
<tr><td>quartername</td></tr>
<tr><td>month</td></tr>
<tr><td>monthname</td></tr>
<tr><td>day</td></tr>
<tr><td>weekday</td></tr>
<tr><td>weekdayname</td></tr>
</table>
Data Source: <a href="https://github.com/babat3e/waste_truck_data_report/blob/fe8f3759298b5bcede6bc917ffd607362ea79690/DimDate.csv">DimDate</a><br>

 2. <b>DimTruck</b>
<table>
<tr><td>truckid</td></tr>
<tr><td>trucktype</td></tr>
</table>
Data Source: <a href="https://github.com/babat3e/waste_truck_data_report/blob/2d32a1ed5e69c61a820528488f9c43523fdbc81e/DimTruck.csv">DimTruck</a><br>

 3. <b>DimStation</b>
<table>
<tr><td>stationid</td></tr>
<tr><td>city</td></tr>
</table>
Data Source: <a href="https://github.com/babat3e/waste_truck_data_report/blob/b1c4bed1f1c69bf9f97cb733fac4b18e86c3e9d8/DimStation.csv">DimStation</a><br>

### Fact Table
 1. <b>FactTrips</b>
<table>
<tr><td>tripid</td></tr>
<tr><td>dateid</td></tr>
<tr><td>stationid</td></tr>
<tr><td>truckid</td></tr>
<tr><td>wastecollected</td></tr>
</table>
Data Source: <a href="https://github.com/babat3e/waste_truck_data_report/blob/18972ade5837da257cfea4957dccf3ac6088d17d/FactTrips.csv">FactTrips</a>
  


