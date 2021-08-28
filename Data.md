# Data
We will make use of open to public location data and demographic data to cluster neighborhoods based on the following criteria:
- Number and type of restaurant:
  - Source: Four Square
  - Method: We discover the number and type of restaurants in each neighborhood of the New York City

- Competition from same/similar type of restaurant
  - Source: Four Square
  - Method: We find out the rating of each restaurant and use it as a basis to estimate competition

- Household median income:
  - Source: Zipatlas
  - Method: The median income of each neighborhood tells us the affordability of potential customers, e.g. number of Asians

- Target customers
  - Source: Zipatlas
  - Method: We can analyze the racial profile of each neighborhood and find out the potential of each neighborhood

- Neighborhood name
  - Source: Json file provided by IBM Skills Network Labs

- Zip/Postal code
  - Method: We can convert latitude and longitude from the Json file above to Zip/Postal code by a method in the Geopy library

After clustering the neighborhoods, we will further differentiate clusters by their physical locations on a folium map.
