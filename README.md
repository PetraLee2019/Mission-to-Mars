# Mission to Mars 

## Mars Data Scraping
A web scraping application which retrieves and presents summary information, the latest news, and images of Mars. A project designed to loads the data into MongoDB and displays the information in a single HTML page. 

### Prerequisites
- The Python libraries flask, flask_pymongo, BeautifulSoup, and splinter must be installed in order for the code to run. The initial data scraping can be run either in a Jupyter Notebook or in Python.

### Technology Stack 
- HTML, CSS, BootStrap, Jupyter, Python
- Python Libraries - Pandas, Beautiful Soup, Splinter, PyMongo
- Database - Mongo DB
- App Server - Flask

![alt tag](https://github.com/PetraLee2019/Mission_to_Mars/blob/master/Images/Final_Screenshot_1.png?raw=true)

### Process:
Scrape data from several websites containing Mars news. Different types of data included were images of Mars, tweets about the current Mars weather, a table of Mars facts, and headlines with the latest Mars news. After scraping, the data is stored in MongoDB and then loaded it into an HTML file using a Flask template that interfaces with Python and formatted with HTML using Bootstrap.

### Steps:
- To scrape various websites for data related to the Mission to Mars and display output on Jupyter Notebook [Scraping_mission_to_mars.ipynb].
- To create a Python Script [scrape_mars.py] to scrape and execute all scraping code and return one Python dictionary containing all of the scraped data.
- To create a Flask App [app.py] to create route (index and scrape). The root route / will query Mongo database and pass the mars data into an HTML template to display the data.
- To create HTML file [index.html] that will take the mars data dictionary and display all of the data in the appropriate HTML elements.
- To create Mongo db and collection to store the scraped data. PyMongo was used to set up mongo connection and to define db and collection.

![alt tag](https://github.com/PetraLee2019/Mission_to_Mars/blob/master/Images/Final_Screenshot_3.png)

### Sources:
[Nasa Mars News](https://mars.nasa.gov/news/)
- Scrape the latest NASA Mars news using BeautifulSoup, splinter, pandas in a jupyter notebook.
[JPL Space Images](https://www.jpl.nasa.gov/spaceimages/?search=&category=Mars)
- Using Splinter to navigate the site and scrape the JPL featured image of mars in full resolution.
[Mars Weather Twitter](https://twitter.com/marswxreport?lang=en)
- Visit the Mars Weather Twitter account and scrape the latest Mars weather data.
[Space Facts](https://space-facts.com/mars/) 
- Mars facts table from Space-Facts.
[USGS](]https://astrogeology.usgs.gov/search/results?q=hemisphere+enhanced&k1=target&v1=Mars)
- From United States Geological Survey Astrogeology to obtain high resulution images for each of Mar's Hemisphere. 

### Run without Heroku:
- Copy/gather the files in this repo (don't need the .gitignore).
- Start a MongoDB daemon in the terminal, then start mongo instance.
- Run the app.py in the terminal. Copy the local url to your web browser.



------------------
note for petra 
Overall Structure
There are four distinct files for this project: the Jupyter Notebook file (mission_to_mars.ipynb), the converted Python scraper script (scrape_mars.py), the Flask app used to access this converted Python scraper script and to store the scraped data into a MongoDB database (app.py), and the HTML file to display and arrange the data (index.html).
