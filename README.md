# Kickstarting with Excel

## Overview of Project

After Louise's play "Fever" almost reached its' goal in her attempt to fundraise for her kickstarter project, she wanted to know how different campaigns fared based on their goals and launch dates. This project analyzes the kickstarter dataset to figure out what the outcomes of different campaigns were, based on their launch dates and their funding goals.

### Purpose

The project contains two technical items, both of which are charts, to help Louise visualize the outcomes of different kickstarter campaigns based on when they were launched and what their funding goals were.

## Analysis and Challenges

The analysis of this project was performed on the [Kickstarter_Challenge](https://github.com/Zarif601/kickstarter-analysis/blob/main/Kickstarter_Challenge.xlsx) dataset, which is downloadable thorugh the provided link. The analysis was split into two parts. The first part covers the analysis of campaign outcomes based on the launch dates, and the second part covers the analysis on outcomes based on the goals of the fundraising campaigns.

### Analysis of Outcomes Based on Launch Date

To start of the analysis, a "Year" column was created using the YEAR() function to hold the year values from the "Date Created Conversion" column, which held all the launch dates of the campaigns. After that a pivot table was created on a new sheet called "Theatre Outcomes by Launch Date." The pivot table displays the outcomes: "successful," "failed," and "canceled" per month filtered on the theatre category every year there was a campaign in this category. The line chart [Theatre_Outcomes_vs_Launch](https://github.com/Zarif601/kickstarter-analysis/blob/main/Resources/Theatre_Outcomes_vs_Launch.png) was then created to visualize the outcomes of the campaigns and their launch months.

### Analysis of Outcomes Based on Goals

In a new sheet called "Outcomes based on Goals" several columns were created to hold different ranges of goals, numbers of successful, failed and canceled projects, their percentages and the total number of projects to perform mathematical analysis on the data. The functions that were used to populate these columns were COUNTIFS() and SUM(), other than performing simple mathematical calculations for the percentages. Afterwards, the line chart [Outcomes_vs_Goals](https://github.com/Zarif601/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png) was created to visualize the relationship between the outcomes and the goal ranges.

### Challenges and Difficulties Encountered

During the analysis of this project I learned the COUNTIFS() formula which I wasn't familiar with. Although it wasn't difficult, it was something new that I figured out and it seems like a very useful function for many types of analyses. I hand-coded the ranges of goals in the COUNTIFS() formula, which may have become difficult if I had many more ranges. As such, figuring out a better way to do it would be a worthwile challenge. Playing around with the charts to make them look the best was also a fun and challenging experience.

## Results

- Two conclusions about the Outcomes based on Launch Date:
1. From the chart we can see that a lot of campaigns had success during the summer months. Especially in May. 
2. We can also see a drop in success of campaigns during the start of the year and towards the end of the year as well.

- Conclusion about Outcomes based on Goals:
From the chart we can see that campaigns with lower goals had higher success rate. The succes rate gradually dropped with larger and larger goals. However, we do see a spike in the success rate of campaigns starting around the 30000-34999 range and staying rising till around the 40000-44999 range, after which the success rate drops significantly.

- Some limitations of this dataset:
This dataset doesn't have any qualitative data which could possibly indicate why people decided not to back certain capmaigns. If there were something like top comments made about said project, it might help with making more informed predictions using the data. It would also help understand why certain campaigns were pladged far more money than their original goals.

- Other possible tables and/or graphs that could be helpful:
1. One interesting analysis could be performed regarding the outcomes of the campaigns based on the duration of the campaigns. The "Date Created Conversion" and the "Date Neded Conversion" data could be used to make such analysis using graphs along with the "outcomes" data.
2. We could also analyze the outcomes of campaigns with the "spotlight" column data to see how being in the spotlight affected the outcome of different kickstarter campaigns.
