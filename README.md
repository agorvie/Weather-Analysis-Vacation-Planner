# Weather Analysis & Vacation Planner

Welcome to the Weather Analysis & Vacation Planner project! This project is part of the Data Analytics BootCamp at Washington University and involves using Python, APIs, and data visualization to explore weather patterns and plan future vacations.

## Table of Contents
- [Project Overview](#project-overview)
- [Part 1: WeatherPy](#part-1-weatherpy)
- [Part 2: VacationPy](#part-2-vacationpy)
- [Getting Started](#getting-started)
- [Findings](#findings)

## Project Overview

In this project, we will create two main parts: WeatherPy and VacationPy.

### Part 1: WeatherPy

In WeatherPy, I will retrieve weather data for over 500 cities from the OpenWeatherMap API. I will then visualize the relationships between weather variables and latitude using scatter plots and perform linear regression analysis to understand these relationships. The key requirements include:

- Retrieving weather data using the OpenWeatherMap API.
- Creating scatter plots to showcase the relationships between weather variables and latitude.
- Computing linear regression for each relationship.
- Generating scatter plots with linear regression lines and model details.

### Part 2: VacationPy

In VacationPy, I will use the weather data obtained in WeatherPy to plan future vacations. I will create map visualizations that display cities based on humidity levels and narrow down cities based on specific weather conditions. Additionally, I will use the Geoapify API to find nearby hotels for selected cities and enhance the map with hotel names and countries in hover messages. The key tasks include:

- Creating a map displaying cities with point sizes representing humidity levels.
- Narrowing down cities based on specific weather conditions.
- Creating a DataFrame to store hotel information.
- Using the Geoapify API to find nearby hotels for selected cities.
- Enhancing the map with hotel names and countries in hover messages.

## Getting Started

To run this project on your local machine, follow these steps:

1. Clone the repository: `git clone https://github.com/agorvie/python-api-challenge.git`
2. Install the required dependencies: `pip install matplotlib pandas numpy requests scipy citipy`
3. Obtain an API key from OpenWeatherMap and add it to the `api_keys.py` file.
4. Run the `WeatherPy.ipynb` Jupyter Notebook or the equivalent Python script. This script generates scatter plots, performs linear regression analysis, and discusses the results.
5. The generated scatter plots and linear regression analysis results will be saved in the `output_data` directory.

## Findings

The findings and insights from the WeatherPy and VacationPy analyses will be discussed in the respective Jupyter Notebooks and Python scripts within this repository.

### Scatter Plots and Linear Regression
The project generates scatter plots for the following weather variables:

Latitude vs. Temperature
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/1150ccd1-385e-48ca-820a-73560c13a9c7)

Latitude vs. Humidity
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/05bf160a-b267-485c-b56b-ccf903a67c26)

Latitude vs. Cloudiness
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/cd32cb66-8cf6-40c0-9783-deca74309c90)

Latitude vs. Wind Speed
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/d1caf1b6-c605-4e7f-a17c-1416c9108b40)

For each scatter plot, a linear regression analysis is performed for both the Northern and Southern Hemispheres. The linear regression line is plotted on the scatter plot along with the regression equation. The r-value (coefficient of determination) is provided to indicate the strength of the linear relationship between latitude and the weather variable.

#### Temperature vs. Latitude Linear Regression Plot

The Northern r-value is: 0.7432718426426184
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/68a32342-049c-4d2d-907b-1ae17a545af3)

The Southern r-value is: 0.6321280156659894
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/f92b70e9-f430-44bf-b81a-2cab2ec7fb72)

Discussion about the linear relationship: The r-value of 0.6321280156659894 indicates a moderate positive linear relationship between the two variables. In other words, there is a moderate linear relationship between the latitude and the maximum temperature in the Northern Hemisphere.

This means that as you move closer to the equator (i.e., decrease in latitude), the chosen variable is also likely to increase.

It's important to keep in mind that correlation does not necessarily mean causation, and further analysis would be needed to determine the specific factors driving the observed relationship between latitude and the chosen variable in the Southern Hemisphere.

Humidity vs. Latitude Linear Regression Plot

The Northern r-value is: 0.035471978532659945
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/7f3b2c54-257d-4397-b0fc-5d9beb426cdd)

The Southern r-value is: 0.020687392677830103
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/09210a7d-b006-4a85-8acd-0928b43f0af9)

Discussion about the linear relationship: Based on the r-value of 0.020687392677830103, there may be a weak positive linear relationship between the two variables being measured. But r-value alone does not provide information about causation or the presence of non-linear relationships between the variables. Other factors can affect the interpretation of the r-value.

Cloudiness vs. Latitude Linear Regression Plot

The Northern r-value is: 0.002207739330413193
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/80f6fddb-5d24-42cd-832d-6f893259d900)

The Southern r-value is: 0.031582010525788115
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/871d75e5-432b-4168-8d92-b712b56dfecd)

Discussion about the linear relationship: The r-value of 0.031582010525788115, which is a small positive number between 0 and 1, suggests that there may be a weak positive linear relationship between the two variables being measured. However, the r-value alone does not provide information about causation or the presence of non-linear relationships between the variables. Also, ther factors such as sample size and the distribution of the data can affect the interpretation of the r-value.

Wind Speed vs. Latitude Linear Regression Plot

The Northern r-value is: 0.0007034828087211801
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/ffeb88e6-987b-42f1-b35d-01479f749d24)

The Southern r-value is: 0.19672836044457795
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/fcca4f6f-4a16-44e4-ae46-603db1c758c3)

Discussion about the linear relationship: The r-value of 0.19672836044457795 indicates that there is a weak positive linear relationship between wind speed and latitude in the southern hemisphere. However, it's important to note that the r-value alone does not provide information about causation or the strength of any non-linear relationships that may exist between the variables. Additionally, other factors such as sample size and the distribution of the data can affect the interpretation of the r-value.

