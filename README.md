## Python API Challenge
Welcome to this Python API Challenge! A class homework for my Washignton University, Data Analytics BootCamp. In this project, I'll be using my knowledge of Python requests, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?"

### Project Overview
### Part 1: WeatherPy
In this deliverable, I'll create a Python script called WeatherPy to visualize the weather of over 500 cities with varying distances from the equator. I'll utilize the citipy Python library, the OpenWeatherMap API, and my problem-solving skills to build a representative model of weather across cities.

### Requirements:

- Retrieve weather data using the OpenWeatherMap API.
- Create scatter plots to showcase the relationships between weather variables and latitude.
- Compute linear regression for each relationship.
- Generate scatter plots with linear regression lines and model details.
  
### Part 2: VacationPy
Moving on to the second part, VacationPy, I'll use the weather data I gathered to plan future vacations. I'll be working with Jupyter notebooks, the geoViews Python library, and the Geoapify API to create map visualizations.

### Tasks:
- Create a map displaying cities with point sizes representing humidity levels.
- Narrow down cities based on specific weather conditions.
- Create a DataFrame to store hotel information.
- Use the Geoapify API to find nearby hotels for selected cities.
- Enhance the map with hotel names and countries in hover messages.

### Getting Started
- To run the WeatherPy project on your local machine, follow these steps:
- Clone the repository: 
git clone [(https://github.com/agorvie/python-api-challenge]
- Install the required dependencies:
pip install matplotlib pandas numpy requests scipy citipy
- Obtain an API key from OpenWeatherMap and add it to the api_keys.py file.

- Run the WeatherPy.ipynb Jupyter Notebook or the equivalent Python script. This script generates scatter plots, performs linear regression analysis, and discusses the results.

- The generated scatter plots and linear regression analysis results will be saved in the output_data directory.

### Findings
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

![image](https://github.com/agorvie/python-api-challenge/assets/122469792/68a32342-049c-4d2d-907b-1ae17a545af3)

![image](https://github.com/agorvie/python-api-challenge/assets/122469792/f92b70e9-f430-44bf-b81a-2cab2ec7fb72)
Discussion about the linear relationship: The r-value of 0.6321280156659894 indicates a moderate positive linear relationship between the two variables. In other words, there is a moderate linear relationship between the latitude and the maximum temperature in the Northern Hemisphere.

This means that as you move closer to the equator (i.e., decrease in latitude), the chosen variable is also likely to increase.

It's important to keep in mind that correlation does not necessarily mean causation, and further analysis would be needed to determine the specific factors driving the observed relationship between latitude and the chosen variable in the Southern Hemisphere.

![image](https://github.com/agorvie/python-api-challenge/assets/122469792/7f3b2c54-257d-4397-b0fc-5d9beb426cdd)
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/09210a7d-b006-4a85-8acd-0928b43f0af9)

Discussion about the linear relationship: Based on the r-value of 0.020687392677830103, there may be a weak positive linear relationship between the two variables being measured. But r-value alone does not provide information about causation or the presence of non-linear relationships between the variables. Other factors can affect the interpretation of the r-value.

![image](https://github.com/agorvie/python-api-challenge/assets/122469792/80f6fddb-5d24-42cd-832d-6f893259d900)
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/871d75e5-432b-4168-8d92-b712b56dfecd)

Discussion about the linear relationship: The r-value of 0.031582010525788115, which is a small positive number between 0 and 1, suggests that there may be a weak positive linear relationship between the two variables being measured. However, the r-value alone does not provide information about causation or the presence of non-linear relationships between the variables. Also, ther factors such as sample size and the distribution of the data can affect the interpretation of the r-value.

![image](https://github.com/agorvie/python-api-challenge/assets/122469792/ffeb88e6-987b-42f1-b35d-01479f749d24)
![image](https://github.com/agorvie/python-api-challenge/assets/122469792/fcca4f6f-4a16-44e4-ae46-603db1c758c3)

Discussion about the linear relationship: The r-value of 0.19672836044457795 indicates that there is a weak positive linear relationship between wind speed and latitude in the southern hemisphere. However, it's important to note that the r-value alone does not provide information about causation or the strength of any non-linear relationships that may exist between the variables. Additionally, other factors such as sample size and the distribution of the data can affect the interpretation of the r-value.

