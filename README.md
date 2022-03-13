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

Narrowing the data down to Theater campaigns, the outcomes are shown based on the launch dates. The most successful campaigns occurred in May and June where the least amount of success was seen in December. December is the only month where the number of failed and the number of successful campaigns are almost equal. In all other states the number of successful campaigns and failed campaigns follow a similar pattern.


### Analysis of Outcomes Based on Launch Date
### Analysis of Outcomes Based on Goals
### Challenges and Difficulties Encountered
When finding the average donation by dividing the pledged amount by the number of backers some columns resulted in an error. This was solved by using the IFERROR() function in order to replace any errors with 0.
## Results
