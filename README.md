**Overview of the project**

**Purpose**

This analysis is conducted for various campaigns to illustrate how each campaign faired in relation to their launch dates and their fundraising goals for a client who estimates that her play to cost $12,000. The Kickstarter requires every campaign to have a fundraising goal. Additionally, the data set details the name of each campaigns, the money each campaign will need to success, the pledged amount of each campaign, the outcome of each campaign, and the country the campaign was started.

**Analysis and challenges**

**Analysis of Outcomes Based on Launch Date:**

Using the Kickstarter data, I first analyzed the month of each campaign using the Year() function to extract name of the month for ease of analysis of each outcomes based on launch date. I,then created pivot based on the outcomes of theatre campaigns and the month/date they were launched. The line chart depicts theatre outcomes based on launch date.

*The blue line plots the numbers of theatre campaigns that were successful for each month.

*The orange line plots the numbers of theatre campaigns that were failed for each month.

*The grey line plots the numbers of theatre campaigns that were canceled for each month.

![Picture1](https://user-images.githubusercontent.com/92557075/139522484-d636b750-b5b8-41d3-b6b8-08ea6bfe2f12.png)
**Analysis of Outcomes Based on Goals:**

Using the Kickstarter data set, I then analyzed outcomes based on goals where I created a new sheet to create the following columns to hold the date:

- Goal
- Number Successful
- Number Failed
- Number Canceled
- Total Projects
- Percentage Successful
- Percentage Failed
- Percentage Canceled

In the goal column, I created a following dollar amount ranges to group projects based on their goal amount.

![Goals](https://user-images.githubusercontent.com/92557075/139522566-9714e538-50c7-48ec-9bcc-15a0e5f7cc1a.png)


I used COUNTIFS(Sheet1!D:D,&quot;\&gt;1000&quot;,Sheet1!D:D,&quot;\&lt;=4999&quot;,Sheet1!F:F,&quot;Successful&quot;,Sheet1!Q:Q,&quot;Plays&quot;) to populate the &quot;Number Successful,&quot; &quot;Number Failed,&quot; and &quot;Number Canceled&quot; columns by filtering on the Kickstarter &quot;outcome&quot; column, on the &quot;goal&quot; amount column using the ranges and play as the criteria. Lastly, I Calculated the percentage of successful, failed, and canceled projects for each row.

![Picture3](https://user-images.githubusercontent.com/92557075/139522572-8e066d2f-a307-459f-9e7a-11017e16cc07.png)


**Challenges/difficulties:**

I did not encounter any challenges due to my vast experience with excel. The challenges that potentially could be identified is not using $ to lock the cells. This will save time and eliminate the possibility from showing the result derived using wrong columns.

Results:

Theatre outcome based on launch date:

1. Based on the analysis, I noticed that very few campaigns were cancelled in relation to other campaigns which were failed and successful.
2. Based on the analysis, I noticed significant increase during the month of May for all theatre campaigns that were successful and decline during the month of December. Additionally, I noticed significant increase during the month of May for all theatre campaigns that were failed and decline during the month of November.

Outcome based on Goals:

1. Based on the analysis using line chart, I noticed significant increase in the number of projects failed in the range of $45,000 - $49,999 range. Further, I noticed significant decrease in the number of projects successful in the range of $45,000 - $49,999 range.

Limitation of Data set:

The data provide an excellent insight into outcomes of each project based on the goal vs pledged amount as well as the outcomes based on each month. However, the limitation is that we do not have much insights as to why certain campaigns were successful than other which includes preferences or the type of advertising.

Suggested Additional Analysis:

I suggest we could have also used 3d clustered bar graph to present the analysis. Additionally, it would have been beneficial to present data by countries for a detailed analysis of outcomes on a country level.
