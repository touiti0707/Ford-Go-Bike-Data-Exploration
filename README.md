## Date created
Project uploaded on 28/09/2019

# Ford Go Bike Data Exploration
## by Touiti MARIE-BORNAND

## Dataset
Ford Go Bike was a bicycle sharing system in the San Francisco Bay Area, California (USA). The data consists of information regarding trip data for 2017 including trip duration, start/end time and date, and other trip characteristics. The dataset is a csv file called `2017-fordgobike-tripdata.csv` and can be found [here](https://www.lyft.com/bikes/bay-wheels/system-data).

## Exploratory Analysis
At the beginning of the exploration we have examined all variables individually, splitting them into two groups: trip characteristics and user details.

Insights extracted about trip characteristics:
* who are the ten most used stations (among a total of 272)
* each of these stations attracted between 1.5% and 3.5% of the overall traffic
* peak activity at 8-9am and 5-6pm with more than 50,000 bike trips each hour
* lots of short trips and a few long trips; a peak around 600 seconds (10 minutes)
* most of the trips last between 180 and 1800 seconds (3 and 30 minutes, respectively)

Insights extracted about user details:
* 79% of the users are subscribers and the rest are customers (21%)
* 77% of the users are male, 22% are female and 1% identify themselves as other
* the typical user of the bike sharing service has between 30 and 40 years old

Then we combined variables in pair in order to identify relationships. We observed a negative relationship between age and duration: younger users make the longest trips and as the age of the customers increases, the trips get shorter in duration. One interesting connection I discovered was the very different trip duration according to user type. The customer category has a median trip duration of roughly 1000 seconds and an interquartile range of 1000 seconds. The subscriber category have much shorter trips and the overall distribution is concentrated within a smaller range: median of approximately 500 seconds and interquartile range of 500 seconds.

Finally, we made multivariate visualizations to validate the relationships found before. It turns out the pattern of trip duration according to the age does not differ depending on the type/gender of the user. Whether they are a subscriber/custoner or male/female, younger users make the longest trips and as the age of the customers increases, the trips get shorter in duration.
    
## Explanatory Analysis
    
For the presentation, I have tried to answer my three initial questions. 

*What is the most popular bike trip?*
I have presented four univariate visualizations in order to illustrate the most populart start/end station (categorical variables), start time (categorical) and duration (numeric). Bar charts for the categorical variables and a histogram for the numeric variable were employed.

*Does the people that use this bike sharing service share similar characteristics?*
I have presented three univariate visualizations in order to identify the typical user of the bike sharing service in terms of user type (categorical - customer or subscriber), gender (categorical - male or female) and age (numeric). Pie charts for the categorical variables and a histogram for the numeric variable were employed.

*Are there relationships between user details and trip characteristics?*
I have presented one bivariate visualizations (boxplots) to display the relationship between user type (categorical) and duration (numeric).
    
*Are there relationships between user details and trip characteristics?*
I have presented two multivariate visualizations (scatterplots) to display the relationship between age (numeric) and duration (numeric), adding also user type and member (categorical variables) in the mix by faceting.

For each graph, I made sure to include explicit graph titles and axis titles.

# Software requirements

You should have Python3, pandas, matplotlib and Jupyter Notebooks.

# Credits

Thanks to the Udacity team for this great project which is part of the Data Analyst Nanodegree Program!