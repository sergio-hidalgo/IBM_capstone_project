# IBM_capstone_project
Captstone project for the IBM Data Science Professional certificate, based on <a href='https://developer.foursquare.com/'>Foursquare API</a> data

Discover the diverse areas of Madrid and Barcelona, based on the common and differential venues included on each, by using the Foursquare API info.
The main purpose is to recommend the best city of the two to possible migrants with a 'persona' profile linked to 'natural way of living'.
Once the best candidate city is chosen, we will follow a funneling process to narrow down to the best possible and more 'natural' options of neighborhoods a possible migrant could move to based on their salary range.

During this journey we will go thorugh the following steps:
* Extract Madrid and Barcelona districts and neighborhoods from Wikipedia page
  - Parse the Wikipedia tables with BeautifulSoup
  - Convert html object into a dataframe
  - Data cleaning
* Get latitude and longitude values per neighborhood 
  - Extract info from a combination of Wikipedia and Geohack tables
  - Use info collected to add as dictionaries
  - Convert dictionaries into dataframes
  - Merge dataframes
* Analyze and cluster the neighborhoods of the winning city based on total venues
  - Run a k-mean clustering process with ScyKit-learn
  - Plot the clustered neighborhoods with Folium
  - Analyze the clusters
  - Chose the cluster with a more homogeneous and 'more natural' profile of neighborhoods included
  - Short-list neighborhoods to a list of top 10 'more natural' options
* Include additional info of interest from sources like INE, Idealista or Glassdoor via csv files
  - Include buildings characteristics by neighborhoods (including average size in m2) from INE
  - Include average renting prices (by m2) by neighborhoods from Idealista
  - Include a series of average job anual salaries in destination city
* Generate the final recommendations
  - convert all above csv files into dataframes and merge accordingly
  - calculate average accomodation renting price per neighborhood
  - compare possible alternative neighborhood options with 3 average salary range scenarios.

This project includes the full notebook with all code both in ipynb and html formats, a project final report in pdf format, and a project presentation, also in pdf format.

Created by Sergio Hidalgo in March 2021
