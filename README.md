# The-Battle-of-Neighbourhoods
# Introduction 

The purpose of this Project is to help people in exploring better facilities in & around their neighborhoods. It will help them in making smart and efficient decisions when selecting their preferred neighborhood out of all the neighborhoods in Scarborough, Toranto. Many people are migrating to Scarborough, Toronto and require a lot og research to find housing prices in their range and good schools for their children. This project will help such people. This Project aims to create an analysis of features for people migrating to Scarborough to search best neighborhoods by comparing neighborhoods with each other. The features include median housing prices and schools according to ratings, crime rates of that particular area, road connectivity, weather conditions, management for emergency, water resources both fresh and waste water and excrement conveyed in sewers and recreational facilities. It will help people to get awareness of the area and neighborhood before moving to a new city, state, country or place for their work or to start a new fresh life.
# DataSet Used

Data Link: https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M

I have used Scarborough dataset which we scrapped from wikipedia in Week 3. Dataset consists of latitude and longitude, zip codes.
# Foursquare API

I have used Four-square API in this Capstone project for data gathering, as it has a database of millions of places, especially their places API which provides the ability to perform location search, location sharing and details about a business.
We will need data about different venues in different neighborhoods of that specific borough. In order to gain that information we will use "Foursquare" locational information. Foursquare is a location data provider with information about all manner of venues and events within an area of interest. Such information includes venue names, locations, menus and even photos. As such, the foursquare location platform will be used as the sole data source since all the stated required information can be obtained through the API.

After finding the list of neighborhoods, we then connect to the Foursquare API to gather information about venues inside each and every neighborhood. For each neighborhood, we have chosen the radius to be 100 meter.

The data retrieved from Foursquare contained information of venues within a specified distance of the longitude and latitude of the postcodes. The information obtained per venue as follows:

Neighborhood
Neighborhood Latitude
Neighborhood Longitude
Venue
Name of the venue e.g. the name of a store or restaurant
Venue Latitude
Venue Longitude
Venue Category
# Methodology

Clustering Techniques
To compare the similarities of two cities, I decided to explore neighborhoods, segment them, and group them into clusters to find similar neighborhoods in a big city like New York and Toronto. To be able to do that, we need to cluster data which is a form of unsupervised machine learning: k-means clustering algorithm.
K-Means Clustering Approach- Most Common Venues
Most common venues near neighborhoods.
Note- Using credentials of Foursquare API features of near-by places of the neighborhoods would be mined. Due to http request limitation the number of places per neighborhood parameter were set to 100 and the radius parameter were set to 500.
# Results

Clusters in Scarborough
Average Housing Price by Clusters
School ratings by clusters
Location
Scarborough is a popular destination for new immigrants in Canada to reside. As a result, it is one of the most diverse and multicultural areas in the Greater Toronto Area, being home to various religious groups and places of worship. Although immigration has become a hot topic over the past few years with more governments seeking more restrictions on immigrants and refugees, the general trend of immigration into Canada has been one of on the rise.

# Conclusion

In this project, using k-means clustering algorithm, I separated the neighborhood into ten clusters and by using 103 different lattitude and logitude from dataset, which have very-similar neighborhoods around them. Through the charts above, results were presented for a particular neighborhood based on average house prices and school ratings.
# Future Use

This project can further be fine tuned to show precise and best choice housing by incorporating more independent varialbes during clustering stage.