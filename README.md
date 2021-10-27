# Kickstarting with Excel

## Overview of Project

### Purpose

This project is a continued dive into Excel using Pivot Tables and Functions to analyze the sucess of various existing kickstarter campaigns to try and deduce what the best course of action for someone who is trying to to understand how different variables, like Launch Date of the campaign or the monetary goal of a theater or play project. Then, once the data is analyzed, the purpose of the project is to present the data in a simple way, using tables and charts, to most effectively portray the outcomes.  

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

The first task of the project was to analyze how effective each Theater campaign was depeneding on the launch date. In order to do this, I created a pivot table utilizing the columns "Parent Category", "Years", "Outcomes", and "Date Created Conversion" of the main Kickstarter Data set. Using "Parent Category" and "Years" as filters for the Pivot Table, we can get a tidy visulization of what the breakdown of the results of each Theater Kickstarter campaign month by month. The values of the pivot table comprise of the count of each outcome broken up by month. The pivot table can bee seen below. 

<img width="325" alt="OutcomesByLaunchDatePivot" src="https://user-images.githubusercontent.com/92888170/139148777-bb14b727-7f82-4742-af32-b4d85752fa1b.png">

A line graph visulization is another way to view the data in a digestable way. This chart below can also be found in the Resources folder also includeded in this repository.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/92888170/139150716-c85a1ebb-24e0-44d3-a344-48a14d4ed67e.png)


### Analysis of Outcomes Based on Goals

The second task of the project was to analyze how effective each Theater campaign was depending on the amount of money the project's goal was to raise. To accomplish this, I first had to organize the data into a form that aligned with what I wanted to figure out. I started by creating a chart, where the columns were the Goal of the project, broken up into different sized bins. I then used Excel's countifs function to parse through the Kickstarter data sheet to count the total number of sucessful, failed, and canceled play Kickstarters. Using this counted data, I was able to figure out what percent of each play was sucsessful, failed, or canceled based on how much money it was asking for. Below is the table I made and a line graph representation of the table. The line graph can also be found in the resources folder in the Kickstarter Analysis Repository.

<img width="614" alt="OutcomesBasedOnGoalsTable" src="https://user-images.githubusercontent.com/92888170/139156785-9bcc853f-927a-4da1-9990-5eb4e22f675a.png">

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/92888170/139157086-dbb0d59c-63a9-4791-8287-b54806abde8c.png)



### Challenges and Difficulties Encountered

One challenge I had was during the second deliverable, I couldn't seem to get the total number of plays to be the correct count. This issue ended up being one that I solved after taking a break after looking over the data. When I came back to it, I realized that my Countifs functions weren't taking in account the fact that I also needed to sort by category, So I was counting every single kickstarter that had an outcome, not just the ones in the cateogry of theater/play. Another challenge I ran into was trying to sort the Pivot Chart of the Outcomes based on Launch Date so that the first column was the successful outcome, followed by the failed then canceled outcomes. I was able to fix this issue by looking up agian how to sort a pivot chart's columns by right clicking the columns headers, then sorting by descending order. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The first thing that becomes immediately obvious while observing the chart is that the most successful month to Launch a Theater campaign is May, with 111 out of 166 Theater Kickstarters reaching their goal of funding. This suggests that the best time to start a theater kickstarter is in May. Also, every single month ended up with more successful Kickstarters than failed Kickstartes in the Theater category, with the month of December having the smallest difference between the successful and the failed campigns. This suggests that when it comes to choosing categories, theater seems to perform well on the platform. 

- What can you conclude about the Outcomes based on Goals?

Based on the line graph of the Outcomes based on Goals, we can conclude an interesting result. It appears that the cheaper projects have a much higher rate of success compared to the campaigns with lofier goals. Projects that have a goal of $5,000 or less have a success rate of above 70%. This level of sucess isn't seen until much more expensive Goal ranges, but those goal ranges are skewed by a smaller sample size. There are only a few plays in the $35,000 to $50,000 goal range, even though they have a success rate of 66% 

- What are some limitations of this dataset?

Some limitations of the data sets include the fact that there are not many play kickstarters that have a high price goal. The few that did, ended up making it too their goal, but I don't think this is necessarily an outcome we can rely, because the sample size is so small. Another limitation on this data set is the fact that it only comes from one website source, Kickstarter. If we wanted to get a more accurate depiction of what works well for campaigns, we could get data from another crowdfunding website to add to the depth of data that we analyzed. 

- What are some other possible tables and/or graphs that we could create?

 Some other possible tables that we could include could be seeing the success based on the country of origin. I think it would be important to figure out of the place you are trying to get the project funded has an appeal and suitible demographic for the idea. Another table that we could create would be to compare whether the staff picked the project and if it ended up being funded. I think that it's important to figure out the relationship between what the platform thinks is a good pick versus what the public ends up choosing to fund. 
