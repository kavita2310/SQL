<h1>Airbnb Hospitality Intelligence Hub project(SQL)</h1>

Airbnb is a leading online marketplace that provides accommodation options across various neighborhoods in New York City 
and around the globe. To ensure their business operations run smoothly, Airbnb has developed a cutting-edge 
'Hospitality Intelligence Hub' that analyzes data from various sources for better insights and trends. 
By using SQL, Airbnb gains valuable insights into their business operations, which help them make informed, data-driven decisions. 

<h1>Project overview:</h1>

The 'Hospitality Intelligence Hub' uses SQL to analyze data which contains information on various neighbourhoods 
in New York City, including the types of listings available, the prices of these listings, and their availability. 
The system tracks trends in customer behaviour and preferences, such as frequently booked room types, 
price trends for specific neighbourhoods etc.With use SQL, Airbnb can identify areas for improvement and make changes to their operations to 
improve customer satisfaction. For example, the 'Hospitality Intelligence Hub' helps Airbnb optimize pricing for different neighborhoods to 
increase occupancy rates, improve listings based on customer preferences, and enhance the customer experience by identifying areas for improvement.
 

<h1>Dataset:</h1>

The dataset consists of two tables:<br>
Table 1: Listing Table: The ‘Listings' table contains information on the various neighbourhoods in New York City, including the 
types of listings available in each neighborhoods. 
•	id: A unique identifier for each listing.<br>
•	Name: The name of the listing.<br>
•	Host id: A unique identifier for the host of the listing.<br>
•	Host Name: The name of the host.<br>
•	Neighborhoods Group: The group of neighborhoods that the listing belongs to.<br>
•	Neighborhood: The name of the neighborhood that the listing belongs to.<br>
•	Room Type: The type of room that is being listed (e.g. private room, entire apartment).<br>

Table 2: Booking Details Table: The Booking details table contains information on the various price, minimum nights, number of reviews etc.<br>
•	Listing id: A unique identifier for each listing.<br>
•	Price: The nightly price of the listing.<br>
•	Minimum Nights: The minimum number of nights that a guest must book in order to stay at the listing.<br>
•	Number of Reviews: The total number of reviews that the listing has received.<br>
•	Reviews per Month: The average number of reviews that the listing receives per month.<br>
•	Calculated Host Listings Count: The number of listings that the host has on Airbnb.<br>
•	Availability 365: The number of days that the listing is available for booking throughout the year.<br>

<h1>Data Sources:</h1>

The data use for this project available from the kaggle. Which  contain information on host name, neighbourhoods group, number of reviews etc.


<h1>Technology used:</h1>

SQL: For querying of the analysis include.<br>
Tableau: For data visualization.<br>
Pandas: For data cleaning.<br>


<h1>Tasks:</h1>

1)	Data cleaning and preparation: Clean and pre process the data by handling missing values, data formatting.<br>
2)	Data Analysis: Perform descriptive statistics and data visualization to identify trends, patterns and correlations.<br>
3)	SQL Querying: Write a SQL Queries to retrieve specific data, perform aggregation and join tables.<br>
4)	Insight Generation: Generate actionable insights and recommendations based on the analysis.<br>



<h1>Insights and Findings:</h1>

1)	Top 5 Host by Price: Phil, Rafael, Girish, Carmel, Dimitri.<br>
2)	Top Neighbourhood Group by minimum nights : Queens, Bronx, Brooklyn, Manhattan.<br>
3)	Top 5 Neighbourhood by Price and Availability : Lower east side, Upper west side,  East harlem, Harlem, Prospect heights.<br>
4)	Top 2 Room Types by Minimum night Entire home/Apartment and Private room.<br>
5)	Top 4 Host by Reviews per month: Akshay, Girish, Karen, Terrance.<br>
6)	Top 5 Name by Calculated host listing count:<br>
•	Private unit close central park.<br>
•	#1 Private room near central park.<br>
•	#1 large studio near central park.<br>
•	Cozy private room in L.E.S.<br>
•	Large Brooklyn 3 bedroom apartment.<br>
