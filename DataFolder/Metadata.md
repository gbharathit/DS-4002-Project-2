# Metadata

## Data Summary

Our dataset consists of the means of the maximum and minimum temperatures of each month in a certain year. Since there is an observation for each unique month and year from 2000-2023, there are a total of 288 rows. For each row, there are five columns, three of which help organize the month and year of the observations. One of the other columns gives the mean of the maximum temperatures in that month, while the last one gives the mean of the minimum temperatures in that month. Our data is in a CSV file, which can be find in our Github repository: DS-4002-Project-2 / DataFolder / AverageTemps.csv https://github.com/gbharathit/DS-4002-Project-2

## Provenance

The dataset originates from the National Oceanic and Atmospheric Administration (NOAA), “Climate” National Weather Service, which includes average temperature for each month from January of 2000 to September 2025. Initially, there was a different dataset for average minimum temperatures and average maximum temperatures. We decided to merge these into one dataset, removing repetitive columns. We also have begun applying time series formatting to our data, so that the data is displayed in a grid format with columns representing months and rows representing years. Because we do not have data for the entire year of 2025, data from this year has been removed. We also had to convert data from the NOAA website into a suitable CSV, since it was not in a downloadable format. We used AI tools in order to copy and paste the original data from the website and create code that would make this data into a table in R that we could then export to a CSV. ****

## License

The original dataset is made publicly available through NOAA. Our cleaned version and analysis outputs will be shared in our GitHub repository under the same open-use conditions, following NOAA’s licensing requirements and citing NOAA and National Weather Service. 

## Ethical Statements

There are no ethical considerations because our dataset deals with climate and temperatures. Because we are not predicting future weather, such as weather in November 2025 and beyond, we don’t have to worry about making any concrete statements that could be affected by external factors. We are simply comparing predictions made by our model with actual data recorded in 2024. 

## Data Dictionary

| Column | Description | Potential Response |
| :------- | :------- | :------- |
| Month_Year | Month abbreviation and year of when temperatures were collected | Jan_2000, Oct_2014, Jun_2023 |
| Year | Year of when temperatures were collected | 2000, 2010, 2023 |
| Month | Month abbreviation of when temperatures were collected | Jan, Jul, Dec|
| Max_Value | Mean maximum temperatures of each month in a certain year, rounded to the nearest tenth | 47.9, 64.8, 80.9|
| Min_Value | Mean minimum temperatures of each month in a certain year, rounded to the nearest tenth | 20.9, 38.4, 76.8|

## Exploratory Plots
![Wordcloud](../OUTPUT/1wordcloud.png)
This word cloud, obtained by finding which words appear the most often in reviews, quickly shows that reviews either focused on loving a product or thinking a product was bad. There are also a lot of words that point out what most of the functionality of the health-related products are.

![Boxplot](../OUTPUT/3boxplot.png)
This box plot shows that a higher compound score generally correlates with a better review score.

![Scatterplot](../OUTPUT/2scatterplot.png)
This scatter plot shows the relationship between review score and review length (number of words), with points colored by sentiment category (positive, neutral, negative). It highlights patterns in how review length varies with sentiment and star rating, providing insight into whether longer reviews tend to express stronger positive or negative opinions. This complements our other exploratory plots by adding a structural perspective on review text, supporting feature selection for predictive modeling.
