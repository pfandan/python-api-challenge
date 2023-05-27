Weather Analysis
The WeatherPy directory contains 2 Jupyter Source Files WeatherPy.ipynb and VacationPy.ipynb which request relevant data from 2 API providers OpenWeatherMap and Geoapify for over 500 cities within the desired coordinates, and a repo output_data which contains the output images generated from WeatherPy.ipynb.

The two Jupyter Source Files utilize Pandas library to create DataFrame for each dataset. Matplotlib library was imported to create series of scatter plots based on different variables. Scipy and linregress were also imported to help with statistical computation and generate linear regresssion line for the data points. Citipy was imported to generate list of cities with the coordinates, hvplot was imported for interactive data visualization, and geoviews is imported to explore and visualize data geographically.

The visulations are stored under output_data folder 
