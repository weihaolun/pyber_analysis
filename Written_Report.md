# PyBer Challenge with Matplotlib

## I. Overview

### Background
We have been assisting PyBer, a Python based ride sharing app company performing an exploratory analysis on their internal data. We have received two CSV files:
1.	[city_data.csv](https://github.com/weihaolun/pyber_analysis/blob/ee0658869a135c32dfe770cd3c33cbc3ab2a05fe/Resources/city_data.csv): includes 120 cities, number of drivers in each city and the type (urban, suburban, or rural) of the city.
2.	[ride_data.csv](https://github.com/weihaolun/pyber_analysis/blob/ee0658869a135c32dfe770cd3c33cbc3ab2a05fe/Resources/ride_data.csv): contains information of 2375 rides, including the city, date, fare, and the ride ID.
We conducted flowing analysis to prepare this part of project:
-	Inspect and merge DataFrames.
-	Create a bubble chart to show the average fare versus the total number of rides with bubble size based on the total number of drivers for each city type, including urban, suburban, and rural.
-	Summary statistics of measurements of central tendency (mean, median and mode) for:
    - The total number of rides for each city type.
    - The average fares for each city type.
    - The total number of drivers for each city type.
-	Created box-and-whisker plot to determine if there are any outliers for:
    - The number of rides for each city type.
    - The fares for each city type.
    - The number of drivers for each city type.
-	Created pie charts to visualize the following data for each city type:
    - The percent of total fares.
    - The percent of total rides.
    - The percent of total drivers.

### Purpose
The purpose of this challenge is to further analyze the performance among urban, suburban, and rural city types. Eventually, the goal is to:
  1.	Generate a Summary DataFrame of the ride-sharing data by city type;
  2.	Then use Pandas and Matplotlib to create a multiple-line graph that shows the total fares for each city type by week (from January to April 2019).
We will use above deliverables to analyze and summarize how the performance differs by three city types. In addition, we will provide three business advices according to the analysis at the end of this report.

## II. Results

### Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types.

![pyber_summary_df](https://user-images.githubusercontent.com/84211948/126138749-e2ad91ec-0233-496c-bdbd-a7a853ec91dc.png)

  - **Total Rides**
    Urban has a significantly number of total rides than suburban and rural. Urban has 1,625 rides, while suburban has 625 rides and rural has only 125 rides. Urban has 2.6 times more rides than suburban does, and 13 times more than rural. The reason behind this result could be that almost all households in rural area have at least one vehicle and the demand of ride sharing is very low. On the other hand, only partial residents in cities have cars and there are many travelers visiting cities, so that the demand of car rides is very high.
    
  - **Total Drivers**
    Same as Total Rides, Urban has many more drivers than the other two types. Urban has 2,405 drivers actively taking ride orders, suburban has 490 drivers and rural has only 78 drivers.  Similar to the reason above, the number of drivers is often driven by ride demands. 
When the demand is very high, more drivers would choose to enter the market to fill the gap between supply and demand.

  - **Total Fares**
    Urban has total fares of $39,854.38, the highest among three types; suburban has total fares of $19,356.33, the second highest; rural has total fares of $4,327.93, the lowest among three. Relating the results from Total Rides and Total Drivers, the differences among the three Total Fares are smaller than expected. For example, urban has 2.6 times more rides and 4.9 times more drivers than suburban, but only 2.1 times more fares than suburban, we will investigate average data in next sections to further analyze the reasons.
    
  - **Average Fare per Ride**
  This data is calculated by Total Fares / Total Rides. Rural area has the highest Average Fare per Ride of $34.62, followed by suburban’s $30.97. Urban has the lowest Average Fare per Ride of $24.53. This ranking is totally the opposite from above data. One possible reason is that the distance between destinations in rural are much longer than in cities, and suburban stands in the middle.

  - **Average Fare per Driver**
   Average Fare per Driver = Total Fares / Total Drivers. Rural again has the highest Average Fare per Driver of $55.49, followed by suburban of $39.50. Urban again has a much lower Average Fare per Driver of $16.57. One reason could be that the number of drivers in rural area is way too small, so the denominator in this function is extremely small and leads to a larger result. Another reason is to Average Fare per Ride above, the fare of rides in rural area is high due to long distance, so that the numerator is not too small at all.

  - **Total Fare by City Type**
  ![PyBer_fare_summary](https://user-images.githubusercontent.com/84211948/126138848-a2e89d66-00d3-4cd0-a53e-638f1d25fbe8.png)

  The figure above is a multiple-line graph that shows the total fares for each city type by weeks from January to April 2019. We can see from the graph that urban overall has the highest total fare, range around $1600 to $2500. Suburban’s total fare remains in the middle, with a range from around $700 to $1400. Rural area has the lowest total fare during this period, from $500 to $60. Urban and suburban both has lowest fare during the first week of January, possibly due to holiday that a large number of urban and suburban residents returned to rural hometown. All of the three types of city have peaks during the week of 2019-02-24, possibly because of a promotion.
  
## III. Summary

### Three business recommendations to the CEO for addressing any disparities among the city types.
 1. 1
 2. 2
 3. 3
