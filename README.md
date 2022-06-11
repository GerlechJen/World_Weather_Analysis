# World Weather Analysis
## Overview
In this project, a random set of latitudes and longitudes were generated using the Numpy and random module. Using the citiPy Module, more than 600 cities near the random latitudes and longitudes were obtained. The OpenWeather map API was used to request for the current weather data of each unique city in JSON format.The following data was then retrieved from the JSON file: 
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
Input statements from customers were used to filter the data for their weather preferences. With that information, potential travel destinations and nearby hotels were identified. From the list of potential travel destinations, four cities in Canada were chosen to create a travel itinerary. Finally, using the Google Maps Directions API, a travel route was created between the four cities, as well as, a marker layer map.



## Vacation Search
Based on traveler’s weather preferences, travelers can identify potential travel destinations and nearby hotels. The map showcases destinations using pop-up markers on a marker layer-map.

### Sample Travel Destinations

![WeatherPy_vacation_map](https://github.com/cmmgw/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

## Vacation Itinerary 
Using the Google Directions API, a sample itinerary was created that shows the route between four cities in Kazakhstan.

![WeatherPy_travel_map](https://github.com/cmmgw/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.PNG)

## Statistical Analysis
Global city data was plotted, and linear regression was used to find the relationship between the following variables: 

* Latitude and Maximum Temperature
* Latitude and Humidity
* Latitude and Cloudiness
* Latitude and Wind Speed



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
