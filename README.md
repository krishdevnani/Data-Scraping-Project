# Data-Scraping-Project


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


















Step 3: Analysis: Summary and visualizations
