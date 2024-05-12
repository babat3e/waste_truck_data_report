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
1. DimDate
<table>
<tr><td><b>DimDate</td></tr>
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
  


