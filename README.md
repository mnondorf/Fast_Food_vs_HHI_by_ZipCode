# You Are Where You Eat - The (Potential) Relationship between Fast Food and Income by Zip Code


## Overview

In the US, fast food restaurants (FFRs) are generally thought of as "cheap food" and are often associated with low-income areas in people's minds. We will use machine learning to investigate whether density of FFRs can be used to predict median household income.  


## Hypothesis

We proposed that there is a correlation between density of FFRs (our independent variable) and median income level (our dependent variable) by zip code. 


## Data Sources

1. Census Data on US Household Income Statistics for 2011-2015 sourced from Kaggle.com

2. Restaurant locations scraped from Yelp.

Given the project's time constraints, we chose a subset of eight states (CA, CO, FL, IL, NY, TN, TX, and VA) to run our analysis on in order to keep the scope of the project manageable.


## Machine Learning

We used supervised learning for this project, specifically using linear regression models to identify relationships between the data. 

The hypothesis we tested is whether density of FFRs (x) has an effect on the median income level (y) of the zip code in question. 

We also parsed out the five most common types of restaurants (based on Yelp's categorization) and ran a multiple linear regression analysis on those to see if there were any differences between income levels for certain types of food. 

## Database

We used Postgres and PgAdmin to join and query the data. 


## Limitations

- Discrepancy in time frame of data capture. Household Income is from 2011-2015 but the Yelp results are ostensibly current, as of April 2022.
- Unexplained data loss in the ETL process : 148 data points were dropped when we “globbed” the 8 csv files with Yelp results together in Pandas. It's a tiny fraction of the data but does it affect the results?
- We only used eight states to run our analysis on. Are the states we randomly selected representative of the country as a whole?
- Was our Yelp search radius appropriate for both rural and urban areas? We only searched a 5,000 meter radius for each zip code, which is approximately 3 miles. Is that really large enough to capture food options in rural areas?
- What counts as “fast food” and what doesn’t? We were dependent on Yelp for what constitutes a "fast food" restaurant and it defintely returned some questionable results. 


## Presentation

[Google Slides Version (without the map slide)](https://docs.google.com/presentation/d/1PhhD7InvFKmFyU4L0sTeOg9N1bieIj3SBS_nOlqfc-4/edit#slide=id.p)

[PowerPoint version (with the map slide)](Group_5_Final_Project.pptx)


## Presentation
[Group 5 Presentation Slides](https://docs.google.com/presentation/d/1PhhD7InvFKmFyU4L0sTeOg9N1bieIj3SBS_nOlqfc-4/edit#slide=id.p)



