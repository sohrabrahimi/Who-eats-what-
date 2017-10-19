# Who-eats-what-
In this project I will analyse the relationship between demographic factors and preferences for restaurant in different regions. 
# Install
This project requires Python 2.7 and the following Python libraries installed:

•	NumPy
•	Pandas
•	matplotlib
•	scikit-learn

You will also need to have software installed to run and execute an iPython Notebook
We recommend students install Anaconda, a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.

# Code
Template code is provided in the Taste_analysis.ipynb notebook file.  You will also be required to use the following CSV files to complete this project: independent_variables, table_business, table_review, yellowpages_zipcode_maindata. 

# Run
To Run the Taste_analysis.ipynb notebook file type the following in either anaconda or Command prompt. 
jupyter notebook finding_donors.ipynb
The paths to files may need to change depending on how you choose to download the files.  

# Data

 In this project we will use three data-sets: 

•	We will use the data provided by Yelp made available for its round 9 contest. The round 10 data-set is available here. However, I will use the round 9 data since I have previously conducted extensive data cleaning on it. This data includes 4.1M reviews by 1M users for 144K businesses as well as 1.1M business attributes (e.g., business name, parking availability and ambience). For this study we were only interested in restaurants in English-speaking North American metropolitan areas therefore, we filtered out Montreal and Urbana-Champaign (a small city) as well as points that fell out of the metropolitan boundaries. Also, we only used businesses tagged as restaurants. This process resulted in 2,186,054 reviews for 34,231 restaurants. This data is stored in two separate tables first the table_business which includes the following fields: Business ID, User ID, Reviews, Business Name, Star Rating, Address, City, State, Zip code, Business Category, Review Count, Longitude, Latitude. Seond the table_reviews which has the actual reviews , Business IDs and User IDs. 

•	We will also use the data that I have scraped from YellowPages. This data included the names and locations of restaurants across all zip codes in 48 contiguous U.S. states. Restaurants with no address or coordinates, and duplicates (instances with the same restaurant name and address—although these could have been legitimate separate franchises in one shopping mall/airport, etc.) were removed. Some restaurants had addresses while missing geographic coordinates information. For these restaurants, I used the Google maps API for geolocation. The original dataset held 824,218 records, and 796,763 remained. In our dataset, there are 505,735 independent restaurant brands and 291,028 restaurants that have different branches elsewhere (i.e. chain restaurants). This data-set includes a unique ID, Name, Category (e.g. Japanese, Mexican), Zip Code, Address, Longitude, and Latitude for all restaurants. This data-set is stored in yellowpages_zipcode_maindata.csv data-set. 

•	The socio-economic data-set has been downloaded from the American Community Survey Website (here). Once you go to this website, you will be directed to an interactive process where you choose the geographic units and the types of data that you would like. The following 7 data sets have been chosen for 5 digits U.S. zip codes: Total Population (we will divide this by zip code area to get population density), Age and Sex, Household and Families, Marital Status, Educational Attainment, Employment Status, Race, and Median Income in the Past 12 Months. Geographic data regarding the number of hospitals, schools, shopping centers, churches, recreation areas, museums, colleges and universities, government offices, and libraries in each zip code were extracted from Esri datasets. These datasets contained point information about each of the mentioned features. These points were then spatially joined with zip code polygons to determine which zip code each point was in. Socio-economic data along with this geographic data will constitute our dependent variables. All these data are stored in “Independent_variables.csv”. 

You can find these data-sets in this Google drive. 
