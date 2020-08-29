# Coursera_Capstone_Battle_Of_Neighborhoods
This is a repository for my capstone project for Applied Data Science Capstone course in IBM Data Science Certificate Specialization.

Project Workflow as follows:
1) Battle for Neighborhoods
	Populated Asian Population staying in London boroughs into DataFrame
	Took the average of population over the years and choose the location with highest Asian population

	Populated weekly earnings of Asian population staying in each boroughs in DataFrame
	Used earnings for the borough with highest Asian population

	Populated existing Licensed Restaurants in each boroughs into a dataframe
	Used Licensed restaurants for the borough with highest Asian population

	Rated Value per Sqm of the retail space in each borough data into a DataFrame

	As I have the Rated Value data from 2008 to 2017, I have to predict what will be the rated value in 2018. I will use Linear Regression Machine Learning algorithm to predict the 2018 rated value.
	I am taking the Earnings data and Licensed Restaurants data of "Newham" borough as the Independant Variables (X - variables) and will predict the Rated Value of the same borough and this predicted rated value becomes our Depedant Variable(Y-Variable)

	Data Cleaning :
	Merge all the 3 DataFrames of Earnings, Licensed Restaurants and Rated Value into a new DataFrame

	Data Exploration : 
	Observed that the Linear relationship exists between the Restaurants and the Rated Value
	A good model can be used to predict what the approximate rated value of the location

	The Rated Value for the year 2018 can be predicted somewhere between 160 to 165 using Simple Linear Regression
  
  Found the neighborhoods where the restaurant can be choosed using K-Means Clustering algorithms. (More described in below section).

2) Clustering for blogspot
	Decided to expose various boroughs in London and expose them into FourSquareAPI.
	Stored borough name, latitude and longitude
	Map stored boroughs on map using folium 
	After finding borough with highest Asian population, cluster the neighborhood only in this borough
	Populate AreaName, Latitude and Longitude in this borough
	Listed top 100 places around select borough upto a range of 500 kms radius
	Listed the venue, venue category, latitude, longitude into a dataframe
	Find the frequency of each venue category in given neighborhood
	Cluster the neighborhood venue categories grouping them by neighborhood. Also list top 10 popular places there
	Find the neighborhood which does not feature Asian restaurant in top 10 popular places.
