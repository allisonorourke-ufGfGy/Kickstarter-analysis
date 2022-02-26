# Kickstarting with Excel

## Overview of Project

### Purpose
#### The purpose of this experiment is to help a prospective client by analyzing trends from Kickstarter data to understand different variables that might affect the success of her project.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
#### I first began this analysis by looking at the different outcomes of Kickstarters based on the month that they were launched in. I broke it down to look at campaigns based on their status as 'successful', 'failed', or 'canceled'. I then looked at the month which the campaign was started. I did this through a pivot table which had parent category and years in the filter, outcomes in columns, date created conversion in rows, and count of outcomes in the values. When I created a graph, as seen below, I was able to see that May ans June were the most successful months to launch a campaign because they had the highest count of 'successful' campaigns. The number of 'failed' plays was pretty consistent throughout with May and October having slightly higher rates of those campaigns.

![Theater Outcomes based on Laucnh Dates](https://github.com/allisonorourke-ufGfGy/Kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
####  I also wanted to look at that outcomes of different campaings based on their monetary goal. This was accomplished through the COUNTIFS function in excel. This was applied to a range of goals that were $4,999 apart. I then also broke it doen by the number successful, failed, and canceled. This was done through the following formula as one of the examples to count the number of canceled plays whose goal was $5000 to $9999.
=COUNTIFS(Kickstarter!$D:$D, ">=5000",Kickstarter!$F:$F, "canceled", Kickstarter!$D:$D, "<=9999", Kickstarter!$R:$R, "plays")
After the total was take of each a percentage of successful, failed, and canceled was calculated for each goal range. This was then graphed into the following table. This shows that a project is more likely to succeed if the goal is under $15,000 or $35,000-$40,000. Anything not in that rate is more likely to fail than to succeed.

![Outcomes Based on Goal](https://github.com/allisonorourke-ufGfGy/Kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
#### I struggled a bit with understanding the COUNTIFS formula. I struggled with understanding which columns to assign to each conditional. This was then solved by watching Youtube videos on this formula and trouble shooting. I also was having issues understanding Github and how to upload a Readme file but that was overcome by using the information in the Slack, watching Youtube, and going to office hours.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
    1. May and June are the best months to launch a campaign to have the highest chance of success.
    2. December is the worst months to launch a campaign because it has a low rate of success and an almost equal rate of failed.

- What can you conclude about the Outcomes based on Goals?
    1. A project is most likely to succeed if the goal is under $15,000 or $35,000-$40,000
    2. A project is most lieekly to fail if the goal is $45,000 and over.
    
- What are some limitations of this dataset?
    This data set does not take into account any of the external factors that were going on at the time. Things such as recessions or pandemics may affect data like this and         skew it. After the COIVD pandemic the play industry is probably very different and all the data in this set is from before that time so it would be very helpful to get some     more recent data.I also think it would be good to get a better understanding of the genre of the play to see if a thriller would do better/ worse than a comedy. The type of     play can have a large affect on how many people would come to see it. Finally, this data set only looks at Kickstarter data. It would be nice to look at different platforms     that can be used to fund a play to see if there is benefit to using one over the other.
    
- What are some other possible tables and/or graphs that we could create?
    1. I would like to look at the different success rates base on different countries to see if there is a benefit to launching in one country over another. This could be done        with a pivot table and then a stacked column graph based on country and then count of successful, failed, and canceled
    2. I would like to look at the success/ fail rates of musicals vs plays as they are in the same parent category to see if there is a favorite. This could be done by doing          COUNTIFS formula to determine the count of success or fail in each sub category.
    3. I would like to look at the average donations based on the goal set to see if the goal plays any affect on the amount people are willing to donate.This could be done by          using a VLOOKUP formula.
