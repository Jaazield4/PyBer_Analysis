# PyBer_Aanlysis

## Overview
Used the groupby method on multiple columns to create a summary dataframe. The summary dataframe included the total rides, total drivers, total fares, average fare per ride, and average fare per driver. By doing so we are able to analyze the information for each city type. We also found the total weekly fares for each city type from January 1, 2019 to April 29, 2019 by using the groupby method on the pyber_data Dataframe, and displayed the information on a multiple line graph. To create the line graph with the proper information displayed we first needed to take the information from the merged dataframe and apply the groupby method to both the "date" and "type" column. Then proceeded to use the loc method on the new dataframe to get only the dates needed into a new dataframe which will be used for the line chart.  

### Purpose
Completing this project gave a better understanding of creating and formatting dataframes as well as give more practice to using the loc and groupby methods. This project also introduced new methods such as the pivot(), resample() and DatetimeIndex, that will be of help in future work.

## Results
### Ride-Sharing Summary Dataframe
By creating the summary dataframe we are able to quickly see the difference in ride-sharing data between the different city types.

![image](https://user-images.githubusercontent.com/85451089/127048902-ccfba2a7-20a0-47f8-996e-e24fb1b8b177.png)

As shown in the image above rural cities have a much greater average fare per ride and per driver while urban cities have low average fares for both ride and driver. Because rural cities are much less populated than urban areas we can see the major difference from 125 total rides in rural cities to 1625 total rides in Urban cities. There is also a major difference in drivers as urban cities have over 30 times as many drivers as rural cities. 

### Total Weekly Fares for City Type Line Chart
Using a multiple linechart we are able to see the differences in ride-sharing data between rural, suburban, and urban cities at a glance.

![image](https://user-images.githubusercontent.com/85451089/127050170-6ccb2b1e-764c-480b-8fc7-79f883dbb52a.png)

In the chart shown above we can see the total fare per moth by city type. Even though we concluded that urban cities have a much lower average fare per ride and driver than rural cities, it is clear by seeing the line chart above that urban cities had a much higher total fare than rural cities between January 2019 to April 2019. Suburban cities found themselves somewhere in between rural and urban cities. Towards the first couple weeks in April we can see that the total fares in suburban cities dipped closer to the total fares in rural cities. We can aslso see that all three city types had a small jump in total fares during the final weeks of February leading into March. 

## Summary
Between the city types, Urban cities are the only ones to have more total drivers than total rides making the average fare per driver lower than the average fare per ride. To decrease the disparity between the city types, PyBer could focus more advertisement for people in uraban cities to use PyBer, thus increasing their total rides which will higher their Average Fare per Driver. Urban cities bring in much more revenue than the other city types, this could simply be due to the difference in population. However, the reason could also be tied to the Average Fare per Ride which is much higher in rural and suburban cities than in Urban. It is possible that by lowering the Average Fare per ride in rural and suburban cities the quantity of total rides will increase to a point which brings in a higher total fares. Third PyBer could lower the disparity between the cities by increasing the number of drivers they have for rural and suburban areas. This will allow for more available drivers at any given time, and drivers will need to drive shorter distances lowering the average cost per ride. 
