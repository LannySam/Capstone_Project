# Cyclistic Bike-Share Usage Analysis

## Project Overview
Analyze the Cyclitics bike-share data to determine the difference how Annual Members and Casual Riders use Cyclitics bikes differently.

## The Dataset

The dataset was for quarter 1, year 2020, provided for the completion of the data analytics program [Download Here](https://divvy-tripdata.s3.amazonaws.com/index.html). The file was downloaded in CSV format and was converted to XLS format. The converted XLS format was saved in a subfolder named XLS_data.

## Tools
- Excel

## Data Preparation and Cleaning

1. Check data for errors
    -The dataset was converted into XLS format from its original CSV format.
   - The dataset was filered for blanks and null values.
   - It was sorted in ascending order by the *started_at column*
2. Transform data for effetive analysis
     - The *started_at* and *ended_at* columns were formatted into *dd:mm:yyyy hh:mm:ss* format
     - *Ride_length* column was calculated by *substracting* the started_at column values from the ended_at column values. This determined the trip duration for each bike ride.
     - *Day_of_week* column shows the day in the week the ride started. This was calculated by using the formular below. Note that 1 denotes Sunday
       ```excel
       =weekday(C2,1)
       ```
## Exploratory Data Analysis
1. Statistical Analysis
   - Average trip duration was calculated, using the *Average function*. Where (E:E) is the data range.
      ```excel
      =average(E:E)
      ```
   - The highest trip duration was determined using the *Max function* Where (E:E) is the data range.
     ```excel
     =max(E:E)
     ```
   - The *Mode Function* was used to determine the day with the highest number of trips. Where (F:F) is the data range.
     ```excel
     =mode(F:F)
2. Pivot Tables

Four pivots tables was plotted to analyze trends and patterns in our data.
- Total Rides Per Subscription type:  shows the percentage of total rides for each subscription type.
- Avg ride length per subscription type: shows the 
- Avg ride length per weekday.
- Total rides per weekdays for all subscription type

## Key Findings

1. Basic Statistics
- The average ride length is 00:22:07
- The maximum ride length is 15:30:24
- The most frequent day of the week for a ride is 3 which denotes Tuesday
2. Pivot Table
- Total rides per subscription type: Casual riders contributed 11% with 48,363 rides while Members accounted for the remaining 89% with a total number of 368,407.
- Avg ride length per subscription type: Casual riders ride the farthest distance as calculated by the average ride length of 01:36:01 (hh:mm:ss format) while the average ride length of members is 00:12:41 (hh:mm:ss format).
- Sunday (00:15:49) and Saturday (00:15:30) are the highest average ride length for annual membership.
- Thursday and Friday have the highest value for average ride length for the casual riders with 02:06:40 and 01:58:46 respectively.


     
