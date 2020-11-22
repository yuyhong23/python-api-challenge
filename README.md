# Python API - What's the Weather Like?

Data and instructions provided by UC Berkeley Extension Data Analytics Bootcamp.

# Introduction 

The goal of this assignment is to use my newfound Python requests, APIs, and Json traversals knowledge and skills to retrieve data from an endpoint. 

There two parts to this assignments: WeatherPy and VacationPy.

# Technologies/Libraries

  - Python Pandas
  
  - Jupyter Notebook
  
  - Matplotlib
  
  - requests
  
  - json
  
  - scipy.stats (linregress)
  
  - citipy
  
  - gmaps
  
  - Conda Environment used: PythonData
  
  APIs used:
  
  - OpenWeatherMap
  
  - Google Map: Place, Maps JavaScript

# Detailed Instructions/Assignment Background

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"
  
Now, we know what you may be thinking: "Duh. It gets hotter..."

But, if pressed, how would you prove it?

###### Part I - WeatherPy:

In this example, you'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.

Your final notebook must:

  - Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
  
  - Perform a weather check on each of the cities using a series of successive API calls.
  
  - Include a print log of each city as it's being processed with the city number and city name.
  
  - Save a CSV of all retrieved data and a PNG image for each scatter plot.
  
  - Must include a written description of three observable trends based on the data.

###### Part II - VacationPy :

Now let's use your skills in working with weather data to plan future vacations. Use jupyter-gmaps and the Google Places API for this part of the assignment.

  - Create a heat map that displays the humidity for every city from the part I of the homework.

  - Narrow down the DataFrame to find your ideal weather condition. 
  
  - Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.
  
  - Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.
  
  - Must include a screenshot of the heatmap you create and include it in your submission.

# Files

  - The Maps folder contains the google map screenshots.
  
  - The output_data folder contains the city csv and scatter plots.
  
  - The vacationpy folder contains the vacationpy jupyter notebook where my scripts are.
  
   - The weatherpy folder contains the weatherpy jupyter notebook where my scripts are.

# Process and Credits

My first assignment using Python requests, APIs, and Json traversals, as well as dealing with gitignore to hide the config.py (where the API keys are stored). I used class materials and outside resources for references, attended office hour, asked Bootcamp's Learning Assistant App for help, and also seeked help from my classmate to complete this assignment.

1. When I first started to work on weatherpy, I was kind of overwhelmed and confused at the beginning. So I attended office hour and instructor pointed out that we need to extract some info from the OpenWeatherMap. He showed me that I can create a key to hold a list of value, and then make a dictionary to hold the extracted values. Then append the dictionary to the list. He also showed me how to convert unix timestamp to readable dates, but that wasn't necessary, since that will give me error when trying to calculate statistical info for all the columns.

2. When I was working on vacationpy, I wasn't able to retrieve the name of the hotel for each city, what I ended up getting was the city name. I asked the Learning Assistant, she said my code looked fine. Then I asked my classmate, and she told me it was because for type I entered "hotels" instead of "lodging." It was tricky.

Here are the outside resources I used for this assignment (as well as attempts):

  - https://stackoverflow.com/questions/3682748/converting-unix-timestamp-string-to-readable-date
  - http://jonathansoma.com/lede/data-studio/matplotlib/labeling-your-axes-in-pandas-and-matplotlib/
  - https://www.pacioos.hawaii.edu/voyager-news/lat-long-formats/
  - https://matplotlib.org/3.1.1/gallery/text_labels_and_annotations/annotation_demo.html
  - https://gist.github.com/subfuzion/db7f57fff2fb6998a16c
  - https://stackoverflow.com/questions/25436312/gitignore-not-working
  - https://www.mapsmarker.com/kb/faq/for-development-purposes-only-error-on-google-basemaps/
  - https://jupyter-gmaps.readthedocs.io/en/latest/tutorial.html
  - https://buildmedia.readthedocs.org/media/pdf/jupyter-gmaps/stable/jupyter-gmaps.pdf
  - https://developers.google.com/places/web-service/overview
