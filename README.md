# Cyclistic Bike-Share Usage Analysis

## Project Overview
Analyze the Cyclitics bike-sharing data to determine the difference how Annual Members and Casual Riders use the program differently in quarter 1 of the fiscal year.

## Data Source

The data was for year 2020, provided for the completion of the data analytics program [Download Here](https://divvy-tripdata.s3.amazonaws.com/index.html). The file was downloaded in CSV format and was converted to XLS format. The converted XLS format was saved in a subfolder named XLS_data.

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
   - The highest trip duration was determing using the *Max function* Where (E:E) is the data range.
     ```excel
     =max(E:E)
     ```
   - The *Mode Function* was used to determine the day with the highest number of trips. Where (F:F) is the data range.
     ```excel
     =mode(F:F)
2. Pivot Tables

Four pivots tables was plotted to analyze trnds and patterns in our data. They are follow:
- Total Rides Per Subscription type:  shows the percentage of total rides for each subscription type.
- Avg ride length per subscription type: shows the 
- Avg ride length per weekday.
- Total rides per weekdays for all subscription type

     
