# python-api-challenge
# module 6 Challenge

Background
Data's true power is its ability to definitively answer questions. So, let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?"
Now, we know what you may be thinking: “That’s obvious. It gets hotter.” But, if pressed for more information, how would you prove that?

# Instructions
This activity is broken down into two deliverables, WeatherPy and VacationPy.

# Part 1: WeatherPy
In this deliverable, you'll create a Python script to visualise the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and your problem-solving skills to create a representative model of weather across cities.
For this part, you'll use the WeatherPy.ipynb Jupyter notebook provided in the starter code ZIP file. The starter code will guide you through the process of using your Python coding skills to develop a solution to address the required functionalities.
To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

# Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
To fulfill the first requirement, you'll use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, you'll create a series of scatter plots to showcase the following relationships:
Latitude vs. Temperature

![Fig1](https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/79356a35-c5b2-42a4-8dce-c0f2b0b4754f)

Latitude vs. Humidity

![Fig2](https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/048b4ae1-be04-4fec-a7af-557ba520e8ae)

Latitude vs. Cloudiness

![Fig3](https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/3d68b570-2100-461e-9462-56c026bcb184)

Latitude vs. Wind Speed

![Fig4](https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/137ccf01-7c47-4eb0-a3ba-60879cb258ce)


# Requirement 2: Compute Linear Regression for Each Relationship
To fulfill the second requirement, compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.
Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r^2 values as you can see in the following image

# Create the following plots:

Northern Hemisphere: Temperature (C) vs. Latitude
![Fig5](https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/cdbdd773-d063-46a5-84bc-729a9ba5189e)

Southern Hemisphere: Temperature (C) vs. Latitude
![Fig6](https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/6e9e76e8-37b0-4cde-bff2-c9fe48499c6c)

Northern Hemisphere: Humidity (%) vs. Latitude
![Fig7](https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/d84d212e-3afd-45a9-b045-3c8720317e88)

Southern Hemisphere: Humidity (%) vs. Latitude
![Fig8](https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/34dce709-f42e-4096-aa4b-3eb25907f216)

Northern Hemisphere: Cloudiness (%) vs. Latitude
![Fig9](https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/7efcce9d-fe5e-4e67-b485-5d16595a74ca)

Southern Hemisphere: Cloudiness (%) vs. Latitude
![Fig10](https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/34d55aeb-258b-43bc-a821-a0a76956dee0)

Northern Hemisphere: Wind Speed (m/s) vs. Latitude
![Fig11](https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/826935fa-36b2-4dc0-9ab9-865d9f4ac424)

Southern Hemisphere: Wind Speed (m/s) vs. Latitude
![Fig12](https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/4ee013b8-5190-42c4-bf5f-3c1adcc5665e)

After each pair of plots, explain what the linear regression is modelling. Describe any relationships that you notice and any other findings you may uncover.

## Part 2: VacationPy
In this deliverable, you'll use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.
The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.
Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualisations.
To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:
Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

# PICTER

2. Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:

A max temperature lower than 27 degrees but higher than 21
Wind speed less than 4.5 m/s
Zero cloudiness
NOTE
Feel free to adjust your specifications, but make sure to set a reasonable limit to the number of rows returned by your API requests.

3. Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.
For each city, use the Geoapify API to find the first hotel located within 10,000 metres of your coordinates.
Add the hotel name and the country as additional information in the hover message for each city in the map:

<img width="569" alt="map" src="https://github.com/EvgeniiaKei/python-api-challenge/assets/166274251/331adb3b-1df5-4d55-a082-34b43e8018ae">



