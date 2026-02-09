# ⛅ OpenWeatherMap API project 

## 📝 Description: 

### A API (Application Programming Interface) project written in Postman using Java Script that fetches weather data from OpenWeatherMap API.
- [OpenWeatherAPI](https://openweathermap.org/api) was the api used to fetch weather data.
- [LatLong.net](https://www.latlong.net/) was used to find the latitude and longitude of a city.
- [Postman](https://www.postman.com/) was the main API platform to test and document the API in one collaborative workspace.

## 🤔 How to create this project?

### 
1. Create an Account on OpenWeatherMap.
2. Once succesfully registered, click on profile, then APIKEY tab to see your APIKEY (Your api key will take a couple hours to activate)
4. Copy the API call:

```
api.openweathermap.org/data/2.5/forecast?lat={lat}&lon={lon}&appid={API key}
```
5. Go to Postman, create an account if not already.
6. Paste the copied API call into Postman.
7. It will prompt you to enter longitude, latitude and your API_KEY.<br>
*For longitiude and latitude use [LatLong.net](https://www.latlong.net/)!* <br>

10. (*Optional*) Make sure to add a key named "units" with the value "imperial", this will allow the degrees to be displayed in farenheit.
11. Click send and you should see data, under "response" below. <br>
Here is a sample, of what your workspace should look like before inputed values: <br>

![postman_layout_visual](https://github.com/talia-gordy/weather_API/blob/main/apipslayout.png)

## 👀 My example 

### For my example, I did the cordinates for Los Angeles, the data I retrieved is a snippet of the data I got from today 2/9/2026 (5 day / 3 hour forecast):

```
{
    "cod": "200",
    "message": 0,
    "cnt": 40,
    "list": [
        {
            "dt": 1770670800,
            "main": {
                "temp": 75.09,
                "feels_like": 73.67,
                "temp_min": 75.09,
                "temp_max": 75.22,
                "pressure": 1016,
                "sea_level": 1016,
                "grnd_level": 995,
                "humidity": 29,
                "temp_kf": -0.07
            },
            "weather": [
                {
                    "id": 802,
                    "main": "Clouds",
                    "description": "scattered clouds",
                    "icon": "03d"
                }
            ],
            "clouds": {
                "all": 32
            },
            "wind": {
                "speed": 5.14,
                "deg": 148,
                "gust": 4.68
            },
            "visibility": 10000,
            "pop": 0,
            "sys": {
                "pod": "d"
            },
            "dt_txt": "2026-02-09 21:00:00"
        }
```
## ❔Common Issues and Must Knows 
 ### 1. In order for a successful send, you must remember to wait a couple hours for your APIKEY to activate, otherwise you will receive an error message.
 
 ### 2. The API used in this project was the 5 day / 3 hour forecast, which is the one avaible to use with the free tier.
