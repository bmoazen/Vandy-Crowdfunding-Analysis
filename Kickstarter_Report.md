# Kickstarting with Excel

## Overview of Project
The purpose of this analysis was to look at differmt factors which may play a role in whether or not a Kickstarter fundraising goal is successful.  This can aid Louise in her second attempt to fund her play "Fever".
### Purpose

## Analysis and Challenges
First, I created a pivot table to look at outcomes by launch date, focusing on Kickstarter projects with category "Theater".  This table is avaliable in the Kickstarter_Challenge excel sheet in my Vandy_Crowdfunding_Analysis repository.  This pivot tabvle was used to create the "Theater Outcomes vs Goals" graph.  I also filtered the data by the subcategory "Plays" and looked at the success of projects based on the fundraising goal.  I used this data to create a plot of "Outcomes vs Goals" which looks at successful, failed, amnd canceled play projects as a function of fundraising goal.

One challenge I encoutered was when I created the tables for outcomes based on goal.  I noticed that the total number of plays (successful plus failed plus canceled) was too low.  After looking at the "COUNTIFS" function, I realized that my lower end conditional needed to be greater than OR equal to the lower amount.  Due to it only being greater than, many plays were not being included in the calculation, since many of them had a goal that was equal to the conditional test.

### Analysis of Outcomes Based on Launch Date
Though most theater projects do meet their fundraising goal, it seems that projects launched in May, June, and July have a particularly high success rate, especially May.  Overall, approximately 61 percent (standard deviation of 5 percent) of all thater Kickstarter projects reach their fundraising goal, however, in May that percentage was slightly higher, at roughly 67 percent (1.2 standard deviations away from the mean).  This seems to suggest that May could be an advantageous time to start a Kickstarter Campaign for a play.  

### Analysis of Outcomes Based on Goals
It certainly seems that plays that have lower fundraising goals do much better.  Up to fundraising goals of $15,000, plays have a better than 50 percent chance of meeting their goals.  Higher than $15,000 and plays are more likely to fail at their campaign.  However, it does seem that there may be a "sweet spot" between $35,000 and $44,999 where the success rate go back over 60 percent.  Perhaps people are more likely to see a play in that range as being higher quality and thus more worthy of funding?

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
    May is the month in which the most Kickstarter campaigns under the category "Theater" are started.  This month also has the highest success rate compared with other months.

- What can you conclude about the Outcomes based on Goals?
    Overall, success rate decreases with increasing fundraising goal, except for a jump between $35,000 and $44,500.  This suggests there is perhaps a "sweet spot" for fundraising goals.

- What are some limitations of this dataset?
    This seems like a fairly robust data set.  While there is data for the total pledged for each project as well as the number of backers, this can pnly give us the average pledge.  It would be very helpful to have some sense of the spread in the donations, either the interquartile range or the standard deviation.  This could help us determine how these projects are being funded.  Is the majority of the money coming from many of the backers or is most of the money coming from just a handful of backers ("heavy hitters").  This could help us in our ficus: are we trying to appeal to many backers or trying to find just a few big donors?

- What are some other possible tables and/or graphs that we could create?
    Instead of looking at the raw numbers for the theater outcomes and launch date, using percentages would be much better.  May had the most successsful campaigns, but it also had the most launches.  Looking at the success rate is what really determines that May is the best month.  Also perhaps looking at launch date by year.  Is the success rate for plays improving over the years?  How is the rate by fundraising goal changing?  How about backers of plays by year?  Are more people donating?
