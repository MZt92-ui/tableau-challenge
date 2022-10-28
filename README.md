
# Project: Citi Bike Program Pre-Covid-19 Performance
**The project aimed to find patterns in how Citi Bike Program was utilized before Covid-19 specifically in the year of 2019. The project was prepared for the Monash Data Analytics Bootcamp study, with the purpose to apply python, tableau, and statistical concepts for real-life datasets.**

## Citi Bike Program & Dataset
Citi Bike is a privately owned public bicycle sharing system serving the boroughs of New York City.
<br>The Citi Bike operator has made monthly riding records available to the public in csv formats, which is accessible in [Link](https://ride.citibikenyc.com/system-data). The information includes demographic entries, start & tilend stations, start & end time and etc.  

## Project Scope & Procedure
This project was to answer below questions:
1. Firstly, to understand overall performance of the program in year 2019, including total riding counts, riding time and etc.
2. Then to understand users' demographics
3. Lastly to reveal some users' behaviours and understand how the program was utilised

The key procedures are:
* **Data extraction & transformation:**
<br>There are some missing records related to station information; I left them blank without deletion and replacement as they are not wrong records, deletion would impact total counts; also there is no other information to support replacements of these non-numerical values. Then extract information of interests and combine 12 tables into one for further analysis. 
* **Visualisation & analysis using python**
* **Create a dashboard in tableau**

## Dashboard (Tableau)
Below is an screenshot of what was created in tableau:
![Dashboard](https://github.com/MZt92-ui/tableau-challenge/blob/main/analysis/dashboard.JPG)

## Key Analysis (Python)

### Analysis 1: Monthly Total Trips
<img align="left" width="400" height="250" src="https://github.com/MZt92-ui/tableau-challenge/blob/main/analysis/1.jpg">
<br><br>Monthly trips from customer & subscriber follow similar pattern, with an upward trend till September and then drop to the level of beginning of the year.

### <br><br><br><br><br>Analysis 2: Top Age Groups
<img align="left" width="400" height="280" src="https://github.com/MZt92-ui/tableau-challenge/blob/main/analysis/2.jpg">
<br>

* For subscriber usertype, age between 30 and 40 make the largest user group; while for customer, it is 50-60 age group.
* For age group classified as "Other", it includes recorded ages over 80, which is likely untrue input from users, e.g. there are around 8,000 records with age over 120yrs old.

### <br><br><br><br><br>Analysis 3: Total Trips By Gender
<img align="left" width="400" height="250" src="https://github.com/MZt92-ui/tableau-challenge/blob/main/analysis/3.jpg">
<br>The male is the primary group utilising the program in year 2019, and most of them (92.5%) were adopting membership.

### <br><br><br><br><br><br><br>Analysis 4: Peak Hours In A Day
<img align="left" width="400" height="250" src="https://github.com/MZt92-ui/tableau-challenge/blob/main/analysis/4.jpg">
<br>

* For all age groups, trips are peaked in 8am, 5pm & 6pm, which implies the primary application of the program is for the sake of commute.
* However, usertype of customer shows different behaviours, with growing activity since 6am and maintained its peak during 2pm-5pm. 

### <br><br><br><br>Analysis 5: Trip Duration Analysis
<img align="left" width="450" height="250" src="https://github.com/MZt92-ui/tableau-challenge/blob/main/analysis/5.jpg">
<br>

The trip duration is extremely right skewed, with median value of 10.25min and over 900K outliers. Based on the map of stations recorded duration over 1day, it shows that:
* these stations are scattered in the serving area;
* the frequency of extremely long trip is considered low, i.e. circle sizes of stations with darker colors are below 20.
