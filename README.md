# Kaggle_Barcelona_Project

## Data Preparation
### In this section, the needed data preparation steps required for the analysis is performed. Unnecessary chunk
### codes are omitted in the compiled pdf-file. First of all, the actual allocation of the immigrants in the city
### is revealed, for which the “immigrants_by_nationality.csv” file was used. Due to the lack of data and the
### impossibility to differentiating them, all types of migrations were considered, including the internal one, even
### when this group represents 36.32% of all migrations data in 2017 (35,354/97,327).
### The data preparation steps for the different variables are as follow:
### For understanding the connectivity of each neighborhood, the “bus_stop.csv” file was used. After tidying
### up missing or mistaken values, and deleting duplicate ones, the final count of metro stations and bus stops
### per neighborhood was calculated. For counting the number of bus stop per area, just the “Day bus stop”
### and “Night bus stop” variables were considered and sum up in the “dayandnigth_count” column, leaving
### appart the “Airport bus stop” and “Bus station” ones because they are just a few observations and do not
### really impact in the daily connectivity of the hood.
### The “accidents_2017.csv” file contains the number of accidents, exact location and severity details for 10,339
### observations during the year 2017. Since areas with higher population would have higher accidents, the number of accidentes was normalized using the total population of that neighborhood and accidents per 1,000 persons. The “life_expectancy.csv” file contains life expectancy data for different neighborhoods of Barcelona. For this purpose, the mean life expectancy per neighborhood was taken. To do so, the average of life expectancy over the years 2006-2014 was calculated. Finally, the average of male and female population for each neighborhood was estimated. To achieve the above the melting and casting operations on the original data table were used. Last but not least, the “unemployment.csv” and “population.csv’ ’ contains the number of unemployed individuals and population at districts and neighborhood level for the years 2013 - 2017. The immigrant_emigrants_age consists of immigrants data for the years 2015-2017. The registered unemployed data at neighborhood level is extracted and merged with neighborhood’s population data for the 2015-2017 time period. The resultant table is then merged with immigrants data at neighborhood level, also the unemployment is then normalized by population and consequently used for analysis and visualization.
