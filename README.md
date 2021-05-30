# tableau-challenge

In this challenge I studied 4 years of April data of citibike usage in Jersey City.   Selected 1 month per year to limit the volume of data in order to stay within the limits of the free version of tableau.  Please find the below analysis on what the data shows intended for a non-techinical audience.  Below that are a few technical details on what this repository contains.


### Analysis 4 Years of April Citibike Trip Counts
##### Total Trip Counts
In the barchart visualizations, you can see that citibike trips were increasing 2018 to 2019.  2020 Covid pandemic greatly affected citibike usage.  2020 has less than 30% of the trip volume of 2019.  In 2021, April trip count has come back to 2018 levels.
##### Customer vs Subscriber Counts
Viewing the trip counts of Customers vs Subscribers, can see over 90% of the trips were taken by subscribers. <br>
93% of trips in 2018 were by subscribers.<br>
91% of trips in 2019 were by subscribers.<br>
While 2021 April total count of trips has returned to 2018 levels, the subscriber count is way down.<br>
4% of trips in 2021 were by subscribers.<br>
<br>
<br>
##### Maps of Stations
The start and end trip maps dots denote popularity by size, larger being more popular and the year by color- Blue 2018, Orange 2019, Red 2020, Aqua 2021. The map is overlayed with Street, zip code and point of interest information.<br>
The top 10 stations in 2018 and 2019 before covid overlap with 9 out of 10 of the top 10 stations during the low usage year of 2020.  Exchange Place which is number 3 in 2018 and 2019 does not exist in 2020 and 2021.  It appears this station was replaced by nearby Columbus Dr at Exchange, which was #8 most popular in 2021. <br> Overall, this dataset shows most of the popular start and end stations are by train or light rail stops: Grove Street, Newport Pkwy, Newport, Sip.  Hamilton Park is another popular station - it is a large park with restuarants near by.

<br>
<br>
<br>
<br>







### Repository Contents
This repo contains a jupyter notebook used to combine 4 months of data into a single dataset.  4 csvs of data were loaded into dataframes, the unneeded columns were dropped, a year column was added and then the 4 were combined into a single dataframe which was dropped into a new csv to load into Tableau.
The jupyter notebook also has a google API to search out hospitals around the Jersey City zipcode.   This was intended to be used in Tableau mapping because the app's "point of interest" map layer did not contain all hospitals, however Tableau does not allow use of a un-joined dataset in the same workbook.
The repository also contains the Tableau-citibike-challenge.twbx workbook file.



