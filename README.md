Extracting Restaurants data using Yelp API

Objective
By creating a well-rounded dataset that entails relevant details of a restaurant such as review count, rating, transactions, phone number, geographical and demographic details, it is made easier for researchers, business owners and entreprenaurs to study patterns in ratings and price looking at geographical and demographic details of the area, and build predictive models for the success of future busineses and make more informed decisions.

Datasets and stack used
1. Yelp Fusion Business Search API
2. List of United States cities by population from Wikipedia
3. BeautifulSoup library for scraping HTML content

Data and variables
1. Yelp Fusion Business Search API : Restaurants.csv
id - A unique ID for the restaurant
alias - alias of the restaurant
name - name of the restaurant
image_url - url of an image of the restaurant
is_closed - holds True if closed and False if not
url - website link of the restaurant
review_count - number of reviews
category alias - alias of the category
category title - title of the category
rating - the yelp rating out of 5
latitude - latitude coordinates of the restaurant
longitude - longitude coordinates of the restaurant
transactions - mode of transaction
price - affordability depicted by $ sign
street - address line 1	
apt - address line 2
area - address line 3
city - city it is located in
zip_code - zip code 
country	state - respective US State the restaurant is located in
display_address1 - first part of the display address
display_address2 - second part of the display address
phone - phone number of the business
display_phone - the phone number displayed for the customers 
distance - distance between you and the restaurant 

2. List of United Sates cities by population from Wikipedia : DemographicData.csv
2018rank - US city ranking by population 
city - US city, also the primary key for merging data
State[c] - repective US state of the city
2018estimate - estimated population of the city in 2018

3. Final Dataset : Final_Data.csv
id - A unique ID for the restaurant
alias - alias of the restaurant
name - name of the restaurant
image_url - url of an image of the restaurant
is_closed - holds True if closed and False if not
url - website link of the restaurant
review_count - number of reviews
category alias - alias of the category
category title - title of the category
rating - the yelp rating out of 5
latitude - latitude coordinates of the restaurant
longitude - longitude coordinates of the restaurant
transactions - mode of transaction
price - affordability depicted by $ sign
street - address line 1	
apt - address line 2
area - address line 3
city - city it is located in
zip_code - zip code 
country	state - respective US State the restaurant is located in
display_address1 - first part of the display address
display_address2 - second part of the display address
phone - phone number of the business
display_phone - the phone number displayed for the customers 
distance - distance between you and the restaurant 
2018rank - US city ranking by population 
city - US city, also the primary key for merging data
State[c] - respective US state of the city
2018estimate - estimated population of the city in 2018

Limitations/Challenges:
1. Limited number (maximum 50) of business results from Yelp Fusion API
2. Complex nested json 
3. Faced challenge in accessing the value as list from the dictionary
4. Challenge adding values with comma to csv
5. Complicated format of json made complex to extract the headers
6. Take care of csv alignment and distortion based on the missing values of key