# Kickstarting with Excel: An Analysis of Kickstarter Campaigns.
  
  
## Overview of Project
A client has recently concluded a crowdfunding campaign that did not reach its funding goals. In order to uncover crowd-fundraising campaign performance trends based on launch dates and initial funding goals of similar projects that would have successful outcomes, a series of computations and charts were completed in excel. While the Kickstarter data set included a wide variety of projects ranging from food and games to film, the majority of the analysis was performed using projects in the theater and plays categories.
### Purpose
 Assist the client develop a better understanding of factors that could improve success rates in their future campaigns.  
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The data set included launch and ending Unix timestamps that were covered to calendar dates. A pivot table was created using the theater parent category and years as filters, the outcomes (success, failure, or canceled) in the columns, date launched as rows, and count of outcomes as the values. 
<br/>
<img width="330" alt="Pivottbl" src="https://user-images.githubusercontent.com/91163155/135775296-db2bf3c9-121a-4706-84b8-2581fbe9bae9.png">


From this table, a pivot chart was created, where the campaign launch month versus outcomes is visually depicted. 
<br/>
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/91163155/135775346-2d6aa4d4-1e94-4bc3-a7f9-8c9999aeeddc.png)


### Analysis of Outcomes Based on Goals
To identify the impact of the funding goal on project outcomes, the goal values were broken into 12 categories, ranging from less than $1,000 to greater than $50,000. The percentage of successful and failed campaigns in each interval were calculated in a table and a line chart was produced.
<br/>
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/91163155/135775372-d2375199-d10e-4d2c-8be3-06d04c4166f4.png)


### Challenges and Difficulties Encountered
Ensuring that the count of projects was accurate for each interval was challenging, as the counter utilized several bounds and criteria in each cell. To ensure the more complex countifs statements were functioning correctly, simpler countifs statement like the total number of plays were compared compared to the total number of plays using sum statements. Once a baseline had been established, I was able to check the results to the original Kickstarter data set and confirm accuracy. 
<br/>

## Results

From the outcomes base on lanch date chart, we can conclude that campaigns lauched in the early summer (May-June) have the highest success rates, while December has the lowest successful outcomes. 

Overall, projects with fundraising goals less than $15,000 have higher success rates, and lower success rates with goals higher than $15,000, especially true for very high ($45,000+) goals.  
Limitations of this dataset include the time frame- it is limited to the years 2009 to 2017, while information from 2017-present would be the most useful to understanding recent funding trends. 
It would be interesting to see how project themes (derived form the "blub" sections) would relate to outcomes.
