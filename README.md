# Weather-Forecast
## What is API?
According to MuleSoft API is the acronym for Application Programming Interface, which is a software intermediary that allows two applications to talk to each other. Each time you use an app like Facebook, send an instant message, or check the weather on your phone, you’re using an API. 

## Open Weather API
Open Weather Map API is an API that gives developer information about current weather, daily forecast for 16 days, and 3-hourly forecast 5 days for particular city. It also gives interactive maps that show precipitation, clouds, pressure, wind around particular location. Developers can get the data in JSON, XML, and HTML formats. Visit https://openweather.co.uk/weather-api for more information. 

## Package Structure
I'm using Model View Controller (MVC) design to seperate the datas and the interfaces of this application and connect it with controllers

### weatherForecast
This is the main package that contains other packages

class WeatherForecast

### weatherForecast.MainPage
This package contains classes that represent the main page when user runs the application. It will show the search bar to search a specific city

- class MainPageController
- class SearchBox
- class SearchButton
- class SearchResult

### weatherForecast.CityCurrentCondition
This package contains classes that represent the current condition (temperature, precipitation, wind, humidity) in a particular city

- class CityCurrentConditionPanel
- class CityCurrentConditionController
- class CityNameLabel
- class TemperatureLabel
- class PrecipitationLabel
- class WindLabel
- class HumidityLabel
- class HourlyPredictionButton
- class DailyPredictionButton


### weatherForecast.HourlyPrediction
This package contains classes that represent the weather forecast (temperature, precipitation, wind, humidity) for several next hours in a particular city

- class HourlyPredictionPanel
- class HourlyPredictionController
- class HourlyPredictionTable

### weatherForecast.DailyPrediction
This package contains classes that represent the weather forecast (temperature, precipitation, wind, humidity) for several next days in a particular city

- class DailyPredictionPanel
- class DailyPredictionController
- class DailyPredictionTable

### weatherForecast.Model
This package contains class that has data from OpenWeather API and transfers it between controller and view in other packages

- class WeatherForecastData

## Progress Checklist
- [] MainPage Package
- [] CityCurrentCondition Package
- [] HourlyPrediction Package
- [] DailyPrediction Package
- [] ModelPackage
- [] MainPage Package JUnits
- [] CityCurrentCondition Package JUnits
- [] HourlyPrediction Package JUnits
- [] DailyPrediction Package JUnits
- [] ModelPackage JUnits
- [] JDepend
