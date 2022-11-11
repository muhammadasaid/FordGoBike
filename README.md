# FordGoBike
# Ford Go Bike Data Exploration

## Dataset

The data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area, the dataset contains the details of 183412 trips with 16 attributes and most variables are numeric in nature, but the variables start_station_name, end_station_name, user_type and member_gender are qualitative nominal variables. Feature engineering was done on duration_sec column to create more columns (duration_minute, start_date, start_hourofday, start_dayofweek, start_month). Some outliers like age (greater than 80) and trips (greater than 60 minutes) were removed.
The dataset can be found in the
following link [here](https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv)


## Summary of Findings

In the exploration, 
1. Males represent 74.6 percent of users, whereas Females represents 23.3 percent, the remainder is others with 2.1 percent
2. from the distribution of duraction we can see that more than 96.56 percent of trips were less than 30 minutes. We can also notice that only 0.79 percent of trips are of duration more than 1 hour. These might be considered as outliers that needs to be removed before going further in the bivariate analysis.
3. Also we can see that peak hours are those from 7 - 9 am and from 4 - 7 pm. This might be related to the time when employees and students go to and leave work or school. This is was also consistent with the distribution of trips over weekdays, where work days have the most demand for trips.
4. The distribution follows a typical age distribution (Skewed to the right). Those aged 20 - 45 are the most demanding segment for rides as they are the most active population either in work or school.
5. Customers represent 9.47 percent of users, whereas subscribers represents 90.53 percent, which shows subscribers get more trip maybe because of their subscriptions.
6. There are way more subscribers than customers.
7. Subscribers usage seem to be very consistent, their usage is intended for daily routine such as work or study.
8. Subscribers usage reaches its highest levels during work days rush hour.
9. On the other hand Customers tend to use bikes for fun, their usage is concentrated during weekends at midnights and middays.

Outside of the main variables of interest i found that the distribution of the duration was surprising, 96.6 percent of trips were 30 mintes or less.
I also created new features out of the time variable (duration_minute, start_date, start_hourofday, start_outofweek, start_month)

## Key Insights for Presentation

For the presentation, I focus on member information (age, gender and user_type) and trip duration in minutes. I start by looking at the relationship between trip duration and age, followed by the distribution of trip duration by Gender, then plot the distribution of trip duration by user type.

Afterwards, I looked at the distribution of gender and duration for each user type using a catplot and a color palettes for each member gender and lastly the distribution of Age and trip duration for each user type using a scatter plot and a color marker for each user_type.
