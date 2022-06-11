# World Weather Analysis
## Overview
In this project, a random set of 2,000 latitudes and longitudes were generated using the Numpy and random module. Using the citiPy Module, more than 600 cities near the random latitudes and longitudes were generated.
The OpenWeatherMap API was used to request for the current weather data in JSON format of each unique city in the cities list. The following data was retrieved from the JSON file: 
* City
* Country
* Date
* Latitude and longitude
* Maximum temperature
* Humidity
* Cloudiness
* Wind speed


This weather data was added to a pandas dataframe and matplotlib was used to create a series of scatter plots showing the relationship between latitudes and the various weather parameters of all the cities. 
Statistical calculations was also performed on the weather data to determine correlations. Using linear regressions on the weather parameters in the northern and southern hemispheres. We were able to predict that there is relation between 


A series of heatmaps were also created using Google Maps and Places API that showcased Latitude and temperature, Latitude and humidity, Latitude and cloudiness, and Latitude and wind speed.The heatmap was improved by including pop-up markers to display information on specific cities based on a customer's temperature preferences.
Using the city's coordinates and Google Maps and Places API, information on hotels in the cities could also be derived.

This data will help people predict the best time of the year to plan a vacation. 

The weather data will then be used to choose the best cities for vacation based on client's weather preferences.

The cities were then mapped using Jupyter gmaps and google places API


and an API call was made on current weather data for the nearest corresponding cities.
From the API callwe retrieved:
Latitudes
Longitudes
Maximum temperature
Percent humidity
Percent cloudiness
Wind speed
Current Weather description
The data was plotted using google maps 
using Jupyter Notebook, Pandas Library, CityPy, JSON Traversals, APIs and Python Requests, 


weather data was used to collect data from over 600 cities around the world. collected from a webiste using API 

to help customers find their ideal hotel anywhere in the world 
