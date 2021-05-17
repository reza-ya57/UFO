# UFO

## Overview of Project:
- In this project we colect the UFO sighting info across the world and gather all data in dynamic table by using Javascript language.

- Build a dynamic table to show the UFO sighting records with the ability of filtering the data.

- We collect all data in tidy HTML page to upload on the web and also using the table to manupulate it easily by adding the filter on different column.

## Results

We added multiple search criteria to make the webpage more attractive and interactive for users. 
users can filtered the data on datetime, city, country, state and also shape of UFO sighting.

Using the filter is realy simple just need to fill in the field of each category that you need to filtered by. 

check below for some sample of filtering:
filtered by city: "benton"
In this example we filtered the data on city named "benton". you just need to add the city name in the field and press enter.

![filter_city](https://github.com/reza-ya57/UFO/blob/main/static/images/filter_city.png)

filtered by shape: "light"
User also can filter the data based on the shape of sighting. Used light and see the below result:


![filter_shape](https://github.com/reza-ya57/UFO/blob/main/static/images/filter_shape.png)

To reset the table and delete all filtered click on "UFO Sightings" on the top right side of the page.

![filter_reset](https://github.com/reza-ya57/UFO/blob/main/static/images/reset_filter.png)

to build the table and add filter on different area, like date, city or country of sighting records. 
Users can easily filtered the data based on their interest or requirements.

Plan is using Javascript language to prepare dynamic table and show the table in HTML page.  
###	In this study we provide some valuable information for decision making process of choosing a best location for running a surf shop. We analyze the temperature for two major time of the year (June and December) and provide statistical info to give a clear vision of the weather.

In below graph you can see overall view of the temperature variance in June and Decemmber
![June Temp](https://github.com/reza-ya57/surfs_up/blob/main/Source/jun_temp_graph.png)

![Dec Temp](https://github.com/reza-ya57/surfs_up/blob/main/Source/dec_temp_graph.png)

## Results
Based on this study you can see below conclusion:
-	Minimum temperature for surfing usually is over 60s and we can see in December which is one of the coldest months of the year 75% of the days have a temperature over 69 degrees. 
-	Maximum temperature also is about 80s and over this is not very comfortable time for surfing. By looking at June temperature which should be hottest month of the year we can see 25% of the June would be higher than 77 degrees which still is a good weather for surfing.
-	By looking at statistical result we can say variation of the temperature also is about 3 to 4 degrees during the hottest and coldest month of the year in Oahu.
-	Average temperature for June and December also shows majority of the days in Oahu would be a good time for surfing. 

## Summary
In summary, Oahu could be a good place to running a surf shop and also sell Ice Cream!
There is a good chance to have lot of days with ideal temperature for surfing and enjoying the vacation in Oahu.

Also I can offer two more study as below to make sure our conclusion is more reliable:
1-	Check the precipitation for June
```
dec_prcp = []
dec_prcp = session.query(Measurement.prcp).\
    filter(extract('month',Measurement.date) == 6).all()
```
2-	Check the precipitation for December
```
dec_prcp = []
dec_prcp = session.query(Measurement.prcp).\
    filter(extract('month',Measurement.date) == 12).all()
```
