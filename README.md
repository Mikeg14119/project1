Executive Summary


Our analysis found varying factors that do affect overall health and fitness in a country’s population. The analysis examined many different relationships between health, environment, and economic indicators. These variables were examined to answer questions regarding the impact that these issues may have on a populations life expectancy and obesity rates. We also looked at how economic factors may impact the prevalence of gyms or health clubs, and how that may impact health and fitness levels.


Introduction
We collected data from multiple sources regarding potential factors that may affect overall health or fitness levels. We are looking at how environmental and financial conditions may impact the health levels of a country’s population and how those conditions may affect the availability and prevalence of gyms and other fitness equipment. We gathered information from the CIA World Factbook, a global analysis of the gym industry, World Happiness Report 2021, and an Air Quality Index with data from over 6,000 cities. 


Data Collection and Preparation


The team looked through Kaggle to identify different datasets that could answer our overarching question: What different factors affect the health and fitness levels of a country’s population? We found the necessary datasets and ensured that they each had a compatible lost of countries so we could begin our analysis.

Some areas where we had to compromise in our data were in how we measured air quality and how we measured economic success. Initially our intent was to find the average wages for each country but were unable to get a sufficient dataset near the year 2021. Instead we were able to find the Real GDP per Capita for each country and used that as an indicator of economic success. For Air Quality Index we were able to find a dataset with data taken from 6,475 cities around the world. We averaged that data out by country and used that as an Average Air Quality Index.  


Data Exploration and Cleaning

When we found the sheets the team individually went over each sheet ensuring that there was a comprehensive list of countries included in the sheet. We then examined the columns to find the pieces of data needed to perform our analysis. Before beginning the data cleaning, we made sure to look over the questions we intended to answer and confirmed that the information we were pulling would provide satisfactory answers.

Each sheet was passed through into a DataFrame and had unnecessary columns removed. Each dataset contained a Country column and we kept only the countries that contained data from all the datasets. The data cleaning included removing any data from years before 2021, as that was our target year. If there were any symbols (Ex: $, %) they were removed and the column types were adjusted to floats for the analysis later. A few columns were also renamed for clarity and conciseness. 


Data Analysis
•	Discuss the methods used to perform the data analysis.
Our main form of analysis was running regressions to get the correlation coefficient, slope, intercept, p-value, r-squared, and std error for different sets of variables to better understand how they interact. Often those findings were paired with a scatter plot with a regression line included but we also included a heat map, a line chart, and a bar chart to assist with visualizing the data. 

•	Discuss the results of the analysis and how they support the conclusion.
For our analysis we singled out a few different variables to attempt to determine if these had an outsized impact on health and fitness levels of a country. We found a small relationship between the Healthy Life Expectancy and AQI per country but our strongest correlation was between Healthy Life Expectancy and World Happiness Score. 

Conclusion


In conclusion we have found that there are a myriad number of variables that affect the health and fitness levels of any given population. While it is not impossible to measure a great many of these variables, for the purposes of our analysis we found that one issue with staying healthy may be the cost of attending a gym itself. Even in the lowest performing economic countries, the base membership price per year was about $300, but would quickly rise with the strength of the countries economy. We feel that this creates an unnecessary barrier to citizens who may not be able to afford that privilege. 

We felt that our largest limitation was the types of data we could gather to measure economic strength and fitness levels. In the future, an analysis like this may require more in depth data gathering to better cover the necessary information. 

References

1.	Singh, A. (2022). World Happiness Report 2021 (Version 2) [CSV file]. Kaggle. https://www.kaggle.com/datasets/ajaypalsinghlo/world-happiness-report-2021
2.	Jas, R. (2022). Most Polluted Cities and Countries (IQAir Index) (Version 2) [CSV file]. IQAir.com. https://www.kaggle.com/datasets/ramjasmaurya/most-polluted-cities-and-countries-iqair-index?select=AIR+QUALITY+INDEX-+top+countries.csv
3.	Central Intelligence Agency. (2022). The World Factbook (Version 3) [CSV file]. Central Intelligence Agency. https://www.kaggle.com/datasets/lucafrance/the-world-factbook-by-cia
4.	Rizzo, N. (2021). 200+ Gym Industry Statistics (Version 1) [Data set]. RunRepeat.com. https://runrepeat.com/gym-industry-statistics#global-gym-industry-statistics
