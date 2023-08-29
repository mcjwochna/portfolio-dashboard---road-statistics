<h1>Portfolio - Road accidents dashboard</h1>


<h2>Introduction</h2>

> This is an analysis of the road incidents in the United Kingdom between January 1st, 2021 and December 31th 2022. It is based on a singular dataset, consisting of more than 307 000 rows. Each row was described by number of variables like: number of casualties, number of vehicles, date and time of the accident, road conditions, speed limit etc. I used this data to perform in-depth analysis of the most important statistics and present them in a user-friendly, functional visualizations.
<br>This particular dashboard also shows my ability to both create additional, necessary data (custom calendar table), manage relationships between tables and to use particular time-intelligence functions for getting the best, most useful insights.
![calendar_table](https://github.com/mcjwochna/portfolio-dashboard---road-statistics/assets/142684191/24d2274f-53ff-452c-8f5a-0cb4430d72fa)


<h2>Data Cleaning and Transformation</h2><br>

<b>This dataset was processed to obtain usable information by:</b><br>
>Removing rows consisting of empty values to acquire high-quality output,<br>
Transforming invalid text values (Accident_severity column),<br>
Removing redundant columns, to not negativly affect performance.

![data_clean](https://github.com/mcjwochna/portfolio-dashboard---road-statistics/assets/142684191/8c4c7868-d1d5-49d0-85dc-f4c2dac52d31)

![data_clean_2](https://github.com/mcjwochna/portfolio-dashboard---road-statistics/assets/142684191/226f8564-09d1-4334-b53c-2b98dd98b82d)
<br><br>
<b>All performed steps resulted in this accurate and comprehensive data used in further analysis:</b>
![data_clean_1](https://github.com/mcjwochna/portfolio-dashboard---road-statistics/assets/142684191/87b50ae7-34b9-4380-bf66-24bf58882460)


<h2>Problem statement</h2>

<b>The goal of this analysis is to:</b><br>
>Determine the information about current year casualties and accidents,<br>
Know the difference between casualties based on the level of injuries,<br>
Know the diffrence between current year and previous year accidents, to idicate year-over-year changes,<br>
Compare the data based on various informations like vehicle type or road type,<br>
Indicate the frequency of accidents, based on geographical data (map)<br>

<h2>Skills and Concepts demonstrated</h2>

<b>I used PowerBI functions/concepts like:</b>
>Creating key performance indicators (KPIs),<br>
Developing DAX calculations,<br>
Data Modelling,<br>
Measures,<br>
Filters,<br>
Custom tooltips,<br>
Data Visualization<br>

![custom1](https://github.com/mcjwochna/portfolio-dashboard---road-statistics/assets/142684191/989d24e6-0b91-4d12-8593-eccdd9ee437a)

![custom2](https://github.com/mcjwochna/portfolio-dashboard---road-statistics/assets/142684191/d98160a2-c941-4b99-ae83-ce71f2137ed5)

![custom3](https://github.com/mcjwochna/portfolio-dashboard---road-statistics/assets/142684191/4bfbbc56-fab9-4fe7-8d38-1990008aee44)

<h2>Data Analysis</h2>

<b>Several expressions and functions were used for the desired KPI. Just to name a few:</b><br>
> CY Accidents = TOTALYTD(COUNT(Data[Accident_Index]),'Calendar'[Date]),<br>
PY Casulties = CALCULATE(SUM(Data[Number_of_Casualties]),SAMEPERIODLASTYEAR('Calendar'[Date])),<br>
YoY Casulties = DIVIDE([CY Casualties]-[PY Casulties],[PY Casulties])]


![kpi](https://github.com/mcjwochna/portfolio-dashboard---road-statistics/assets/142684191/ec467dd5-635f-400a-aa3c-57c1a6fd9912)
