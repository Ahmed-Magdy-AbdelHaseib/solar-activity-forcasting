# Ford GoBike System Data Exploration
## by: Ahmed Magdy Abdelhaseib Mohamed


## Dataset

There are 170839 trips in this dataset with 18 features like ('duration_sec','distance_Km', 'day_of_week', 'user_type',..etc) these trips happened in the period between febreuary and march in 2019. i made some data wrangling, i created two features from the data features ('distance_Km', 'day_of_week') and There were some missing values, trips with distances equal 0 and some illogical values in the member_birth_year like (1878, 1910, 1920,....etc) so, i removed all these values.

## Summary of Findings

In the exploration, I found that there was a strong relationship between the duration of a trip and its distance, with some effects from the other infromations about the trip like (user_type, day_of_week, member_gender, bike_share_for_all_trip). Duration variable has a weak correlation with the distance varible when they are plotted on thier standard scales but they have a very strong positive correlation Approximately linear after plotting the two variables on the log-scale.There was also an interesting relationshipe between the duration and distance variables with the categorical variables. we know that increasing the distance makes the duration increase but we observe that subscribers can do long trips in short durations than customers and slightly males can do that than females and aslo not shared bikes can do long trips in short durations than shared bikes.there indeed is a positive effect of days and gender of the rider and his type on the duration of the trip, we saw in the plots that riders who are subscribers and mals have the lowest average trip duration in general and a day like "Tuesday" has the lowest avarge durations than other days althought "Saturday" has the lowest avarage distance.

Out of the main features i explored the effect of the member_birth_year on 
the trip duration but it have very weak negative correlation with the duration.


## Key Insights for Presentation

For the presentation, I focus on just the influence of the main feature ('distance_Km', 'day_of_week', 'user_type','member_gender'). I start by introducing the duration variable, followed by the pattern in distance distribution, Distribution of riders birth year and Distribution of Trips over the weekdays. then plot the transformed scatterplot of duration and distance features.

Afterwards, I introduce each of the categorical variables one by one. To start, I use the box plots of duration and distance across user type. I'm only looking at the user type plot here since it's a very clear example of how the categorical variable affect trip duration.
The other two categorical variables, member gender and day of week, are covered afterwards, using heat maps to show how weekdays and the gender if the rider affect trip duration regardless its distance.ss