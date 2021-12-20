# Kickstarter Analysis with Excel

## Overview of Project
In this scenario, we have been following the prospective client, Louise, as she attempts to make a decision on her kickstarter campaign based off of data that is available. This data is multifaceted, showing the monetary values associated with projects, whether successful or not. Now Louise would like to know how theater project outcomes are correlated with launch dates and funding goals. Utilizing the data at hand, we will analyze and answer her inquiry to the best of our abilities. 

### Purpose
We will analyze the Kickstarter_Challenge data within the parameters that the client was interested in - namely, launch dates and funding goals. This, in turn, will allow us to consider the outcome of a theater project (whether successful, canceled, or failed) in relation to its launch date and associated funding goal. After this data has been obtained and depicted, we will provide a clear analysis for the prospective client - so that she may make a decision of her own.

## Analysis and Challenges
As mentioned previously, we wanted to present an analysis that shows the relationships present between theater outcomes, launch date, and goals. We approached this in a two-prong manner, with seperate sections of analysis. 

### Analysis of Outcomes Based on Launch Date
We changed the timestamps in the original dataset to a recognizable format and used Excel capabilites to filter the data based on launch date. To execute this, we made a pivot table so as to efficiently isolate and analyze the different variables in the dataset. We then grouped the dates into months of the year, so that the pivot table showed the number of canceled, failed, and successful outcomes relative to each month. Furthermore, we put the numbers of each outcome column in descending order to pave the way for a nice depiction of the data. As such, we then created a line chart that showed "Theater Outcomes Based on Launch Date."

![Theater_Outcomes_vs_Launch_Data](https://github.com/JV348/kickstarter-analysis/blob/c63905168076e5f2373dfeca756d910afca16370/Resources/Theater_Outcomes_vs_Launch_Data.png)


![Theater_Outcomes_vs_Launch](https://github.com/JV348/kickstarter-analysis/blob/c63905168076e5f2373dfeca756d910afca16370/Resources/Theater_Outcomes_vs_Launch.png)

Derived conclusions in Results 


### Analysis of Outcomes Based on Goals
After analyzing the previous data trend, we shifted over to the relationship between theater project outcomes and their monetary goal. We created a new Excel sheet and established twelve dollar-amount goal ranges from less than 1000 to greater than 50000. Afterwards, we created columns for the number of failed, canceled, and successful outcomes followed by their respective percentage columns. This in turn paved the way for the COUNTIFS() function. We used Excel commands in this function to filter the Kickstarter_Challenge data for a number output on a specific type of outcome within a goal range. 

![Outcomes_vs_Goals_Data](https://github.com/JV348/kickstarter-analysis/blob/c63905168076e5f2373dfeca756d910afca16370/Resources/Outcomes_vs_Goals_Data.png)

Once we had the numbers of each outcome for each goal range, we used simple math functions to add the Total Projects and then found the percentages of each outcome type in each goal range. This table of data then allowed us to create a line chart depicting "Outcomes Based on Goal."

![Outcomes_vs_Goals](https://github.com/JV348/kickstarter-analysis/blob/c63905168076e5f2373dfeca756d910afca16370/Resources/Outcomes_vs_Goals.png)

Derived conclusion in Results
 

### Challenges and Difficulties Encountered
In Deliverable 1, the first obstacle was the Epoch timestamp. In order to present the launch dates, the timestamp in the dataset needed to be converted. To do this, online assistance was used, and the timestamp listed for each project was converted into a regular date in a new column. The YEAR() function was then used to extract the date from the new "Date Created Conversion" column. Only then could we move foward with the analysis and chart. 

In Deliverable 2, the greatest obstacle was ensuring that the Excel commands were typed correctly in the COUNTIFS() function. A considerable amount of time was lost backtracking, dictating rules, and monitoring for further errors. In short, Google was used to figure out some minor things about Excel, like the way we are supposed to type greater than or less than. 


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

Based on the depiction provided by the chart, we can acknowledge that most projects launch in the middle of the year, peaking in the Summer around May to July. This trend is evident with Successful and Failed Outcomes as much of their data falls on those Summer months. 
This trend is not as evident with Canceled Outcomes, as it appears that Launch Date is not very indicative of whether a theater project will be canceled. 

- What can you conclude about the Outcomes based on Goals?

According to the data, over seventy percent of successful theater outcomes are found in the lower goal ranges. Generally, the greater the  monetary goal, the more likely the project is to fail. Of course, this is not always the case, as some projects succeed despite having large goals. It is worth noting that some expensive and successful projects have a greater number of financial backers. This may help explain the trend reversal that occurs around 30000. 
Nonetheless, it is clear that the Percentage Successful reciprocates the Percentage Failed, as they maintain an opposite relationship. On the other hand, Percentage Canceled does not seem to show a clear relationship between goal and outcome. It is possible that a lack of donors/backers is more related to that issue. 

- What are some limitations of this dataset?

The dataset that we are using for analysis is actually a theater subset of the Kickstarter_Challenge data, and therefore it is arguably a smaller sample size. As such, the analysis may not accurately convey real world relationships nor those relationships that would be present in the original dataset. Furthermore, the variables chosen to be analyzed are also a limiting factor - as there are many variables to consider and we have decidedly cut out a lot of data to analyze very specific parameters. For instance, it would have been beneficial to look at the number of financial backers in this analysis. 

- What are some other possible tables and/or graphs that we could create?

It would be relevant to this analysis to include the number of backers. Along those lines, a table and/or graph that shows the relationship between Theater Outcomes and Number of Backers would be appropriate. It would also be appropriate to analyze the country of origin, as that gives insight to the culture and market that will sustain a theater project. Another table and/or graph that depicts the relationship between country and theater outcome would be helpful as well. 
