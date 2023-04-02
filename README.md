# Ford GoBike System Data Exploration
## by Hadil Jilani


## Dataset

This data set includes information about 183412 individual rides made in a bike-sharing system covering the greater San Francisco Bay area. It includes features such as the start- and end-times, start- and end-locations, duration and information about the user such as their type, gender, year of birth etc..

Before starting the investigation, I did some preliminary wrangling such as dropping missing values. I also converted user types, user gender and whether the bike was shared the entire trip or not into categorical variables to facilitate the exploration. I converted the start- and end-time of the trip into datetime format, and converted the IDs and birth year to integers.


## Summary of Findings


In the exploration, I looked for the effect the indicators of the trip have on the average duration. I found that there was a strong relationship between the average duration and the user types. With a big difference, customer have tendencies to conduct average longer trips than subscribers. The user type seems to be a strong predictor of the length of trip.

As for the gender, the investigation showed that gender can play a role in predicting the average duration of the trip, with the other genders having the highest value, then females then males.

Another interesting Feature was the time of the day in which the trip started. Surprisingly, there was a strong peak in hours between 1am and 4am with a duration of 1500 sec (25 min).

I wanted to look at the relationship between these variables and their effects on the average duration. The exploration confirmed that the hour of the day was alone a strong predictor itself on the average duration.

Outside of the main variable of interest, there wasn't any inetersting relationships. However the variables were not fully independent, as there was a strong domination of males among the subscribers.

## Key Insights for Presentation

For the presentation, I focus on just the influence of the hour of the day, user types and gender of users. I start by introducing the duration variable, followed by the user types and then gender distribution.

Afterwards, I introduce the relationships between user types, hours of the day and the average duration as it conveys both information (bivariate and multivariate distribution) in the same plot. Same thing goes to the influence of the hour and the gender on the average duration. These categorical variables are not ordinal and have only two or three different values. So there is no need for gradual colormap or palette. the default palette conveys better the information without confusing the audience.