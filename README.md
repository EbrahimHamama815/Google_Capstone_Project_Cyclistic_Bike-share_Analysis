# Google_Capstone_Project_Cyclistic_Bike-share_Analysis

   This is a guide for the google professional data analytics certificate capstone project Track A case study 1 (cyclistic).

## :page_facing_up: Task Summary

   Cyclistic, a bike sharing company, The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. 
Cyclistic’s finance analysts have concluded that annual members are much more profitable than casual riders. Although the pricing flexibility helps Cyclistic attract more customers.

Design marketing strategies aimed at converting casual riders into annual members.

## :clipboard: Approach

Using googles data analytics process 5 phases we begin with:

### :interrobang: Ask:

1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?

### :inbox_tray: Prepare:

• Download the data sets from the [divvy-tripdata](https://divvy-tripdata.s3.amazonaws.com/index.html) site. <br>
• Organize data in a single directory. <br>
• Explore the dataset to better understand what are our dimensions and measures: <br>

|  **Variable**       |  **Description**                                        |
|------------------   | --------------------------------------------------------|
| ride_id             | A unique id for each ride/trip.                         |
| rideable_type       | Type of bike per ride/trip.                             |
| started_at          | Starting Date/Time of the ride/trip                     |
| ended_at            | Ending Date/Time of the ride/trip                       |
| start_station_name  | Name of the starting station of the ride/trip           |
| start_station_id    | ID of the starting station of the ride/trip             |
| end_station_name    | Name of the ending station of the ride/trip             |
| end_station_id      | ID of the starting station of the ride/trip             |
| start_lat           | Latitude of starting station                            |
| start_lng           | Longitude of starting station                           |
| end_lat             | Latitude of ending station                              |
| end_lng             | Longitude of ending station                             |                            
| member_casual       | Type of customer per ride/trip                          |


### :arrows_counterclockwise: Process:

Due to the large data size, it wasn't possible to work with the data using excel without processing each file one at a time, so it was much better to Use **Python PANDAS** and jupyter notebooks to perform all the required data cleaning:

1.	Combine each month of data.
2.	Converting some data types to optimize memory usage.
3.	Exploring if there are aby duplicate or null ride_id.
4.	Separating geo data and ride time data into 2 different tables.
5.	Calculating ride_length, correct negative ride lengths.
6.	Categorize ride length times.
7.	Adding necessary Date/time columns for time series analysis.
8.	Importing the data to Power BI and applying some slight changes with power query to begin the analysis phase.


### :bar_chart: Analyze:

• Currently we can see that 41% are by casuals and 59% of trips are made by members, lets work on improving this percentage!

 ![image](https://github.com/user-attachments/assets/77820b50-5b2c-4b28-8f03-4ca670a46248)

 • Over the course of a full year, it seems that the most busy time of the year is around summer time (July, August, September).

 ![image](https://github.com/user-attachments/assets/a525deeb-9447-42cb-8087-77e236eca3ec)

 • Over the course of the week, it looks like most casual customers use the service on weekends, on the other hand the members use all week long.

 ![image](https://github.com/user-attachments/assets/d0285cd5-94f8-49f4-a594-fa5a709b9e03)

 • On a daily basis, it appears that both members and casual customers use the service around the end of the day, which might be due to the normal work hours.

 ![image](https://github.com/user-attachments/assets/4b170660-07bd-4872-b1c2-bb9e78c03653)

 • On average, most casual customers rides are longer than members.

 ![image](https://github.com/user-attachments/assets/7392768c-d3fe-4a35-adfd-41c6bf598f5d)

 • And the below visual show how ride/trip lengths are distributed.

 ![image](https://github.com/user-attachments/assets/c5726cc2-c183-4d1f-bb94-b338608f612f)

 • Here we can see the most user bike by both members and casual customers.

![image](https://github.com/user-attachments/assets/546af050-b976-4a3c-ba0a-ab02f1d5dc40)


### :loudspeaker: Share:

Here is a link for An interactive report on [Power BI service](https://app.powerbi.com/view?r=eyJrIjoiNjUxNjNmZDYtOTRhNi00ZDJhLWEzMzEtMWY0YmZjNzJhODIyIiwidCI6IjU5ZDRjODc4LTE4NTEtNDFkNC05ZmVmLTY5MzE2ODYyMjI5OCJ9)

![Screenshot 2025-04-19 215807](https://github.com/user-attachments/assets/efb6f451-ffe6-4dbf-8f1d-4c59c682a071)

### :pencil: Act(Take Actions):

1. In general, number of rides increase around summer time so this would be an optimal time to start advertising campaigns.
2. On average the ride length of casual customers is longer than members, so maybe provide them with time/distance based subscribtions and/or offers.
3. On a weekly basis, casual customers seems to increase in weekdends, so maybe having different types of subscriptions for example weekends only or any specific days chosen by the user would be engaging.
4. Judging by the hourly trend, most rides happen mid day (around 5:00 PM), so maybe conducting a simple survey would help better understand how both type of customers use the service wether they use it as transport method for work, or just for amusment, which will help determine what is the best place for advertisments public transports, parks, etc...























