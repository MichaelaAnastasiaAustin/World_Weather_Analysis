
## Background and Overview

PlanMyTrip is a top travel technology company that specializes in internet related services in the hotel and lodging industry. Jack, the head of analysis for the user interface team, asked us to help him collect and analyze weather data for over 500 cities in the world in order to help PlanMyTrip recommend ideal hotels based on clients' weather preferences. After completing that task, Jack along with beta testers suggest the following recommendations: 1) add the weather description to the weather data we already retrieved, 2) create a customer travel destinations map, and 3) create a travel itinerary map. This analysis details the results of these three recommendations. 

## Resources
Data Source: 
Software: Python 3.7, Anaconda, Jupiter Notebook, Google Maps API


## Results: 

### Retrieve Weather Data

With a set of 2,000 random latitudes and longitudes, we retrieved the following information from an API call: Latitude and Longitude, Maximum Temperature, Percent Humidity, Percent Cloudiness, Wind Speed, and Weather Description. The weather data was added to a DataFrame, and then exported into a CSV file (see screenshot below):

![WeatherPy_Database_csv](https://github.com/MichaelaAnastasiaAustin/World_Weather_Analysis/blob/main/Weather_Database_csv_screenshot.png)

### Create a Customer Travel Destinations Map

Customers let us know that the minimum temperature they'd like for their trip is 70 degrees F and the maximum temperature they'd like is 80 degrees F. Using these weather preferences, we identified 177 potential travel destinations and nearby hotels. We then created a marker layer map that indicates the potential travel destinations with pop-up markers. Each pop-up marker includes the following information: Hotel name, City, Country, and Current weather description with maximum temperature. See map below:


![WeatherPy_vacation_map](https://github.com/MichaelaAnastasiaAustin/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

### Create a Travel Itinerary Map


Using the Google Directions API, we created a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations, specifically Sansepolcro, San Giorgio Del Sannio, Melfi, and Sorrento. The map below indicates the the driving route to get to each city in Italy.


![WeatherPy_travel_map](https://github.com/MichaelaAnastasiaAustin/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

We also created marker layer map that pinpoints each city in Italy we are traveling to, along with a pop-up marker. The pop-up marker tells us the Hotel Name, City, Country, and Current weather description with maximum temperature.

![WeatherPy_travel_map_markers.png](https://github.com/MichaelaAnastasiaAustin/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)

## Summary: 

All in all, we successfully completed the three recommendations for PlanMyTrip: 1) add the weather description to the weather data, 2) create a customer travel destinations map, and 3) create a travel itinerary map.
