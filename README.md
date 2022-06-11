# World Weather Analysis
## Overview
In this project, a random set of latitudes and longitudes were generated using the Numpy and random module. Using the citiPy Module, more than 600 cities near the random latitudes and longitudes were obtained. The OpenWeatherMap API was used to request for the current weather data of each unique city in JSON format.The following data was then retrieved from the JSON file: 
* City
* Country
* Date
* Latitude and longitude
* Maximum temperature
* Humidity
* Cloudiness
* Wind speed

This weather data was added to a pandas DataFrame and a series of scatter plots showing the relationship between latitudes and the weather parameters (maximum temperature, percent humidity, percent cloudiness, wind speed) for all cities was plotted using matplotlib. Statistical calculations were also performed on the parameters to determine their correlations with latitude. Using linear regressions on the weather parameters in both the northern and southern hemispheres separately, we were able to predict that there is a strong correlation between latitude and temperature. However, for humidity, cloudiness, and wind speed, there is low correlation between them and latitude. This makes them unpredictable due to changing weather patterns that can increase or decrease their value.

A feature was added whereby a customer enters their preferred temperature and cities are filtered based on the customer's preference. Making use of the coordinates of those filtered cities, hotels were found using Google Places API.

A series of heatmaps were also created using Google Maps and Places API for all the four weather parameters (maximum temperature, percent humidity, percent cloudiness, wind speed) . The heatmaps were improved by creating a marker for  each city that displays the name of the city, country code, maximum temperature, and name of a nearby hotel within three miles of the coordinates when the marker is clicked. 

## Weather Data
Continuing further with the project, a set of 2,000 random latitudes and longitudes were generated, the nearest cities retrieved, and an API call performed with the OpenWeatherMap. In addition to the city weather data already gathered, the current weather description for each city was also retreved and included in the data. A new DataFrame containing the updated weather data was then created for further analysis.

## Customer Travel Destination Map
Input statements from customers were used to filter the data for their weather preferences. With that information, potential travel destinations and nearby hotels were identified and shown on a marker layer map with pop-up markers.


## Travel Itinerary Map 
From the list of potential travel destinations, a sample itinerary was created that shows the route between four cities in Canada. 
![image2](https://github.com/GerlechJen/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

Finally, using the Google Maps Directions API, a marker layer map with a pop-up marker for each city on the itinerary was created.
![image3](https://github.com/GerlechJen/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)
