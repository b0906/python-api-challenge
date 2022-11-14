# python-api-challenge: What's the Weather Like as we approach the equator?"



## Part 1: WeatherPy
In this section, I create a Python script to visualize the weather of 500+ cities of varying distance from the equator. I use a simple Python library, the OpenWeatherMap API, and create a representative model of weather across cities.
I create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

After each plot, I add the explaination what the code is analyzed.
I compute the linear regression for each relationship. This time, I separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots, I explain what the linear regression is modeling. 
My final notebook includes:

* Randomly select at least 500 unique (non-repeated) cities based on latitude and longitude.
* Perform a weather check on each of the cities using a series of successive API calls.
* Include a print log of each city as it's being processed, with the city number and city name.
* CSV of all retrieved data and a PNG image for each scatter plot.


## Part 2: VacationPy
I use Jupyter-gmaps and the Google Places API for this part.
I follow steps below:


* Create a heat map that displays the humidity for every city from Part 1, as in the following image:


Narrow down the DataFrame to find an ideal weather condition as below:


* A max temperature lower than 80 degrees but higher than 70.
* Wind speed less than 10 mph.
* Zero cloudiness.
* Drop any rows that don't satisfy all three conditions. You want to be sure the weather is ideal.



I use Google Places API to find the first hotel for each city located within 5,000 meters of my coordinates.
I Plot the hotels on top of the humidity heatmap, with each pin containing the Hotel Name, City, and Country, as in the following image:
