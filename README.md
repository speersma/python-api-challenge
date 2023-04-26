# python-api-challenge

This repository contains files for the API challenge of the MSU Data Analytics boot camp. 

The files contained in this repo can be conceptually partitioned into analysis notebooks and output data. 

- **Analysis notebooks**: There are two notebooks in the WeatherPy directory: WeatherPy.ipynb and VacationPy.ipynb. 
    - In the WeatherPy notebook, a random list of cities distributed around the globe is generated using the `citypy` library. This list of cities is then used in conjunction with the OpenWeatherMap API to retreive weather data for each city in the list. This data is then converted to a dataframe and relationships amongst several variables are examined using scatterplots and OLS regression. These scatter plots are saved in the output_data directory. 
    
    - In the VacationPy notebook, the city weather dataframe generated in the WeatherPy notebook is used to create some data maps. The first data map shows a point on the world map for every city, the size of the point on the map is the humidity of each city. The city weather dataframe was subsequently reduced to cities that met vacation criteria (detailed in the vacationpy notebook). The geoapify API was then used to identify hotels near (within 10,000 meters) each city. The names of these hotels were then incorporated into the city weather dataframe and a new data map was generated which included points for cities meeting the vacation criteria. This new map also included the hotel names in the hover data displayed when a cursor is placed over a point. 


- **output data**: The `output_data` folder contains figures from the WeatherPy notebook. This includes several scatterplots and the cities.csv file generated in WeatherPy and used in VacationPy. 