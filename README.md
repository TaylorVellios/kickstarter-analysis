# Kickstarter - Live Theater Fundraisers

## Overview
A look into the viability of the fundraising platform Kickstarter for live theater projects in the US.

### Purpose
By looking at past Kickstarters, I will be looking for data trends that can assist with determining the ideal conditions for achieving a successful fundraising effort.

## Analysis and Challenges
Kickstarter is a vast platform that allows almost anyone to begin a fundraising effort.
Thankfully, every fundraiser pulled from the platform is tied with heaps of useful data that can be filtered and categorized to hone in our target information.

![1](https://user-images.githubusercontent.com/14188580/110266986-8cd34a00-7f84-11eb-97f6-23ec62d68722.PNG)

Since there are two main goals to achieve, the data needed to be organized and filtered. From what was pulled from the Kickstarter platform, the first step was to separate the subcategories from their parent category. By using delimited Text to Columns, I was able to create split columns that would easily narrow down "Plays" from the "Theater" category.
For an idea of scope in this project: 1,066 Kickstarter fundraisers for "Plays" launched from 2010 to 2017 were pulled from the platform out of a grand total of 4114 data sets.
Within those 1,066 fundraisers that we will be diving into, 671 of them were launched in the United States.
Below are the descriptive statistics for Kickstarter fundraisers for plays within United States compared to global fundraisers for plays.

![2](https://user-images.githubusercontent.com/14188580/110326006-b40a3580-7fdd-11eb-94a7-5477914a5fac.PNG)

We already know that fundraisers in the US make up a majority of fundraisers for plays. Looking at the numbers we can conclude that this subset provides some monetary upwards weight for the overall averages. Moving forward, one of my challenges will be dealing with outliers and visual data.
As we can see above, the mean goals for successful and failed fundraisers in the US respectively are $5,049 and $10,554; while their medians are $3,000 and $5,000.
These numbers tell us that we have slightly left-skewed data, which is not too surprising. The real issue is below:

![3](https://user-images.githubusercontent.com/14188580/110329780-ac995b00-7fe2-11eb-964d-0cdec648badd.PNG)

What we can infer from this is that the range of targets for fundraisers in the US is incredibly vast. In the second graphic I included calculations for outliers according to the 1.5 x IQR rule; but from an analysis standpoint - all data points can be considered valid regardless of how they compare to the average fundraising campaign.

### Analysis of Outcomes Based on Launch Date

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/14188580/110330640-9e980a00-7fe3-11eb-97bd-1ba2444b060f.png)

Using the following pivot table, I have visualized the line chart above that shows the results of Theater related Kickstarter fundraisers by month.

![4](https://user-images.githubusercontent.com/14188580/110345026-becfc500-7ff3-11eb-9be6-22ae656c2168.PNG)

What does this tell us?
1. It is very clear that May is the most popular month for people to launch their fundraising efforts, resulting in the greatest amount of successful Kickstarters over failed ones.
2. Kickstarters launched in December have a near-equal amount of fundraisers that succeeded as those that failed, resulting in the lowest success rate. December is the only month where the failrate moves opposite of the successrate.

Overall the amount of failed Kickstarters doesn't move very much from month to month, but the amount of successful Kickstarters is a wild ride.

Based on these outcomes, I would highly recommend those who aim to start a fundraiser for a live theater event to launch from May through July.
Conversely, it would not be prudent to launch a Kickstarter nearing the end of the year.

### Analysis of Outcomes Based on Goals

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/14188580/110354104-6998b100-7ffd-11eb-8b4a-8fb3f0125422.png)

Along with understanding what works and what doesn't in regards to timing a Kickstarter, it is crucial to look at the success rate for fundraisers in relation to their fundraising goals.
Above is a line chart depicting the percentage of Kickstarters that failed and succeeded in each of their asking price-points at launch.
The X-axis is a series of ranges that represent the goal amounts (in dollars) of Kickstarters.

The key points to look at for someone aiming for a successful Kickstarter are the segments of the chart where the blue line (successes) is above the orange one (fails).
This chart is filtered for only Kickstarters listed under "Theater/Plays", and would not accurately represent fundraising data for other sectors or topics.

![5](https://user-images.githubusercontent.com/14188580/110357364-d2cdf380-8000-11eb-87c4-09128cd03c91.PNG)

Key Takeaways:
 - There is a significant "middle zone" and "top end" of failure that would seem to be asking too much of the play-going market. From $15,000-$30,000 and above $45,000 has a much higher rate of failure than the other price points. To be fair, there are very few data points above the $25,000 mark. Either way, it is safe to say that high budget productions are best fundraised elsewhere.
 - It should come as no surprise that the lower the goal, the higher the likelihood of running a successful Kickstarter campaign. For the data collected, we can see a sweet spot in the $10,000 - $15,000 range that blows much lower-budget fundraisers out of the water with its 83.6% success rate.

### Challenges and Difficulties Encountered

The biggest challenge with this project was organizing the data in a meaningful way. There is so much raw information tied to a single Kickstarter that there was a lot of shoe-tying before any running could take place. Many Excel sheets had to be made in order to keep pivot tables and charts from changing with new filters on the core data, which led to a very bulky Excel workbook. I will likely have to reupload a trimmed down version of my edited workbook in the future for the sake of others.

The biggest limitation with this dataset is how wide the range of usable data is. For the sake of simplicity, we could remove the outliers of successful Kicksters that are way above the mean, but while they are outliers, they are still valid data points. For anyone hoping to launch a successful fundraiser in the Theater/Play market, the important thing to take away is you need to come into this knowing what your price target is beforehand. With the data points given for the "Plays" subcategory, visualization via a box and whisker chart is not viable.

For example, if a potential client wanted to know what price point they should be considering for a fundraising campaign in Great Britain for a live Musical, the data is much more uniformly distributed compared to what we saw above and can be plotted as such:

![Musicals_GreatBritain_Boxplot](https://user-images.githubusercontent.com/14188580/110385869-1cc8d080-8025-11eb-91a5-920e61032bf1.PNG)

Compared to the significantly less useful model based around "Plays in the US":

![6](https://user-images.githubusercontent.com/14188580/110386470-ef305700-8025-11eb-8910-68c0ae6926dc.PNG)


## Results

In conclusion, the data shows that May is the month of the year with the highest success rate of Kickstarters in the live theater category, while December has the lowest.
Know your market. Based on fundraising goals, we have seen that (generally speaking) the more you ask for, the less likely you are to succeed.

There is a lot more that can be done with the data that we pulled, and more information to dig into. I believe there is a lot of interesting correlations that could be found in the "Average Donation" and "Number of Backers" columns that could tell us a lot about certain categories of fundraising campaigns. Overall the biggest hindrance on these metrics for live events is their limited geographic reach. Kickstarters for online marketplace products have the ability to reach a global audience, consequently having the opportunity to hit much higher goals and pledge milestones. A play in a live theater, say in New York, would only have a viable backer market of people in that vicinity to attend the event.

