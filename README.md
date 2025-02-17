# ds_module_11_Scraping_Data_Collection
Homework Module 11 - Scraping HTML, Web Scraping with CSS Selectors
# ds_module_11_Data_Collection
Homework Module 11 - Data Scraping: HTML, Web Scraping CSS Selectors
=========
Objective
----
This project was done with the objetive to practice the web-scraping and data analysis, after learned how to identify HTML elements on a page, identify their id and class attributes and use the knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. With this knowledge the process of scraping was done on include HTML tables and recurring elements, like multiple news articles on a webpage.

To better show off the learned during the Module, the next project was done following the instructions, the new assignment consists of two technical products Deliverable 1 and Deliverable 2.

![alt text](./images/Web-Scraping-Best-Practices.gif)

Deliverable 1:
===
Scrape titles and preview text from Mars news articles.
--
![alt text](./images/Mars_web.PNG)

1. Use automated browsing to visit the Mars news siteLinks to an external site.. Inspect the page to identify which elements to scrape.
2. Create a Beautiful Soup object and use it to extract text elements from the website.
3. Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:
    - Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview.
    - Store all the dictionaries in a Python list.
    - Print the list in your notebook.
4. Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. (Note: there will be no extra points for completing this.)


Deliverable 2: 
===
Scrape and analyze Mars weather data, which exists in a table.
--
![alt text](./images/Mars_table.PNG)

1. Use automated browsing to visit the Mars Temperature Data SiteLinks to an external site.. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.

2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.

3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
    - id: the identification number of a single transmission from the Curiosity rover
    - terrestrial_date: the date on Earth
    - sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
    - ls: the solar longitude
    - month: the Martian month
    - min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
    - pressure: The atmospheric pressure at Curiosity's location

4. Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.

5. Analyze your dataset by using Pandas functions to answer the following questions:
    - How many months exist on Mars?
    - How many Martian (and not Earth) days worth of data exist in the scraped dataset?
    - What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
        - Find the average minimum daily temperature for all of the months.
        - Plot the results as a bar chart.

        ![alt text](./images/plot_bar_Avg_Temperature_by_Month.PNG)

    - Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
        - Find the average daily atmospheric pressure of all the months.
        - Plot the results as a bar chart.
        ![alt text](./images/plot_bar_Avg_Pressure_by_Month.PNG)

    - About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
        - Consider how many days elapse on Earth in the time that Mars circles the Sun once.
        - Visually estimate the result by plotting the daily minimum temperature.

        ![alt text](./images/plot_line_Daily_Minimum_Temperature.PNG)

6. Export the DataFrame to a CSV file.

Note: Citated ChatGTP to help to understand and get the formula how many days elapse on Earth in the time that Mars circles the Sun once.# Unit 11 Homework: Mission to Mars

The homework instructions and requirements are located in Canvas (or in the 08-Canvas folder for those cohorts not on Canvas).