
## About New York Citi Bike
Citi Bike is New York City’s bike share system, and the largest in the nation. Citi Bike launched in May 2013 and has become an essential part of our transportation network. It's fun, efficient and affordable – not to mention healthy and good for the environment.<br>

Citi Bike, like other bike share systems, consists of a fleet of specially designed, sturdy and durable bikes that are locked into a network of docking stations throughout the city. The bikes can be unlocked from one station and returned to any other station in the system, making them ideal for one-way trips. People use bike share to commute to work or school, run errands, get to appointments or social engagements, and more.<br>

Citi Bike is available for use 24 hours/day, 7 days/week, 365 days/year, and riders have access to thousands of bikes at hundreds of stations across Manhattan, Brooklyn, Queens and Jersey City.<br>

Citi bike is providing data about all the rides from its birth. Lets dive into it and explore it.

> __Note:__ Each plot opens up in a new tab. Every plot has a tool box using which you can interact with the plot by zooming in, dragging or hover over the data points to get the data at a point.

## Collective distance
Click on the image to open interactive plot
[![image](https://user-images.githubusercontent.com/30205620/29245013-47f16d66-7f99-11e7-8727-612a112a030d.png)](https://htmlpreview.github.io/?https://github.com/naveenrc/naveenrc.github.io/blob/master/citibikenyc/total_distance.html)<br>
These are the estimated numbers, assuming that the riders reach their destination as suggested by google`s shortest route.<br>
Just think about __676 million miles__, Yes this is the estimated minimum total distance traveled so far by all the riders.<br>

## Members vs non-Members
Click on the image to open interactive plot
[![image](https://user-images.githubusercontent.com/30205620/29245022-6e178a5c-7f99-11e7-9ec3-18170e067747.png)](https://htmlpreview.github.io/?https://github.com/naveenrc/naveenrc.github.io/blob/master/citibikenyc/user_plot.html)<br>
From this it is evident that users are willing to subscribe. We can make following assertions:<br>
1. Users are mostly based in New York city and use citi bike services very frequently. Taking advantage of the unlimited 45 minutes rides.
2. Reducing pay per ride price could improve the no-member involvement too.
3. The period from July 2016 till October saw a huge increase, which could be because citi bike expanded its services to Jersey city, increased number of bike stations and bikes in NYC as well.

## Involvement by gender
Click on the image to open interactive plot
[![image](https://user-images.githubusercontent.com/30205620/29245025-8ea8a422-7f99-11e7-8ea6-298aa5f99d46.png)](https://htmlpreview.github.io/?https://github.com/naveenrc/naveenrc.github.io/blob/master/citibikenyc/gender_plot.html)<br>
Male are ahead of female by about an average of __7000 rides a day__

## Involvement by age
Click on the image to open interactive plot
[![image](https://user-images.githubusercontent.com/30205620/29245039-f2bfb78e-7f99-11e7-9ba6-af51bcbda522.png)](https://htmlpreview.github.io/?https://github.com/naveenrc/naveenrc.github.io/blob/master/citibikenyc/age_plot.html)<br>
These figures are only based on members, because non-members details are not provided.<br>
People around __35 years__ are leading the race with __more than 1.4 million rides__. Contrast to teens less than 200k rides.

## Is it raining? So what
Click on the image to open interactive plot
[![image](https://user-images.githubusercontent.com/30205620/29245047-20cfc43e-7f9a-11e7-9339-d9aa48240cba.png)](https://htmlpreview.github.io/?https://github.com/naveenrc/naveenrc.github.io/blob/master/citibikenyc/weather_rides.html)<br>
Although no rain is definitely a good increase in number of rides, 2 inches of rain also saw 30k rides. So, these new yorkers like rain? I think so.<br>

[![image](https://user-images.githubusercontent.com/30205620/29245059-66fed396-7f9a-11e7-9e3b-30b04c37b40a.png)](https://htmlpreview.github.io/?https://github.com/naveenrc/naveenrc.github.io/blob/master/citibikenyc/weather_rides.html)<br>
Extreme temperature is effecting the number of rides<br>

[![image](https://user-images.githubusercontent.com/30205620/29245053-3b772db8-7f9a-11e7-8ff1-e117f0045309.png)](https://htmlpreview.github.io/?https://github.com/naveenrc/naveenrc.github.io/blob/master/citibikenyc/weather_rides.html)<br>
Snowfall is having similar effect to that of rain.

## Popular bike stations
Click on the image to open interactive plot
[![image](https://user-images.githubusercontent.com/30205620/29245066-9a20eaac-7f9a-11e7-910f-0f236be5d7d2.png)](https://htmlpreview.github.io/?https://github.com/naveenrc/naveenrc.github.io/blob/master/citibikenyc/plot_popular.html)<br>
Midtown bike stations are having the most number of transactions (bicycle in/out) in March 2017.<br>

## Station to station transport
Click on the image to open interactive plot
[![image](https://user-images.githubusercontent.com/30205620/29245070-c341ed5a-7f9a-11e7-9a13-dc44ccdafb9b.png)](https://htmlpreview.github.io/?https://github.com/naveenrc/naveenrc.github.io/blob/master/citibikenyc/transport_plot.html)<br>

Citi bike transports bikes to stations where there are less number of bikes. So, we can see Dec 2015 to Jan 2016 is having massive increase. It is just because citi bike installed new bikes and stations in NYC and Jersey city regions, repairs at some stations or some group events.<br>
I have emailed a member of citi bike for exact reason of this pattern.<br>
Overall transportation is gradually decreasing, which is good for citi bike authorities.

## Google vs citi bike users
Difference between average citi bike riders speed and google estimate is __2.5 miles/hr__. This could be because riders usually stop to look around the places, or because of traffic.

The source code for this analysis can be found on my [Github](https://github.com/naveenrc/new_york_citibikes)
