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
In the main data frame called "userdata", the list of countries are presented as strings and the number of medals are presented as integers.
Smaller data frames called "summerdata" and "winterdata" are created from "userdata". The smaller data frames have the same types of data. The columns of countries under the header 'Country' are stored as strings. The number of gold medals under the headers 'Summer Olympics Gold' and 'Winter Olympics Gold' are stored as integers.


**Any known issues or potential issues, such as sources of bias in collection:**
The first issue identified was that the raw data table consisted of codes for the countries in addition to the name of the country itself. This prevented the bar graph from looking concise and visually appealing. To resolve this problem, a function defined as "name_fixer" was created. Since the code of the country was placed in a parentheses and was located after the name of the country, the replace function was utlized to search it and delete the remainder of the string. This allowed the program to splice the country's code and only return the name of the country. 

The second issue was the inclusion of the total row in the tables for summerdata and winterdata. The total row interfered with the bar graph because its number appeared to be significantly large than the number of medals attained by the rest of the countries. Since the total medals row was located in the last row for the summer olympics and winter olympics, I was able to solve this problem by removing the last row. I ensured that I completed this before displaying my bar graph.  

A bias that I identified during my data collection process was that I assumed that all countries had an equal opportunity to win a gold medal in the olympics. However, after displaying the graph for the winter olympics, I realized that it only comprised of countries located in the northern hemisphere. This may be due to ideal weather conditions to popularize the winter sports. This case was observed with countries like Norway, Canada, and Germany. 

A potential limitation was that I was dependent on Wikipedia for obtaining data regarding the number of olympic medals acquired from countries around the world. To increase reliability, it would be better to refer to the Olympics source itself. This can potentially help make the results displayed more accurate. 
