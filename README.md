# Data-Scraping-Project


**The goal of your project:**
The goal of this project is to identify the top five countries that have attained the greatest number of gold medals in the summer olympics and the winter olympics. 
This would allow the reader to draw parallels between the top five countries and create conclusions based on the results in the bar graph.


**Links to any relevant API documentation:**
The Wikipedia API was used to scrape information from the tables and display it as a bar graph in Jupyter Notebook. 
This was the link that was utilized for instructions: https://pypi.org/project/Wikipedia-API/


**The license of your data and any source data:**
The MIT License is utilized for this project. This is the source website: https://en.wikipedia.org/wiki/All-time_Olympic_Games_medal_table


**A data type and description for each attribute in your data:**
After creating smaller dataframes like summerdata and winterdata from the raw data table, there are two types of data identified: strings and integers.
The columns of countries under the header 'Country' are stored as strings.
The number of gold medals under the headers 'Summer Olympics Gold' and 'Winter Olympics Gold' are stored as integers.


**Any known issues or potential issues, such as sources of bias in collection:**
The first issue identified was that the raw data table consisted of codes for the countries in addition to the name of the country itself. Therefore, a function defined as "name_fixer" was created in order to splice the codes that were present in brackets. 
The second issue was the inclusion of the total row in the tables for summerdata and winterdata. As a result, it was necessary to splice the respective rows as they were interfering with the results displayed in the bar graphs.
A bias that was identified was with respect to the countries achieving gold medals in the winter olympics. I noticed that countries in the northern hemisphere were more likely to win the winter olympics, possibly due to the ideal weather conditions to popularize the sport. This case was observed with countries like Norway, Canada, and Germany. 
















