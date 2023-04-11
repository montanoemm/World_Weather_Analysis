# World_Weather_Analysis
Weather analysis.

The first code is a project to analyze the relationship between several latitudes and the different weather parameters it affects. Linear regression patterns were created as well as scatter plots to represent the findings. A sample of 642 cities was extracted from the OpenWeather API, the format of the information was JSON following the next link from the documentation to formulate the specific requests(https://openweathermap.org/current#current_JSON)
API endpoint URL code was obtained through Chat GPT:
“import requests
import urllib.request

# Define the base URL for the OpenWeatherMap API
url = 'https://api.openweathermap.org/data/2.5/weather?appid=YOUR_API_KEY'

# Define a list of cities to get weather data for
cities = ['San Francisco', 'New York', 'Los Angeles', 'Chicago']

# Iterate over the list of cities and create an endpoint URL for each city
for city in cities:
    city_url = url + "&q=" + urllib.request.pathname2url(city)
    response = requests.get(city_url)
    print(response.content)”

Output files are stored in a folder named output_data. File names are (cities.csv, Fig1, 2, 3, and 4)
The Vacation file includes a list of 158 cities with hotel names filtered by max temperature from 21 Celsius to less than 27 Celsius.
The parameter for the API call were obtained through the following link:
(https://apidocs.geoapify.com/docs/places/#api)
