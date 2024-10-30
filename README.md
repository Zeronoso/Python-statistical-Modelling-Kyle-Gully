# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The goal of this project was to analyze and model the relationship between the availability of nearby bikes, and the ratings of coffee shops in downtown Vancouver, BC, Canada. This was done by using
API data from CityBikes, Foursquare, and Yelp. I was looking to determine if there is a positive correlation between bikes available and business rating. This project was done to offer potential insight for business owners and/or potential investors 

## Process
obtain required information by parsing responses to Yelp, Foursquare, and Citybikes to get coffee shops and bars and their respective ratings, and coordinates. 
Afterwards, I placed the responses into a dataframe. Which I saved into a csv file to later combine all dataframes into a combined set.

Note I had to do data normalization for the ratings as Yelp was based on a total rating scale of 5 while FourSquare was on a total rating scale of 10.

After all the information was parsed we combined them all into a single csv file and created a visualization using a scatterplot with a regression line 
with the Y column as the ratings tab with the X row being the number of bikes. 

Afterwords I placed the findings into an SQLITE database that has been included in this repository for future usage.

Finally, I worked on creating a regression model. The results indicated a weak, positive relationship between bikes available and ratings.


## Results
Using the CityBikes, Foursquare, and Yelp API coverage of downtown Vancouver, BC Canada. I created a model to attempt to predict the ratings of coffee shops based on the number of nearby bikes available.
the regression models results indicates a weak, but positive relationship between nearby bikes available and ratings.

## Challenges 
grabbing data on yelp was a struggle with its limited calls per day.

Alot of the businesses provided via the api's had no/little ratings leaving a smaller dataset to work with and creating bias in variability

## Future Goals
I would look for other factors that could come into play that could have a bigger impact on ratings, such as proximity to nearby transportation (bus stops, skytrain entrances, etc), foot traffic, and population density.

collecting data over time on different months to analyze if seasonal trends could also influence the relationship between bikes available/ratings.

Develop an interactive interface with Tableau so that business owners/investors interested in my data could interact and explore the data themselves in a more user-friendly manner.
