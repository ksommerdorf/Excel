# Analysis of Kickstarter Campaign Data
## Overview of Project
This project analyzes data from crowdfunding campaigns from various countries in order to find trends based on the outcome of the campaign. The focus of this project is to provide Louise trends in outcomes from other theater-related crowdfunding campaigns in order to help her play, Fever, met the funding goal. 
### Purpose 
The goal of this project is to improve Fever's crowdfunding campaign strategy in order to ensure the funding goal is met in time. This project will analyze the outcomes based on goals and outcomes based on launch date to find key patterns and trends. The final deliverable will be funding recommendations based on the concluded key insights. 
## Analysis and Challenges
![Module1 1](https://user-images.githubusercontent.com/57520471/158078910-1e80bb6f-edda-45dd-bfb9-480c10f86b04.png)
![module1 2](https://user-images.githubusercontent.com/57520471/158078912-cda395c4-25bc-4613-9d78-aa173b2d27ed.png)
* The data set was downloaded as an .xlsx file and the data was resized in order to make the data and text more legible. The categories were changed to the appropriate data type, such as currency for 'goal' and 'pledge' amounts. Dates were formated uniformly for 'date created conversion' and 'date ended conversion' using the timestamp converter. 

![module1 3](https://user-images.githubusercontent.com/57520471/158078913-a48d052d-e7fb-4558-92c5-e5a93cd714b3.png)
![module1 4](https://user-images.githubusercontent.com/57520471/158078914-f42bbf05-6e1e-47df-8701-373f36307d33.png)

* Using conditional formatting I then color coded the four outcomes of the crowdfunding campaigns in order to make the results easier to distinguish. 
Then I created a new column with the Percentage Funded and used conditional formatting in order to easily point out outliers with very high percentage funded and very low percentage funded. 
* Next I created a new column with the average donation by dividing the pledged amount in column E by the number of backers in column L and rounding to the hundredths place. 
* I then took the category and subcategory and split the data to separate the parent category from the subcategory. This the parent categories and subcategories to be filtered and singled out. 

![module1 5](https://user-images.githubusercontent.com/57520471/158078915-3f70729b-a7d2-4403-b3ad-917d6653bad7.png)

* In order to determine the statistical significance of the data, the mean, median, standard deviation, and IQR were calculated for both successful and failed outcomes in the goal and pledged category for plays. The standard deviation in compared to the IQR has the greatest difference in the failed kickstarters. Which means some of the failed campaigns had very high goals. The mean of each of the successful and failed kickstarters in the goal and pledged categories is around the 3rd (upper) quartile. Therefore both sets of data have similar distributions which means the pledged and goal data follow the same trends.

![Outcomes_based_on_launch_date_theater](https://user-images.githubusercontent.com/57520471/158078597-a8189bf7-ea9e-4db4-bc09-da0aedcf0c14.png)

* A pivot chart was then created to analyze the different outcomes of each parent cateogry. Using this pivot table a graph was created and the theater category can be seen with not only the most outcomes but also the most successful outcomes. 

![parentcateogryoutcomes1](https://user-images.githubusercontent.com/57520471/158078566-016a8133-6242-486d-9612-70d436c5b6cf.png)

* Narrowing the data down to Theater campaigns, the outcomes are shown based on the launch dates. The outcomes in this graph are successful, failed, canceled, and live. In order to narrow the data to only focus on outcomes instead of campaigns that are still ongoing, I filtered out the campaigns that are still "live".

### Analysis of Outcomes Based on Launch Date
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/57520471/158076909-1a239b96-8ab1-4862-94bc-50346433b8df.png)
This graph shows the outcomes of finished theater campaigns based on the launch month. The most successful campaigns occurred in May and June where the least amount of success was seen in December. December is the only month where the number of failed and the number of successful campaigns are almost equal. The most failed campaigns occurred in the month of October which also is the only month where there were no canceled campaigns. Based on this graph the ideal time to launch a crowdfunding campaign is in May and June and December and January are the most unfavorable. 


### Analysis of Outcomes Based on Goals
![outcomes_vs_goals](https://user-images.githubusercontent.com/57520471/158076907-3342bc07-3148-4249-b6f8-514a0b6ec806.png)
This data shows the percentage of successful, failed, and canceled campaigns in relation to the funding goal. The most successful campaigns have a low goal of less than 5000. Also campaigns with a goal between 35000 and 44999 also show almost the same success rate. Campaigns with a goal between 45000 and 49999 had a 100% failure rate but note that only 1 campaign had a goal between this value. More failures occur with a goal between 25000 to 34999 where out of 16 campaigns 12 failed. Therefore the smaller the asking amount, the more likely the campaign was able to reach the goal successfully. 

### Challenges and Difficulties Encountered
When finding the average donation by dividing the pledged amount by the number of backers some columns resulted in an error. This was solved by using the IFERROR() function in order to replace any errors with 0.
## Results
### Conclusions:
* Campaigns have a higher success rate when launched in May and June. This could be in correlation to the start of nice weather or the beginning of summer. In the summer more people are likely to spend money on extra activities such as campaign funding.
* The most failed comapaigns occur in December and January. These results are likely due to people having other financial obligations that occur in the month of December and January such has Christmas and/or New Years Eve. Therefore campaigns started during these months do not have much success. 
* Successful campaigns also have lower goals (lower than 1000) which means that campaigns are more likely to fail if they ask for too much money. Therefore the outcomes would be more favorable to have smaller crowdfunding campaigns rather than one with a large goal. 

### Limitations/Future Suggestions:
* In the Outcomes Based on Goals graph, the data surrounding the goal amount is in different currency. Therefore the graph does not take into account of the different currencies value differences and the country's economic staus either. This graph also does not take into consideration the average donation or how many backers pledged. Lastly, this graph only shows the outcomes but does not consider the length of the campaign. In order to take away these limitations the data should be broken down by country with similar median income and currency should converted to USD to make the numbers more comparible. Also there should be a graph that compares the outcomes to the length of the campaign.
* In the Outcomes Based on Launch Dates, the graph does not consider the different yearly cultural events that occur in the countries that could be contributing to the results. Therefore the country that Fever's campaign took place in should also be isolated into a separate graph to be able to observe the similar or differences in the trends. 
* This data does not include the different tactics each campaign took that may have helped or hindered the outcome. 
