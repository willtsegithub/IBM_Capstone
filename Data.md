# Data
The purpose of the project is to segregate different neighborhoods based on demographic and F&B specific data. We first need to decide what features are necessary to perform this analysis.
Our project focuses on setting up a new Asian restaurant. Therefore it is good to first understand the population or racial profile of the neighborhoods, e.g. find out the Asian population or ratio of Asians in the neighborhood. Spending power of the neighborhood can reflect the affordability of potential customers. Median household income can be a good indicator of the spending power. Here we assume a strong and direct relationship between the income of a household and their corresponding spending power. We also want to know if there is competition from similar type of restaurants in the neighborhood. The number of Asian restaurants in a neighborhood could be a good representation of competition within that neighborhood.
We have identified 3 main features to perform our clustering analysis. They are:
- Median household income
- Asian percentage
- Number of Asian restaurants
If we want to further investigate the competition from other Asian restaurants, the rating of Asian restaurants in the neighborhood could add additional analysis to the clustering result. There may not be Asian restaurant in every neighborhood and therefore we cannot add this feature to the clustering analysis. This becomes an optional feature. The optional feature is:
- Average Asian restaurant rating


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
