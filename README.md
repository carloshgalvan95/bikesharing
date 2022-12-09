# NYC Citi Bikes

## Overview
Now that we've gotten a good idea of how to create our story, there is still some more work to be done to convince investors that a bike-sharing program in Des Moines is a solid business proposal. To solidify the proposal, one of the key stakeholders would like to see a bike trip analysis.

For this analysis, you’ll use Pandas to change the "tripduration" column from an integer to a datetime datatype. Then, using the converted datatype, you’ll create a set of visualizations to:

- Show the length of time that bikes are checked out for all riders and genders
- Show the number of bike trips for all riders and genders for each hour of each day of the week
- Show the number of bike trips for each type of user and gender for each day of the week.
- Finally, you’ll add these new visualizations to the two you created in this module for your final presentation and analysis to pitch to investors.

As mentioned before, the purpose of the analysis is to visualize the data gathered from NYC Citi Bikes to grasp the decision making and data behind it.

![dashboard](https://github.com/carloshgalvan95/bikesharing/blob/main/NYC_citi_bikes_dashboard.png)

## Results

### Supply and demand
First and foremost, we have to analyze the number of rides during the month of August, and contrast those numbers to the actual population of New York. That information will give us an idea of the number of rides per citizen, and then we can estimate a very rough amount of what we could expect at Des Moines.

|**City**  |**Number of Rides**|**Population**|
|----------|-------------------|--------------|
|New York  |2,344,224          |8.64 Million  |
|Des Moines|**58,697**         |212,031       |

Therefore, our goal metric and expected number of rides when the business is consolidated would be 58,697 for a summer month.

The Next thing to analyze would be the lowest and peak hours of the day, we need to:

- Ensure that the number of bikes provided are going to be enough to satisfy the demand during peak hours.
- Determine when the best hours would be for maintenance.

### Most important hours of the day

![august_peak_hours](https://github.com/carloshgalvan95/bikesharing/blob/main/August%20Peak%20Hours.png)

On our plot, we can see that the peak hours for NYC Citi Bikes are between **4:00 pm to 7:00 pm** with a peak demand of roughly **225,000 rides**.

Taking into consideration our metrics above, we should aim for an estimate of **5633** rides on our peak hours and ensure the investment is enough to satisfy that expected demand.

We can also see that the best maintenance hours to ensure peak demand is maintained are going to be between **2:00 am to 4:00 am**.

### Best equipped stations

![top_starting_locations](https://github.com/carloshgalvan95/bikesharing/blob/main/Top%20Starting%20Locations.png)
![top_ending_locations](https://github.com/carloshgalvan95/bikesharing/blob/main/Top_Ending_Locations.png)

From the data gathered from NYC Citi Bikes we can also observe that the top starting and ending locations coincide most of the time, this will help us determine the best equipped stations that we will need to have to ensure meeting the demand, as well as strategic middle points between them and carefully and slowly expand the available stations assessing the peak hours every month.

### Average trip durationg

![avg_trip_duration](https://github.com/carloshgalvan95/bikesharing/blob/main/Average_Trip_Duration.png)

From this chart we can also gather information that will help us determine the amount of bikes that we will to consider for the initial investment, the proposed strategy is to launch an app where we can see metrics for initial subscribers a few weeks prior to the launch in Des Moines, given that the age of the subscribers is a decisive factor on trip duration, looking at the data of our subscribers can give us a rough estimate of trip duration we will observe.

We can also see this by analyzing the data for average trip duration in minutes by gender and in general numbers we see for New York in the charts below.

![checkout_times_users](https://github.com/carloshgalvan95/bikesharing/blob/main/Checkout_Times_For_Users.png)
![checkout_times_gender](https://github.com/carloshgalvan95/bikesharing/blob/main/Checkout_Times_gender.png)

We can see that the gender is also an important metric to observe in our initial subscriber.

![user_trips_gender](https://github.com/carloshgalvan95/bikesharing/blob/main/Trips_gender.png)

### User trips by weekday

The only way to properly analyze our peak hours will be to determine peak hours as well as peak days in demand. From the chart below, we can see that, Monday, Tuesday, Thursday and Friday will be our most important days and safely assume that the most important factor to determine the success of the project is to analayze the main Work Areas in Des Moines and focus our attention there. 

![user_trips_gender_weekday](https://github.com/carloshgalvan95/bikesharing/blob/main/User_Trips_gender_weekday.png)

The fact that the days with most demand are not weekends paired with the information on peak hours is enough to assume that the main use is for conmute to work places.

![user_trips_weekday_hour](https://github.com/carloshgalvan95/bikesharing/blob/main/User_Trips_weekday_hour.png)



## Summary

Based on the data we observe in New York City we can safely assume that the project can be succesful as well in Des Moines.

The key factor to ensure this success are going to be:
- Ensure that the initial investment is going to be enough to satisfy the demand during peak hours
- Gathering data before launch day from a subscribe based app to use the bikes to analyze metrics of potential users based on genre and age
- Gathering information about the most common commute routes and most important Work Activity Areas in Des Moines
- Scheduling Maintenance hours during least concurent hours of demand

## Resources
[link to dashboard](https://public.tableau.com/views/NYC_citi_bikes_challenge/Story1?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)
