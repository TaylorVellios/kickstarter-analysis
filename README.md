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

### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
