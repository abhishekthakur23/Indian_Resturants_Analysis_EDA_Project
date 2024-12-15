# Indian_Resturants_Analysis_EDA_Project

The goal of this project is to perform an in-depth analysis of Zomato restaurant data to identify key factors that influence restaurant success, as measured by customer ratings. By examining various attributes such as location, cuisine, pricing, service offerings (e.g., online orders, delivery, Wi-Fi, alcohol availability etc.), we aim to uncover meaningful patterns and trends that contribute to higher customer satisfaction and ratings. This will provide insights that can help restaurant owners and Zomato users make informed decisions.

# Data Overview

The dataset provides detailed information about restaurants listed on Zomato, including key features that describe their location, services, pricing, and customer ratings. Below is a summary of the dataset and its structure.

Dataset Structure:

1.	res_id: Unique identifier for each restaurant.
2.	name: Name of the restaurant.
3.	establishment: The type of establishment (e.g., Café, Fine Dining, Quick Bites).
4.	url: Zomato URL for the restaurant's page.
5.	address: The physical address of the restaurant (134 missing values).
6.	city: The city where the restaurant is located.
7.	city_id: A unique identifier for the city.
8.	locality: The locality within the city where the restaurant is situated.
9.	latitude & longitude: Geographical coordinates of the restaurant.
10.	zipcode: The postal code of the restaurant’s location (163,187 missing values).
11.	country_id: A unique identifier for the country.
12.	locality_verbose: A more detailed description of the restaurant’s locality.
13.	cuisines: The type(s) of cuisine served at the restaurant (1,391 missing values).
14.	timings: Operating hours of the restaurant (3,874 missing values).
15.	average_cost_for_two: The average cost for two people dining at the restaurant.
16.	price_range: A categorical variable representing the price range of the restaurant.
17.	currency: The currency used for pricing (e.g., INR, USD).
18.	highlights: Special features or services offered (e.g., Wi-Fi, Alcohol, Outdoor Seating).
19.	aggregate_rating: The average rating of the restaurant, as rated by users.
20.	rating_text: A textual representation of the rating (e.g., Good, Very Good, Excellent).
21.	votes: The number of user votes (reviews) received by the restaurant.
22.	photo_count: The number of photos uploaded for the restaurant.
23.	opentable_support: Indicates if the restaurant supports OpenTable reservations (48 missing values).
24.	delivery: Binary value indicating if the restaurant offers delivery services.
25.	takeaway: Binary value indicating if the restaurant offers takeaway services.


•	Dataset contains 211944 rows.
•	Dataset contains 26 columns.
•	Dataset contains Null Values.
•	Dataset contains 9 int type 4 float type and 13 object type columns.

Few Columns are get removed as we find it of no use or unnecessary for analysis.

These below columns removed from dataset.
“zipcode","address","country_id","res_id","url","locality_verbose","currency","opentable_support"

-	zipcode (due to missing values)
-	res_id (identifier, usually not useful in analysis)
- url (not useful unless analyzing web data)
-	locality_verbose and address (No potential use)
- currency (Single Currency)
- photo_count (unless analyzing photos)
- opentable_support (not relevant to our analysis)

# Missing Value Treatment

The dataset contains 168,634 missing values, which were addressed using various methods to ensure data integrity. Numerical data with missing values were imputed using the mean or median. In cases where the missing data was deemed insignificant to the overall analysis, the affected rows were removed. 
Additionally, for features where imputation wasn't appropriate, alternative techniques were applied to effectively handle the missing data.

# EDA

This EDA will provide valuable insights into restaurant success on Zomato, helping restaurant owners improve their offerings and guiding users in making better dining choices. The analysis will deliver actionable recommendations based on the relationship between various features and restaurant ratings. Visualizations like Histogram, Scatter Plot, Bar Plots etc. are employed to understand key factors and insights. The primary goal is to uncover patterns and relationships between various features such as cuisine, pricing, and service offerings, and their impact on restaurant ratings.


# Exploratory Data Analysis

This EDA will provide valuable insights into restaurant success on Zomato, helping restaurant owners improve their offerings and guiding users in making better dining choices. The analysis will deliver actionable recommendations based on the relationship between various features and restaurant ratings.Visualizations like Histogram, Scatter Plot, Bar Plots etc. are employed to understand key factors and insights. The primary goal is to uncover patterns and relationships between various features such as cuisine, pricing, and service offerings, and their impact on restaurant ratings.
