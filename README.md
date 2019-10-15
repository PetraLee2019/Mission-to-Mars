Web scrapes data from Mars News related websites, loads the data into mongo db and displays the information in a single HTML page.

![alt tag](https://github.com/PetraLee2019/Plotly/blob/master/newfolder/Images/microbes-sem.jpg?raw=true)
![alt tag](https://github.com/PetraLee2019/Plotly/blob/master/newfolder/Images/microbes-sem.jpg?raw=true)


Technology Stack - HTML, CSS, BootStrap, Jupyter, Python

Python Libraries - Pandas, Beautiful Soup, Splinter, PyMongo

Database - Mongo DB

App Server - Flask

Steps :
To scrape various websites for data related to the Mission to Mars and display output on Jupyter Notebook [Scraping_mission_to_mars.ipynb].

To create a Python Script [scrape_mars.py] to scrape and execute all scraping code and return one Python dictionary containing all of the scraped data.

To create a Flask App [app.py] to create route (index and scrape). The root route / will query Mongo database and pass the mars data into an HTML template to display the data.

To create HTML file [index.html] that will take the mars data dictionary and display all of the data in the appropriate HTML elements.

To create Mongo db and collection to store the scraped data. PyMongo was used to set up mongo connection and to define db and collection.
