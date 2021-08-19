# Introduction

Ford GoBike System Data 
is a dataset includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area And I'm going to explore this data to get some observations and answers of some questions.

# Summary of the analysis steps

(A) Reading the .csv file of the Ford GoBike System dataset.

(B) Data Wrangling (Assessment & Cleaning):

- Checked the number of rows and columns in the dataset.
- Checked if there is a miising values.
- Checked the number of misssing values in each column and As the number of missing values cells is not large I choose to delete this rows from the data.
- Checked the data types of each variable and found some data types need to be converted.
- So I converted the (start_time & end_time) to datatime data type and (start_station_id & end_station_id & member_birth_year) to integer data type.
- Checked the number of unique values in each column and it sounds sense.
- Checked if there is a duplicated rows and there was no duplicated rows.
- Checked the discription of the dataset.
- In the description I found that min of member birth year is 1878 which is not logical and it is only with one row so I droped this row to not affect negatively on the accuracy of data explorin.

(C) Data Exploration:

- Used a pie chart for the categorical variable (member_gender) to know which gender is more of total members.
- Used a bar chart for the categorical variable (user_type) to know which user type is more of total members.
- Used a histogram for the quantitative variable (member_birth_year) to know what is the age of the most members.
- Create if Function to sort the trips durations into categories and used bar chart to know what is the most duration of the trips.
- splited the Date and Time of start time column into columns to be able to get some insights from it.
- Used clustered Bar Chart to check the relationship between the days and members gender.
- Used clustered Bar Chart to check the relationship between rush hour and user types.
- Used boxplot to check the relationship between gender and trip duration.
- Sort the top ten start stations and used a stacked bar chart to check if the number of males still much more than females in all start station.
- Used pointplot to check the relationship between user type and trip duration durring the month.
- Created a new column of the members ages to be easier to use than the birth year and used heatmap with .corr function to create a correlation matrix For the mentioned three numeric variables.

# Conclusion

- The males members are much more than females and other gender.
- The most of users are subscribers not customers.
- The hight age range of the members is whos birth year from 1985 to 1995.
- The most trips durations are less than 10 minutes, So it uesd for the very short trips.
- The most common start station is (Market St at 10th St) and the most common end station is (San Francisco Caltrain Station 2  (Townsend St at 4th St))
- The dataset contain only the february month of 2019.
- The high or low traffic days are the same for males and females.
- The rush hours are the same for subscribers & customers and they are 8/9 am and 5/6 pm.
- Females and other gender have a longer trip duration than males.
- The number of males is more than the females and other gender in all top ten start stations.
- Customers have a longer trip duration than subscribers during the month.
- There is no relatively high correlation between the variables / And there is a negative correlation between the start hour and members age.

# Key insights:

The number of males members is much more than females but females spend a longer duration of the trips. As for the users type, Subscribers members are much more customers, also customers spend a longer duration of the trips. In general the most trip durations are for less than 10 minutes and the most rush hours for trips are 8/9 am to 5/6pm.
