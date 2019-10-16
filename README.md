Mars Data Scraping
A web scraping application which retrieves and presents summary information, the latest news, and images of Mars. A project designed to loads the data into MongoDB and displays the information in a single HTML page. 

![alt tag](https://github.com/PetraLee2019/Mission_to_Mars/blob/master/Images/Final_Screenshot_1.png?raw=true)

Prerequisites
The Python libraries flask, flask_pymongo, BeautifulSoup, and splinter must be installed in order for the code to run. The initial data scraping can be run either in a Jupyter Notebook or in Python.

Technology Stack - HTML, CSS, BootStrap, Jupyter, Python
Python Libraries - Pandas, Beautiful Soup, Splinter, PyMongo
Database - Mongo DB
App Server - Flask

![alt tag](https://github.com/PetraLee2019/Mission_to_Mars/blob/master/Images/Final_Screenshot_3.png)

Process:
Scrape data from several websites containing Mars news. Different types of data included were images of Mars, tweets about the current Mars weather, a table of Mars facts, and headlines with the latest Mars news. After scraping, the data is stored in MongoDB and then loaded it into an HTML file using a Flask template that interfaces with Python and formatted with HTML using Bootstrap.
 

Steps:
To scrape various websites for data related to the Mission to Mars and display output on Jupyter Notebook [Scraping_mission_to_mars.ipynb].

To create a Python Script [scrape_mars.py] to scrape and execute all scraping code and return one Python dictionary containing all of the scraped data.

To create a Flask App [app.py] to create route (index and scrape). The root route / will query Mongo database and pass the mars data into an HTML template to display the data.

To create HTML file [index.html] that will take the mars data dictionary and display all of the data in the appropriate HTML elements.

To create Mongo db and collection to store the scraped data. PyMongo was used to set up mongo connection and to define db and collection.


Scraping:
NASA Mars News
Scrape the NASA Mars News Site and collect the latest News Title and Paragraph Text

JPL Mars Space Images - Featured Image
Visit the URL for the JPL Featured Space Image
Use Splinter to navigate the site and find the image URL for the current Featured Mars Image and assign the URL string to a variable called featured_image_url
Make sure to find the image URL to the full size .jpg image
Make sure to save a complete URL string for this image

Mars Weather
Visit the Mars Weather Twitter account and scrape the latest Mars Weather Tweet from the page
Save the Tweet text for the weather report as a variable called mars_weather

Mars Facts
Visit the Mars Facts webpage and use Pandas to scrape the table containing facts about the planet including Diameter, Mass, etc.
Use Pandas to convert the data to a HTML table string

Mars Hemispheres
Visit the USGS Astrogeology site to obtain high resolution images for each of Mar's hemispheres
Save both the image URL string for the full resolution hemisphere image, and the Hemisphere title containing the hemisphere name.
   Use a Python dictionary to store the data using the keys img_url and title
   
Append the dictionary with the image URL string and the hemisphere title to a list
This list will contain one dictionary for each hemisphere




------------------
note for petra 
Overall Structure
There are four distinct files for this project: the Jupyter Notebook file (mission_to_mars.ipynb), the converted Python scraper script (scrape_mars.py), the Flask app used to access this converted Python scraper script and to store the scraped data into a MongoDB database (app.py), and the HTML file to display and arrange the data (index.html).
