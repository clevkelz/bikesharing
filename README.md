# Bike Sharing

## Overview of the Analysis

Ridership data from the Citi Bike sharing program in New York (https://s3.amazonaws.com/tripdata/index.html) was evaluated to determine whether a similar program could be feasible in Des Moines, Iowa.  Data from August 2019 were selected for review as selecting a month with warmer weather would result in a more robust set of information to analyze.  The data contained the following fields:
- Trip Duration[^1]
- Start Time and Date
- Stop Time and Date
- Start Station Name
- End Station Name
- Station ID
- Station Latitude and Longitude Coordinates
- Bike ID
- User Type (a customer had a 24-hour or 3-day pass while a subscriber was an annual member)
- Gender (unknown, male, or female)
- Year of Birth

## Results

The results of the analysis are housed in this [Tableau Story.](https://public.tableau.com/app/profile/kelley.richards/viz/CitiBikeRideSharing_16627616385190/sheet8)

Eight visualizations were made as follows:

### Checkout Times for Users

![image](https://user-images.githubusercontent.com/106293233/189464125-6f8f4693-8a33-4c4b-9cc2-1c759adaf1d4.png)

Most rides are short; the peak ride time is only five minutes.  This suggests that many trips are purpose-driven such as to commute to work, to run errands, to visit friends, etc. rather than leaisurely rides.

### Checkout Times by Gender

![image](https://user-images.githubusercontent.com/106293233/189464391-1119a7c4-a276-470b-907f-c731d39a72d5.png)

Trip duration peaks at the same time for men and women but levels off more slowly for men, indicating that men tend to take longer trips than women.  This visualiation also shows that there are much more male than female riders which is corroborated by the Gender Breakdown pie chart.

### Trips by Weekday per Hour

![image](https://user-images.githubusercontent.com/106293233/189464580-da39bf9d-5b34-478e-bf71-85a66cfc8b90.png)

This heatmap illustrates that ridership is highest during the morning and evening commute times during the week but is more evenly distributed among daylight hours during the week.  Bikes may need be redistributed on the weekdays to reflect this different demand pattern.

### Trips by Gender (Weekday per Hour)

![image](https://user-images.githubusercontent.com/106293233/189464706-f0501ea7-5a2f-4cfd-a123-0e8e6d693ed3.png)

This heatmap does not show a distinct difference between the peak ridership times (as described above) for men and women.

### User Trips by Gender by Weekday

![image](https://user-images.githubusercontent.com/106293233/189464941-e00eec73-8d01-4d87-b286-8f32b53ce8ed.png)

This heatmap illusrates that customers are more likely to use bikes on the weekend, which indicates that these are more casual riders.  The heaviest use for subscribers is during the week, particular on Thursdays.  This suggests that subscribers may rely on the Citi Bikes for a regular mode of transportation.  The heatmap also shows that more rides are made by subscribers than customers, which is corroborated by Customer Type pie chart.  Finally, this heatmap illustrates that men are more likely to be subscribers.   

### Gender Breakdown

![image](https://user-images.githubusercontent.com/106293233/189465063-e8feae87-de51-4e35-b226-a55645e7a252.png)

This pie chart shows that men are the large majority of riders.  

### Customer Breakdown

![image](https://user-images.githubusercontent.com/106293233/189465180-c2f0dd28-c043-4ace-ae96-f9803909336f.png)

This pie chart shows that subscribers, who have an annual membership, make up the substantial majority of the riders.

### August Peak Hours

![image](https://user-images.githubusercontent.com/106293233/189465363-27e8182e-e9c8-4dd5-8b5e-8fa5e8e787a5.png)

This bar chart demonstrates that the highest number of rides occur in the evenings.  This main supports the results from the Checkout Times for Users chart; however, there are differences in usage patterns for weekdays and weekends. 

## Summmary

### General Conclusions

These visualizations provide important conclusions about the Citi Bike riders.  These key takeaways should be considered when developing a plan for a similar program in Des Moines:
- Short trips appear to be the "sweet spot" so successful business plan should focus on high volume with enough stations to cater to these quick trips.
- Bikes should be readily accessible to people's houses in the morning hours of the weekdays and then quickly available near workplaces in the evening hours.  Bikes may need to be redistributed on the weekends to accomondate a more steady demand throughout the day.
- There appears to be a strong relationship between subscribers and regular use of the bikes.  Benefits of subscribership should be highlighted when developing marketing plans.
- Men use the bikes more often, indicating that they likely see the bikes as a regular, reliable form of transportation.  Marketing research should be conducted to see why women are more reluctant to use the bikes.

### Additional Visualizations to Explore

Adding visualizations that focus on the age of the riders could guide decisions regarding where more bikes are needed; for example, if younger people use the bikes more often, more bikes should be placed near college campuses or other areas to which young poeple flock.  Visualizations that show the distance traveled from the start station could help planners map out where additional stations may be needed and whether bikes may need to be more regularly repaired from these stations as longer trips could result in more wear and tear to the bikes coming through there.















[^1]: The trip duration data were modified using Python to change the format from an integer to a datetime datatype to make it possible to render this information correctly in Tableau.
