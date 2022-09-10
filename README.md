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












[^1]: The trip duration data were modified using Python to change the format from an integer to a datetime datatype to make it possible to render this information correctly in Tableau.
