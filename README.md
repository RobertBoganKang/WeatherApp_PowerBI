# WeatherApp with Microsoft Power BI & R
## Notice
This project is not fancy, it is only used for demo. 

You can use this repository for any purposes except my API key for `OpenWeatherMap.org`, thank you!
## Introduction
### Method
This project use R to fetch data from [OpenWeatherMap](http://openweathermap.org/) API, and convert from JSON to the data that Power BI could read.
### Something else
Basically, it is a visualization of data but could update very easily. Some plot generated by R is used for learning and testing purposes.
## Usage
### In order to run this program, please follow this step
* Make sure R is installed in local machine, and make sure 2 libraries are installed in local machine `jsonlite` and `ggplot2`.
* Open program "weather app.pbix", the default setting is the location at Milwaukee, US. The weather now page shows all parameters of current weather (time is UTC; users must set the time zone from the script).
* Refresh data by clicking `Home>Refresh`.

### If you wish to change the cities of weather, please follow this step
* Click `Home>Edit Queries`.
* Select one of the data set, then double-click `Query Settings>APPLIED STEPS>Souce` on the right panel; then find the line and change `city <- ""Milwaukee,US""` and `timezone <- -6`, the field of "Milwaukee,US" and "-6" to any city and time-zone as you like; however please follow the format of `<city name>,<country code>`, time-zone is the time shift over UTC. If you don't know your country code, you can type your city to [city](http://openweathermap.org/city) to check.
* Do this for another data set.
* Apply changes, close, and save the project.

## Explanation (for non-IT person)
* BI: Business Intelligence.
* JSON: JavaScript Object Notation (it is a format to store data).
* UTC: Coordinated Universal Time (Greenwitch Time).
* R: A programming language for statistics.
* jsonlite: An R library used for converting JSON format into a format (i.e. data frame) R could understand.
* ggplot2: An R library for visualization the data, this only used for R graphics test in this project (not necessary).
* Visualization: Convert data into the graphics that people could understand more easily.

***Enjoy***
