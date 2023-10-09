# Data-Scraping-Project


The goal of your project:
The goal of this project is to identify the top five countries that have attained the greatest number of gold medals in the summer olympics and the winter olympics. 
This would allow the reader to draw parallels between the top five countries and create conclusions based on the results in the bar graph.


Links to any relevant API documentation:
The Wikipedia API was used to scrape information from the tables and display it as a bar graph in Jupyter Notebook. 
This was the link that was utilized for instructions: https://pypi.org/project/Wikipedia-API/


The license of your data and any source data:




A data type and description for each attribute in your data:
After creating smaller dataframes like summerdata and winterdata from the raw data table, there are two types of data identified: strings and integers.
The columns of countries under the header 'Country' are stored as strings.
The number of gold medals under the headers 'Summer Olympics Gold' and 'Winter Olympics Gold' are stored as integers.


Any known issues or potential issues, such as sources of bias in collection:
The first issue identified was that the raw data table consisted of codes for the countries in addition to the name of the country itself. Therefore, a function defined as "name_fixer" was created in order to splice the codes that were present in brackets. 
The second issue was the inclusion of the total row in the tables for summerdata and winterdata. As a result, it was necessary to splice the respective rows as they were interfering with the results displayed in the bar graphs.
A bias that was identified was with respect to the countries achieving gold medals in the winter olympics. I noticed that countries in the northern hemisphere were more likely to win the winter olympics, possibly due to the ideal weather conditions to popularize the sport. This case was observed with countries like Norway, Canada, and Germany. 
















**Step 1: Data extraction**
The API that was utilized for the following project was the wikipedia api. 
This was conducted by entering the code "import wikipediaapi"

Imported Requests, Pandas, and BeautifulSoup

Status of the wikipedia URL is checked to ensure that it is legal to scrape using the code "print(response.status_code)"

The table of contents is printed in HTML format using the code "olympictable=soup.find('table',{'class':"wikitable"})"

Created a dataframe using the code "userdata = pd.DataFrame(userdata[0])"

A columns list is created by the titles of all of the columns in the raw data table

A "name_fixer" function is defined to remove the the codes for the country, making the table visually appealing. Function is called.




**Step 2: Data transformation and load**
summerdata dataframe is created to record the Gold Medals won by countries in the Summer Olympics
Values in the column are converted from strings to integers

winterdata dataframe is created to record the Gold Medals won by countries in the Winter Olympics
Values in the column are converted from strings to integers



**Step 3: Analysis: Summary and visualizations**
The last row from summerdata and winterdata are removed since they consist of the total number of medals
Using the 'n.largest' function, the countries with the top 5 number of gold medals are printed
Using the '.plot' function, the countries are printed using a bar graph
The title, x axis label, and y axis label are added as paramater to print on the graph




**Step 4: Documentation**
An aspect of the data  that surprised me was the high number of gold medals attained by the United States in the summer olympics. 

















Step 3: Analysis: Summary and visualizations
