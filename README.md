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







[^1]: The trip duration data were modified using Python to change the format from an integer to a datetime datatype to make it possible to render this information correctly in Tableau.
