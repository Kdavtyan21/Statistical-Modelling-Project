# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The goal of this project is to determine how many bike stations or available bikes are near different point of interests in a chosen city (In this case I've chosen Assemini in Italy as my city of choice).

## Process
### First step was to get information on availability of bikes in a city of my choice and for that I went to citybik.es API that gives you information on available bikes in an area of your choosing in real time. From their API, I took a number of available bikes in an area based on latitude and longitude.
### Second step was to get information on points of interests (restaurants, bars, clubs, etc.) based on latitude and longitude that we got from step 1. In short we wanted to see how many POI were around available bikes or bike stations. For that we got API from Foursquare and Yelp. We used two different APIs for the same inquiry to see a difference in data that will be given to us and after getting both datas, Yelp provided more detailed description for the locations (ratings, open/close times, if the place is shut down.), Foursquare data was very barebones which resulted in a lot of data missing when joining those two datas together into one DataFrame.

## Results
After making a regression model to see if there is a correlation between an availability of bikes and longitute/latitude or places around bike stations. First multivatiate regression model showed that places around values should be removed from the model for better results. I went more in depth on the results and process of making the models [here](/notebooks/model_building.ipynb)
(fill in what you found about the comparative quality of API coverage in your chosen area and the results of your model.)

## Challenges 
Biggest challange that I've faced was incomplete data from foursquare API which had me creating more variables and columns to compensate for the lack of data.

## Future Goals
In the future I would like to only use Yelp API rather than 2 APIs to prevent a lot of incomplete data for better results. Another goal wold be making a visual representation of my findings and using Tableau as a software for it.
