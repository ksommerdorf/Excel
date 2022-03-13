# Analysis of Kickstarter Campaign Data
## Overview of Project
This project analyzes data from crowdfunding campaigns from various countries in order to find trends based on the outcome of the campaign. The focus of this project is to provide Louise trends in outcomes from other theater-related crowdfunding campaigns in order to help her play, Fever, met the funding goal. 
### Purpose 
The goal of this project is to improve Fever's crowdfunding campaign strategy in order to ensure the funding goal is met in time. This project will analyze the outcomes based on goals and outcomes based on launch date to find key patterns and trends. The final deliverable will be funding recommendations based on the concluded key insights. 
## Analysis and Challenges
The data set was downloaded as an .xlsx file and the data was resized in order to make the data and text more legible. The categories were changed to the appropriate data type, such as currency for 'goal' and 'pledge' amounts. Dates were formated uniformly for 'date created conversion' and 'date ended conversion' using the timestamp converter. 

Using conditional formatting I then color coded the four outcomes of the crowdfunding campaigns in order to make the results easier to distinguish.

I created a new column with the Percentage Funded and used conditional formatting in order to easily point out outliers with very high percentage funded and very low percentage funded. 

Next I created a new column with the average donation by dividing the pledged amount in column E by the number of backers in column L and rounding to the hundredths place. 

I then took the category and subcategory and split the data to separate the parent category from the subcategory. This the parent categories and subcategories to be filtered and singled out. 

A pivot chart was then created to analyze the different outcomes of each parent cateogry. Using this pivot table a graph was created and the theater category can be seen with not only the most outcomes but also the most successful outcomes. 

Narrowing the data down to Theater campaigns, the outcomes are shown based on the launch dates. The outcomes in this graph are successful, failed, canceled, and live. In order to narrow the data to only focus on outcomes instead of campaigns that are still ongoing, I filtered out the campaigns that are still "live".

### Analysis of Outcomes Based on Launch Date
This graph shows the outcomes of finished theater campaigns based on the launch month. The most successful campaigns occurred in May and June where the least amount of success was seen in December. December is the only month where the number of failed and the number of successful campaigns are almost equal. The most failed campaigns occurred in the month of October which also is the only month where there were no canceled campaigns. Based on this graph the ideal time to launch a crowdfunding campaign is in May and June and December and January are the most unfavorable. 


### Analysis of Outcomes Based on Goals
This data shows the percentage of successful, failed, and canceled campaigns in relation to the funding goal. The most successful campaigns have a low goal of less than 5000. Also campaigns with a goal between 35000 and 44999 also show almost the same success rate. Campaigns with a goal between 45000 and 49999 had a 100% failure rate but note that only 1 campaign had a goal between this value. More failures occur with a goal between 25000 to 34999 where out of 16 campaigns 12 failed. Therefore the smaller the asking amount, the more likely the campaign was able to reach the goal successfully. 

### Challenges and Difficulties Encountered
When finding the average donation by dividing the pledged amount by the number of backers some columns resulted in an error. This was solved by using the IFERROR() function in order to replace any errors with 0.
## Results
