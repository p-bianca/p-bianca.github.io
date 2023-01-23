---
layout: post
---

<body style="background-color:#006366;"></body>


## INTRODUCTION

## Bank Data Analysis Project

&emsp; <font size = "2">This is simpla a brief outline of the project as this particular project is company-related (and therefore proprietary). 
I've put this together by creating a relational database, running queries through SQL to gain meaningful insights and visualizing the data using Tableau. </font>

Examples of use cases: 
* <font size = "2">Outline the number of funded loans by underwriter on a monthly and yearly basis to measure output across the team to measure performance </font>
* <font size = "2">Determine the average interest rate by underwriter relative to the average rate across the entire team</font>
* <font size = "2">Rank the top 10 brokers by the number of loans funded for the year as well as the cumulative total dollar amount of funded loans to determine the bank's most productive relationships</font>
* <font size = "2">Isolate the percentage of deals declined relative to deals actioned by each underwriter to determine opportunities for coaching </font>
* <font size = "2">Measure the quality and accuracy of each underwriter based on their respective compliance scores for deals funded to determine opportunities for coaching </font>
* <font size = "2">List brokers by rate of declines relative to submissions to determine opportunities for coaching </font>

*****

## Mortgage Brokerage Analysis Project

&emsp; <font size = "2">As a quick synopsis, I created a relational database for mortgage brokerage. Only mock data was used in the creation of this project. </font>

<img src="https://imgur.com/a/vbw2WQ1" alt="Schema" style="height: 100px; width:100px;"/>

<img title="a title" alt="Alt text" src="C:\Users\pquib\OneDrive\Documents\portfolio\p-bianca.github.io\schema.png">

<img title="a title" alt="Alt text" src="p-bianca.github.io\schema.png">

![ttttext](https://github.com/p-bianca/p-bianca.github.io/blob/main/schema.png "a title")

## <font size = "2"> Using joins and aggregate functions </font>

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

<font size = "2"></font>

****


[back](./)


