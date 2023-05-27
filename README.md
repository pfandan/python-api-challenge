
Unit 6 Homework: 
What's the Weather Like?

Before You Begin
Create a new repository for this project called python-api-challenge. Do not add this homework to an existing repository.

Clone the new repository to your computer.

Inside your local Git repository, create a directory for both of the Python challenges. Use a folder name that corresponds to the challenges, such as WeatherPy.

Inside the folder you just created, add new files called WeatherPy.ipynb and VacationPy.ipynb. These will be the main scripts to run for each analysis.

Push the above changes to GitHub.

Part 1: WeatherPy
In this section, you'll create a Python script to visualize the weather of 500+ cities of varying distance from the equator. To do so, you'll use a simple Python library, the OpenWeatherMap API, and your problem-solving skills to create a representative model of weather across cities.

The first requirement is to create a series of scatter plots to showcase the following relationships:

Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude
After each plot, add a sentence or two explaining what the code is analyzing.

The second requirement is to compute the linear regression for each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude
After each pair of plots, explain what the linear regression is modeling. For example, describe any relationships that you notice and any other findings you may have.

Your final notebook must:

Randomly select at least 500 unique (non-repeated) cities based on latitude and longitude.
Perform a weather check on each of the cities using a series of successive API calls.
Include a print log of each city as it's being processed, with the city number and city name.
Save a CSV of all retrieved data and a PNG image for each scatter plot.
Part 2: VacationPy
Now, let's use your skills working with weather data to plan future vacations. Use Jupyter-gmaps and the Google Places API for this part of the assignment.

To complete this part of the assignment, you will need to do the following:

Create a heat map that displays the humidity for every city from Part 1

Narrow down the DataFrame to find your ideal weather condition. For example:

A max temperature lower than 80 degrees but higher than 70.

Wind speed less than 10 mph.

Zero cloudiness.

Drop any rows that don't satisfy all three conditions. You want to be sure the weather is ideal.

Note: Feel free to adjust your specifications, but make sure to limit the number of rows returned by your API requests to a reasonable number.

Use Google Places API to find the first hotel for each city located within 5,000 meters of your coordinates.

Plot the hotels on top of the humidity heatmap, with each pin containing the Hotel Name, City, and Country

As final considerations:

You must complete your analysis using a Jupyter notebook.
You must use the Matplotlib or Pandas plotting libraries.
For Part 1, you must include a written description of three observable trends based on the data.
For Part 2, you must take a screenshot of the heatmap that you create and include it in your submission.
Your plots must include labeling aspects like plot title (with date of analysis) and axis labels.
For max intensity in the heatmap, try setting it to the highest humidity found in the dataset.
Hints and Considerations
The city data that you generate is based on random coordinates and different query times, so your outputs will not be an exact match to the provided starter notebook.

You will need to apply your critical thinking skills to understand how and why we're recommending the tools we are. What is citipy used for? Why would you use it in conjunction with the OpenWeatherMap API? How would you do so?

While building your script, pay attention to the cities you are using in your query pool. Are you covering the full range of latitudes and longitudes? Or are you choosing 500 cities from one region of the world? Even if you were a geography genius, simply listing 500 cities based on your personal selection would create a biased dataset. Try to think of ways that you can counter this.

Hint: Consider the full range of latitudes.
Once you have computed the linear regression for one relationship, you will follow a similar process for all other charts. As a bonus, try to create a function that will create these charts based on different parameters.

Remember that each coordinate will trigger a separate call to the Google API. If you're creating your own criteria to plan your vacation, try to reduce the results in your DataFrame to 10 or fewer cities.

Ensure your repository has regular commits and a thorough README.md file.
