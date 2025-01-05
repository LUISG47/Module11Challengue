# MODULE 11 CHALLENGUE


## Part 1: Scrape Titles and Preview Text from Mars News

Open the Jupyter Notebook called part_1_mars_news.ipynb. 

1. Use automated browsing to visit the Mars website: https://static.bc-edx.com/data/web/mars_news/index.html Inspect the page to identify which elements to scrape.
2. Create a Beautiful Soup object and use it to extract text elements from the website.
3. Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:
+ Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. An example is the following:
![Screenshot 2025-01-05 at 5 27 13 p m](https://github.com/user-attachments/assets/fdec3dc7-61ac-458f-84c8-fffa49130e61)


+ Store all the dictionaries in a Python list.
+ Print the list in your notebook.

+ The result should be as follows:

![Screenshot 2025-01-05 at 5 28 33 p m](https://github.com/user-attachments/assets/000b0611-ad82-40d1-b7b6-0a746b5ebbdf)


4. Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. 
The file will be created in the resources folder and it will be called mars_news.json

![Screenshot 2025-01-05 at 5 53 07 p m](https://github.com/user-attachments/assets/edcc7867-d4c4-451e-8947-951434f80395)


## Part 2: Scrape and Analyze Mars Weather Data

Open the Jupyter Notebook in the starter code folder named part_2_mars_weather.ipynb

1. Use automated browsing to visit the Mars Temperature Data Site: https://static.bc-edx.com/data/web/mars_facts/temperature.html Inspect the page to identify which elements to scrape
2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.
3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
+ id: the identification number of a single transmission from the Curiosity rover
+ terrestrial_date: the date on Earth
+ sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
+ ls: the solar longitude
+ month: the Martian month
+ min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
+ pressure: The atmospheric pressure at Curiosity's location
4. Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.
5. Analyze your dataset by using Pandas functions to answer the following questions:
+ How many months exist on Mars?
+ How many Martian (and not Earth) days worth of data exist in the scraped dataset?
+ What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
  + Find the average minimum daily temperature for all of the months.
  + Plot the results as a bar chart.
The resulting graph should be as follows:

![Screenshot 2025-01-05 at 3 59 42 p m](https://github.com/user-attachments/assets/a08ffa53-4763-48a8-bc48-fb31bfe4679b)


And the same graph sorted from highest to lowest should be as follows:

![Screenshot 2025-01-05 at 3 59 35 p m](https://github.com/user-attachments/assets/978a4f37-3942-4dd5-8003-7d28ebf8b04a)


+ Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
  + Find the average daily atmospheric pressure of all the months.
  + Plot the results as a bar chart.
 
The resulting graph should be as follows:

![Screenshot 2024-12-28 at 10 21 13 p m](https://github.com/user-attachments/assets/da425f5c-0b82-402c-b81a-e848a5438fb3)

And the same graph sorted from lowest to highest should be as follows:

![Screenshot 2024-12-28 at 10 21 19 p m](https://github.com/user-attachments/assets/e0acbe22-aa37-4fd1-943d-dc79e6a3d900)


+ About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
  + Consider how many days elapse on Earth in the time that Mars circles the Sun once.
  + Visually estimate the result by plotting the daily minimum temperature of each observation.

The resulting graph should be as follows:

![Screenshot 2024-12-28 at 10 21 27 p m](https://github.com/user-attachments/assets/05deb8f8-5712-4181-8030-76053061fd50)


From the graphs obtained we can make this conclussions:

#### Minimum Temperature

As we can see in the ordered graph, the coldest months on Mars are months 3, 4 and 2 and the "warmest" months are months 8, 9 and 10. This must be taken into account since today they are forecast more explorations on Mars.
Average minimum temperatures on Mars display significant variation throughout the year, reflecting the planet's unique seasonal cycles. The coldest temperatures are typically recorded during the winter months in the Southern Hemisphere, where conditions can become extremely harsh. In contrast, summer months in the same hemisphere experience comparatively warmer temperatures. These temperatures can pose considerable challenges for the design and engineering of rovers and other technological systems that will be deployed in the Martian environment.

#### Atmospheric Pressure

The graph we obtained illustrates the variations in atmospheric pressure on Mars throughout the months. From this graph, we can observe that the lowest atmospheric pressures occur during the months of 5 to 7. Conversely, the highest pressures are typically recorded during months 10, 9, and 2. This significant fluctuation in pressure indicates that there are considerable changes in atmospheric conditions from month to month. As a result, it becomes challenging to make accurate predictions about the stability of atmospheric pressure, since it can vary greatly in a short time frame.

#### Year Length

The analysis of the temperature patterns reveals a sinusoidal function, which indicates that the Martian year spans approximately 687 Earth days. This extended duration means that each season on Mars lasts nearly twice as long as the corresponding seasons on Earth. Such an elongated seasonal cycle can lead to prolonged atmospheric phenomena and more extended weather patterns.
Understanding these temperature dynamics is crucial because they have significant implications for the Martian environment. The length of the Martian seasons influences not only the climate but also the behavior of various atmospheric processes
This understanding provides essential insights into the environmental conditions on Mars, which are vital for scientific research.

6. Export the DataFrame to a CSV file.

The resulting file will be stored in the Resources folder and it will be named mars_weather_data.csv

  
  



























