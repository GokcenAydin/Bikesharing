# Bikesharing

## Overview of the Analysis

The purpose of this analysis was to inspect and visualize the August 2019 data on 'bike-usage as a commute' from 
the Citi Bike program in New York city with the aim of applying a similar program to start a business in Des Moines.
Five different visualizations and a story bearing the results of the analysis were created in this module to highlight 
the key information below: 

- The checkout times of users as a total with a filter on tripduration 
- The checkout times of users by gender with a filter on gender and tripduration
- The number of trips by weekday for each hour on a graph of heatmap
- The number of trips by gender and by weekday per hour with a filter on genders and on a graph of heatmap
- The trips by gender by weekday with the filters of usertypes and genders
- A new summary created by using three visualizations to support the key findings of the analysis.

## Results of the Analysis

### Converting the Data

Using Python and Pandas functions, the "tripduration" column in data was converted from an integer to datetime datatype, a
new DataFrame was created as shown in the visual below, and exported as a CSV file to use for the analysis.

<img width="494" alt="Capture1" src="https://user-images.githubusercontent.com/104400293/205478449-4db0ca0a-38df-4f3d-8657-53e150eb2594.PNG">

### Checkout Times for Users

Using Tableau, the number of checkout times were visualized for all riders on a line chart with a filter of tripduration per hour and per minutes. 
As seen on the chart, the number of the trips with a checkout time of less than one hour is giving the highest values when compared
to the general, showing that a great majority of the users used a checkout within less than an hour, with a peak of 146,752 users with
a duration of 5 minutes.
The number of the users commuted over one hour shows a value of within 0K according to the chart. In this case, the most preferred 
duration of usage can be considered as maximum one hour.

<img width="562" alt="Capture2" src="https://user-images.githubusercontent.com/104400293/205478452-b01c94cb-fca9-46d2-acf6-2dd716d22c0b.PNG">
[link to dashboard] (https://public.tableau.com/app/profile/gokcen.aydin/viz/CheckoutTimesforUsers_16701360990770/CheckoutTimesforUsers?publish=yes)

### Checkout Times by Genders

The chart created to visualize the number of checkout times for users in the previous step was updated with an additional classification 
of genders in this step as shown below. Using an IF condition, a new table, showing the number of checkout times by genders, was created,
classified by using colours as a marker, and was also shown as a filter.
The number of male users -within the checkout times of under one hour- showed the highest numbers in the chart when compared to female and 
gender-unknown users. While the number of male users reached a peak of 108,087, the peak number of female users was 34,151.

<img width="598" alt="Capture3" src="https://user-images.githubusercontent.com/104400293/205478455-eba8b954-bdc7-4d56-9b14-425ff8df7790.PNG">
[link to dashboard] (https://public.tableau.com/app/profile/gokcen.aydin/viz/CheckoutTimesbyGender_16701362868470/CheckoutTimesbyGender?publish=yes)

### Trips by Weekday per Hour

On this graph of heatmap, the number of trips were given in a daily stoptime distribution grouped by hour of starttime. The count of trips were
accompanied with a colour, where larger numbers were associated with darker colours.
The graph showed that, the largest numbers of trips were seen on Thursdays as a stoptime, and with the starttime of 5:00 pm and 6:00 pm.

<img width="604" alt="Capture4" src="https://user-images.githubusercontent.com/104400293/205478462-95b373a2-2f82-4ed9-a3ea-f5bb7cd3c7bc.PNG">
[link to dashboard] (https://public.tableau.com/app/profile/gokcen.aydin/viz/TripsbyWeekdayperHour_16701363878050/TripsbyWeekdayforEachHour?publish=yes)

### Trips by Gender by Weekday per Hour

In this step, the graph of heatmap created in the previous step was updated with a classification of genders. As the highest majority of the users
were male, the heatmap showing the male users' information gave the highest range of distribution, and the largest number of values in the males-graph
showed a great similarity with the values of the all-users graph. A filter on genders was added to the graph.

<img width="571" alt="Capture5" src="https://user-images.githubusercontent.com/104400293/205478464-4cba9369-9c49-40b2-8fc2-e81e377beb18.PNG">
[link to dashboard] (https://public.tableau.com/app/profile/gokcen.aydin/viz/TripsbyGenderbyWeekdayperHour/TripsbyGenderbyWeekdayperHour?publish=yes)

### Trips by Gender by Weekday

In this graph of heatmap, the numbers of female, male and gender-unknown users were distributed with a classification of customer and subscriber options
and by a grouping of weekday as a starttime. The larger number of trip counts were associated with darker colours.
In this graph, the values showed that a greater majority of the female and male users were subscribers, while a larger number of gender-unknown users was
in customer group. As a summary of this graph, male subscribers showed the larger numbers of trips with a peak of 259,316 and with Thursday as the most popular
starttime.

<img width="516" alt="Capture6" src="https://user-images.githubusercontent.com/104400293/205478471-e8971538-78c4-4341-a905-16162a4b0e5d.PNG">
[link to dashboard] (https://public.tableau.com/app/profile/gokcen.aydin/viz/TripsbyGenderbyWeekday_16701365555030/TripsbyGenderbyWeekday?publish=yes)

### Bikesharing Story

In the story of this analysis, three visualizations created in this module were used to summarize and highlight the results: Checkout Times for Users, 
Trips by Weekday for Each Hour and Trips by Gender by Weekday. 

<img width="495" alt="Capture7" src="https://user-images.githubusercontent.com/104400293/205478476-bd41d742-d82d-42e1-9ad2-c630a6249a44.PNG">
[link to dashboard] (https://public.tableau.com/app/profile/gokcen.aydin/viz/BikesharingStory_16701366390160/BikesharingStory?publish=yes)

## Summary of the Analysis

The various graphs created with the August 2019 data of the Citi Bike program showed that within that certain duration of the year, the majority of the usage 
duration was under one hour with a majority of male users. The most preferred trip start times were between 5:00 pm and 6:00 pm on Thursdays as the stop time,
and with a majority of male users, and the larger number of the trips were done by the male subscribers, mostly on Thursdays. 
The two visualizations stated could be done to improve the content of this analysis:

- Start and End Station Latitude and Longitudes could be used to visualize the locations in which the program was mostly preferred as a commute type so as 
to understand the possible reasons why bike trip was preferred. 
- Birth year of the users could be visualized to understand the age range of the users that prefer this program so as to make a market investigation of the
areas that could help to reach these age groups for a public relations study. 
