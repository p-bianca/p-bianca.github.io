---
layout: post
---

<body style="background-color:#006366;"></body>


## BANK DATA ANALYSIS PROJECT

&emsp; <font size = "2">This is simply a brief outline of the project as this particular project is company-related (and therefore proprietary). 
I've put this together by creating a relational database, running queries through SQL to gain meaningful insights and visualizing the data using Tableau. </font>

Examples of use cases: 
* <font size = "2">Outline the number of funded loans by underwriter on a monthly and yearly basis to measure output across the team to measure performance </font>
* <font size = "2">Determine the average interest rate by underwriter relative to the average rate across the entire team</font>
* <font size = "2">Rank the top 10 brokers by the number of loans funded for the year as well as the cumulative total dollar amount of funded loans to determine the bank's most productive relationships</font>
* <font size = "2">Isolate the percentage of deals declined relative to deals actioned by each underwriter to determine opportunities for coaching </font>
* <font size = "2">Measure the quality and accuracy of each underwriter based on their respective compliance scores for deals funded to determine opportunities for coaching </font>
* <font size = "2">List brokers by rate of declines relative to submissions to determine opportunities for coaching </font>

*****

## MORTGAGE BROKERAGE ANALYSIS PROJECT

## SQL Portion

&emsp; <font size = "2">As a quick synopsis, I created the below relational database for mortgage brokerage. Only mock data was used in the creation of this project. </font>

<img src="schema.png" width="800" />

Below are quick links to the tables for reference. 

[Download link - deals raw data CSV file](./deals.csv)   
[Download link - brokers raw data CSV file](./brokers.csv)       
[Download link - institutions raw data CSV file](./institution.csv)  
[Download link - clients raw data CSV file](./clients.csv)    

## <font size = "2"> Using joins and aggregate functions </font>
In this example, I ran the below query to list the top 10 brokers by total deals (includes all funded, approved, declined and cancelled deals).

```sql
SELECT 
    name, COUNT(*) AS totaldeals
FROM
    brokers
        JOIN
    deals ON brokers.id = deals.brokerid
GROUP BY name
ORDER BY totaldeals DESC LIMIT 10;
```

## Data Visualization

<img src="tableau1.png" width="800" />
<img src="tableau2.png" width="800" />
<img src="tableau3.png" width="800" />
<img src="tableau4.png" width="800" />


<font size = "2"></font>

****


[back](./)


