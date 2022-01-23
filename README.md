# Module_6_Challenge
The purpose of this challenge was to work with the OpenWeatherMap and GoogleMaps API to create travel itenerary maps given an input of temperature from the client. 

## Weather_Database
This script creates a randomly generated list of latitudes and longitudes and assigns a city name using the citipy module. Then I perform an api call to OpenWeatherMap to get weather data (maximum temperature, % humidity, % cloudiness, windspeed, and weather description) for the input city and save this dataframe as a csv file. 

## Vacation_Search
This script imports the previously saved city/weather dataframe and filters for cities that fall with in the input max and min temperature. Then it performs and api call to the GooglePlaces API via nearbysearch to find hotels with in 5000m of the city lat/long and saves the data in csv format. Then it uses the gmaps module to plot pins and info boxes for each hotel. 

## Vacation Itinerary
This script imports the hotel data and plots it using gmaps again. Then I choose 4 cities to create roundtrip driving directions map via the gmaps.directions_layer function. 
