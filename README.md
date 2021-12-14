# "Analysis of Kickstarter Campaigns."

## Overview of Project

### Purpose

The purpose of this project is to analyse the data set, Kickstarter Campaigns, to help a playwright to start and succeed in a crowdfund campaign to get funds for her play, "Fever". Excel reatures (formulas, pivot tables, charts and graphs) are used in order to find the results of the analysis. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

The analysis of outcomes based on launch date started with the Kickstarter_Challenge.xlsx workbook, a new column was created and named "years", and the function "Year()" was used in order to extract the year from the “Date Created Conversion” column. After the extraction, a pivot table is created and added to a new sheet "Theater Outcomes by Launch Date". The table is filtered by "Parent category" and "Years". Placing the fields, "Outcomes" is added to Columns and Values, and "Date created a conversation" is added to rows. Column labels are filtered to show only "successful", "failed" and "canceled". And the "Parent Category" is filtered to show only the data for "theater."

After sorting the campaign outcomes to descending order, a line chart named "Theather Outcomes Based on Launch date" was created from the pivot table, as well, to vizualize the relationship between outcomes and launch months. 

![Theater_Outcomes_vs_Launch.png](path/to/Theater_Outcomes_vs_Launch.png)

Noticeble, the theather campaign is very successful and May is the most successful month. While June, July an August drop and have aproximately the same amount of failed campaigns. 
 
### Analysis of Outcomes Based on Goals

A new sheet named "Outcomes Based on Goals" was created to start the analysis. Eight columns were added to the sheet to hold the data: Goal, Number of successful, failed and canceled, total projects, percentage of successful, failed and canceled. The goal column had amounts added, as well.

The main function used to analyze and populate the number of successful, failed and canceled data, was "COUNTIFS()". Filtering by outcomes, goal and subcategory (using "plays" as the criteria).

After finding the number of the successful, canceled and failed campaigns, the "SUM()" function was used in order to find the total projects, based on the number of successful and failed, since the "plays" criteria had no canceled projects. The percentage was found dividing the number of successful, failed and canceled by the total projects.

The line chart was created and named "Outcomes Based on Goal", showing the percentage of successful, failed, or canceled projects and their goal amounts.

![Outcomes_vs_Goals.png](path/to/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

No challenges were faced during the "Outcome based on Launch Date analisys", the analysis is very easy to perform and the functions used in excel are simple and understandable. However, the "Outcomes based on goal" can be a little bit challenging if the data set is not right

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

Theather is the most popular and succesful campaign compared to other categories.  
May was the most successful month of the campaign, then the percentage drops in the later summer months. After August, the successful percentage drops drastically. 

- What can you conclude about the Outcomes based on Goals?

Upon visualisation of the line chart, we can see that the percentage of failed campaigns increases when the goal amount increases. Which makes a lower set goal more succesful, concluding that the reason of the unsuccessful campaigns it is because of overly ambitious financial goals. When campaigners set more realistic goals, they're more likely reach and even exceed. 

- What are some limitations of this dataset?

While I found this data set very useful in perfoming a broad analysis, I do believe some more qualititative data points could help in performing a more in depth analysis. One aspect missing is type of "incentive" for the kickstarter campaign. Perhaps some theaters gave away tickets, while others provided disocunts, or different swag. Incorporating this into the data could give further ideas for how to succesfuly raise funds.

- What are some other possible tables and/or graphs that we could create?

Successful, Failed and canceled Kickstarters based on country
Succesful, Failed, and canceled kickstarter campaigns based on average donation
Succesful, failed, and canceled campaigns based on backer count, put into bins of 10.

