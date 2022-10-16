
# Project: Citi Bike Program Pre-Covid-19 Performance Analysis
**The project was aimed to find patterns about how Citi Bikes Program was utilised before Covid-19 specifically in year 2019. The project was prepared for Monash Data Analytics Bootcamp study, with the purpose to apply python, tableau and statistical concepts for real-life datasets.**

## Citi Bike Program & Dataset
Citi Bike is a privately owned public bicycle sharing system serving the boroughs of New York City.
<br>The Citi Bike operator has made monthly riding records availble to the public in csv formats, which is accessible in [Link](https://ride.citibikenyc.com/system-data). The information includes demographic entries, start & end stations, start & end time and etc.  

## Project Scope & Procedure
This project was to answer below questions:
1. Firstly, to understand overall performance of the program in year 2019, including total riding counts, riding time and etc.
2. Then to understand users' demographics
3. Lastly to reveal some users' behaviours and understand how the program was utilised

The key procedures are:
* **Data extraction & transformation:**
<br>There are some missing records related to station information; I left them blank without deletion and replacement as they are not wrong records, deletion would impact total counts; also there is no other information to support replacements of these non-numerical values. Then extract information of interets and combine 12 tables into one for further analysis. 
* **Visualisation & analysis using python**
* **Create a dashboard in tableau**

## Dashboard
![Dashboard](https://github.com/MZt92-ui/tableau-challenge/blob/main/analysis/dashboard.jpg)
## Key Analysis
### Analysis 1: Monthly Total Trips
Monthly trips from customer & subscriber follow similar pattern, with an upward trend til September and then drop to the level of beginning of the year.

![Monly Total Trips](https://github.com/MZt92-ui/tableau-challenge/blob/main/analysis/1.jpg)
### Analysis 2: Top Age Groups
* For subscriber usertype, age between 30 and 40 make the largest user group; while for customer, it is 50-60 age group.
* For age group classified as "Other", it includes recorded ages over 80, which is likely untrue input from users, e.g. there are around 8,000 records with age over 120yrs old.
![Age group](https://github.com/MZt92-ui/tableau-challenge/blob/main/analysis/2.jpg)
### Analysis 3: Total Trips By Gender
The male is the primary group utillising the program in year 2019, and most of them (92.5%) were adopting membership.
![Gender](https://github.com/MZt92-ui/tableau-challenge/blob/main/analysis/3.jpg)
### Analysis 4: Peak Hours In A Day
* For all age groups, trips are peaked in 8am, 5pm & 6pm, which implies the primary application of the program is for the sake of commute.
* However, customer type show different behaviours, with growing activity since 6am and maintained its peak during 2pm-7pm. 
![Gender](https://github.com/MZt92-ui/tableau-challenge/blob/main/analysis/4.jpg)
### Analysis 5: Trip Duration Analysis
The trip duration is extremely right skewed, with median value of 10.25min and over 900K outliers. Based on the map of stations recorded duration over 1day, it shows that:
* starting stations are scaterred in the serving area;
* the frequency of extremely long trip durations is considered low, i.e. circle sizes of stations with darker colors are below 20.
![Trip](https://github.com/MZt92-ui/tableau-challenge/blob/main/analysis/5.jpg)
