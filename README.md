# PyBer Analysis

## Overview of Analysis

### Purpose 
-   After starting a new job at a ride sharing company, PyBer I was tasked with a new assignment revolving around ride-sharing data by city type. The city types were broken down in to 3 subcategories: Urban, Suburban, and Rural.  The main goal of the assignment was to analyze and present the comparisons between the three city types based on the sum of their fares by month over a four-month period (Jan 2019 - April 2019). By going through the data, we can see the major key differences between the city types with relation to the number of drivers in those cities and number of rides. Reviewing these items further helped paint a picture as to why the weekly/ monthly fares were so different. 

-   The Data we were drawing from initially came from two CSV files, that we ultimately merged in to one Data Frame that broke down the data by specific city, city type, the number of drivers that were in that city, the date of those rides, and the unique ride ID (ID number specific to that ride on that date/ time).


## Results
### Ride-Sharing Data Among City Types
-  Between the three city types, see a breakdown of total data below in a table created using the code shown in [PyBer_Challenge.ipynb](https://github.com/Jess-Vannatter/PyBer_Analysis/blob/main/Starter_Code/Starter_Code/PyBer_Challenge.ipynb). The code was used to pull the data from the two CSV file [Resources](https://github.com/Jess-Vannatter/PyBer_Analysis/tree/main/Starter_Code/Starter_Code/Resources) merged in to one data frame ```pyber_data_df = pd.merge(ride_data_df, city_data_df, how="left", on=["city", "city"]))```. The numbers represent the totals over a 4 month period (Jan 2019 - April 2019) [PyBer_Challenge.ipynb](https://github.com/Jess-Vannatter/PyBer_Analysis/blob/main/Starter_Code/Starter_Code/PyBer_Challenge.ipynb).
 	
![image](https://user-images.githubusercontent.com/117245167/208255021-aa46866b-1686-4a48-82ef-31c8ef8914d5.png)

### Differences in Ride-sharing Data among City Type
-   When reviewing the data presented above, one can draw a couple obvious conclusions. Urban areas are going to usually have a higher number of drivers and rides, which makes sense because the population will usually be higher/ denser in an urban setting. the table above corresponds with this statement, showing both total rides, and total drivers increasing drastically from Rural, to Suburban, and then even more to Urban areas.  As a result, the total sum of fares will increase as we go from more rural areas to Urban areas. I would consider this to be a positive correlation. With that being said, even though the total number of fares increases as we go towards more rural areas, there is a negative correlation between the average fare per ride/ per driver. The figures for Average fare per Ride and Average Fare per Driver decrease as we go from rural areas to Urban areas. Even though the total fares figure for Urban areas is almost 9.3% times higher than compared to the Rural areas, because there are so many drivers and rides in urban areas the averages are much lower. Making the Rural and Suburban areas more efficient

### Total Fare's by City Type
![PyBer_fare_summary.png](https://github.com/Jess-Vannatter/PyBer_Analysis/blob/main/Starter_Code/Starter_Code/analysis/PyBer_fare_summary.png)
-   The graph above, also located in the [Resources](https://github.com/Jess-Vannatter/PyBer_Analysis/tree/main/Starter_Code/Starter_Code/analysis) folder, further breaks down the data and provides a visualization of fare amounts by city type each week within a given month. This helps determine several items with regards to the ride-share data. It helps pinpoint which months are more successful across all city types or possibly which month was more successful for just one specific city type. Inversely, we can see which months have lower performance across all three city types/ or which city type preformed particularly poor during that period. This allows us to look deeper into the data by looking past the population differences. For instance, we can see that the end of February seems to be a rather successful time for PyBer ridesharing as we see spikes in total fare amounts across all city types in the third week of march Which is followed by a decrease in all city types by the 4th week/ end of March. In Addition, Urban cities see a lot of variation in March, as compared to Rural and Suburban cities. Each week results in a rather sharp increase, followed by a decrease. As compared to a rather consistent or flat data line for both Rural and suburban cities for the month of march.

## Summary 
-   Reviewing the data as a whole we see that even though Urban cities have a much higher total fare sum than Rural and Suburban cities, the Rural/ suburban cities are much more efficient. With there being less drivers than rides in both Rural and Suburban cities, it is more lucrative for the drivers and the company because a larger share of the fares are taken in (With Suburban cities being the most efficient). Whereas in the Urban areas, there is an over saturation of drivers causing the supply to outweigh the demand which leads to a loss of money. 
### Business Recommendations
-   How do we get more rides in Rural area's/ city types to drive up total fares for rural areas overall?
    -    With Rural Cities having the lowest Total rides and lowest total fares we should look to drive up rides in these cities. In order to be more efficient, we would want the drivers to stay relatively the same and have the rides increase. So possibly providing incentives to consumers to order more rides in these areas may be beneficial. Whether it be discounts or promotions, it may lead to more dividend.

-   Urban areas have too many drivers, which is driving down the average fare per ride/ driver.
    -   Depending on what the company is looking for as the preferred avg fare per ride/ driver. It may be best to look to reduce the number of total drivers in Urban Cities. Urban cities according to the data is the only city type that has more drivers than rides. Essentially, we have too much supply in Urban cities. In order to be more efficient, it might be best to look into which specific Urban cities have the highest driver to ride ratio and look to cut drivers in those cities.

-   Why are certain times of the year or moth more productive than others. How do we recreate this in other, slower producing times of the year?
    -   I would suggest doing more research in to why there was a spike in fares/ rides at the end of February. Is this possibly a geographic cause? We would need to know more about the specific location (state) of the cities. I addition there appears to be a spoke for Urban and Rural Fares at the end of April, While Suburban stayed relatively consistent. It may be best to look into the weather/ climate of these cities (or the state the cities are located in) and see how that impacts number of rides throughout the full year. Are there more rides throughout the year for locations in warmer climates? Do city's that experience stronger seasons see higher numbers of rides in warmer times of the year. these are some suggestions of what I would want to investigate a little deeper to get a better sense of what is driving the total ride count.

