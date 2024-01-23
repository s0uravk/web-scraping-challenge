# web-scraping-challenge
![web-scraping](https://github.com/s0uravk/web-scraping-challenge/assets/144293972/137479d7-48d6-4d2f-97b3-10d210c93c96)

This challenge emphasizes web scraping to retrieve data for analysis and making informed decisions based on that. Web scraping is done using the splinter library of Python to perform browser actions and the BeautifulSoup library to read through the HTML elements of the webpage. And then storing the retrieved data in a Pandas dataframe for visualization of the data, which is then stored as a csv file.

For part_1_mars_news.ipynb, The script first import the required dependencies. Then an instance of Browser object is created and visit method  is used to with a URL to to open browser for scraping the data. Then Beautifulsoup instance is created to parse the retrieved HTML. Next, required HTML data is filtered by the class_  and is stored into a variable. That stored data is looped through using For loop to get data present within the elements by the class_. And output is being stored into a dictionary and appends to a list which return a list of dictionaries with title and preview. Then browser is closed.

For part_2_mars_weather.ipynb, the script follows the same procedure until saving the required data as a variable, but while looping through that data, a nested for loop is also used. As the data to be extracted is in a table element of HTML, that returns a list for each record, which is then added to a list and finally returns a list of lists.

Going further, that list is converted into the Pandas Dataframe using suitable column names, and datatypes are converted appropriately for the ease of data analysis. Analysis: answer the following question using the Pandas aggregate function, etc., and the data is plotted using Matplotlib and Pandas for visual understanding:

1. How many months exist on Mars?
2. How many Martian (and not Earth) days worth of data exist in the scraped dataset?
3. What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
    Find the average the minimum daily temperature for all of the months.
    Plot the results as a bar chart.
4. Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
    Find the average the daily atmospheric pressure of all the months.
    Plot the results as a bar chart.
5.About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
    Consider how many days elapse on Earth in the time that Mars circles the Sun once.
    Visually estimate the result by plotting the daily minimum temperature.

Finally, the retreived data is stored as a CSV file in the  Output folder and the browser is exited.
