# Surfs up Weather analysis
Weather analysis using SQLite and SQLAlchemy. Climate App building using Flask. Other tools include Python and Jupyter Notebooks.

## Purpose

1.  Explain the structures, interactions, and types of data of a provided dataset.
2.  Differentiate between SQLite and PostgreSQL databases.
3.  Use SQLAlchemy to connect to and query a SQLite database.
4.  Use statistics like minimum, maximum, and average to analyze data.
5.  Design a Flask application using data.

## Overview

An investor wants to learn more about the weather before committing to build a Surf and Ice Cream shop in Oahu, Hawaii. The investor's main concern is the precipitation forcing the shop to close too frequently. To analyze Hawaii's weather data, SQLAlchemy was used to query the SQLite database.

## Results

Performed exploratory climate analysis for Oahu to assess weather patterns and their potential affects on a surf and ice cream shop business.

Weather patterns were determined by writing queries that referenced the hawaii.sqlite database containing yearly weather information gathered from multiple weather stations. In addition, a Flask weather app (app.py) was set up to share the results via a webpage.

## Challenge Assessment

One of the main concerns for establishing a surf and ice cream shop is whether or not certain times of the year will be better or slower for business. For example, summer months may have better weather than the winter months. Therefore, the key statistical data for the months of June and December have been analyzed and the results are displayed below:

June Statistics:
![Jun](https://github.com/awalindeep/surfs_up/blob/AwalinGHMAIN/Resources/Jun.png)

December Statistics:
![Dec](https://github.com/awalindeep/surfs_up/blob/AwalinGHMAIN/Resources/DEC.png)

The key statistics analysis calculates the mean, standard deviation, minimum and maximum values, percentiles, and count; precipitation (prcp) is in total inches and temperature (tob) is the temperature observed in degrees fahrenheit. From a quick glance at the data, it is observed that on average, there is less rain and higher temperatures during the month of June. However, with the data displayed, there is not much disparity between the two months. The temperature is in the 70's during the June and December months with max temperatures in the 80's, and average amount of precipitation jumps from about 0.14 inches to 0.22 inches respectively.

## Summary:

The investor's main concern was getting rained out too frequently. Comparing the June and December weather patterns, the temperatures and precipitation means are reasonably close. The temperature data is not strongly skewed for either month. The ratio of the temperatures to the precipitation for the two months is also reasonably similar with few outliers over 3 inches of precipitation. The data supports opening a Surf and Ice Cream shop year-round.

## Recommendations for Further Analysis

I would recommend calculating the number of days that it rained each month in addition to the amount rained. Although some months may have had more rain, the data could have been skewed by a couple of days of heavy rain. If it is raining more days out of certain months, people may be less inclined to surf during those months. To help support the additional analysis, I would also recommend constructing histograms for the targeted months, such as June and December, to visualize the number of observations for certain levels of rainfall.

For next steps, I would also begin to consider where on Oahu the shop would be best located. The weather data was gathered from different stations across the island. Some parts of the island may have better weather than the other locations. A key statistical weather analysis can be made for each of the 9 stations, and then compared. As well as, the number of observations made by each station can be reviewed. Before relying solely on the statistical data, it is important to make sure that sufficient and accurate data is being used; maybe one of weather stations is new or data was not being gathered due to issues experienced by the station. These are all possibilities that need to be considered before proceeding with building the surf and ice cream shop.
