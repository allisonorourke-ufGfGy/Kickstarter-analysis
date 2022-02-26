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
#### I struggled a bit with understanding the 
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
    

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
