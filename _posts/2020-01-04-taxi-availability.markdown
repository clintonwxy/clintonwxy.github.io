---
layout: post
title:  "Taxi Availability after New Year's Countdown 2020"
date:   2020-01-04
categories: Singapore datagovsgR Geospatial-Data
---

Making use of the Rpackage I just created, the taxi_availability function allows us to query taxi locations to the minute. I was interested in finding out how the taxi availability changes throughout the day after the new year countdown. For this post, I queried the taxi availability for the entire day of 2020-01-01 in 10 minute intervals. Subsequently, it was cleaned and several graphs were plotted.

<p style="text-align: center;">
<img src="https://raw.githubusercontent.com/clintonwxy/Exploring-Data.gov.sg/master/TaxiAvailability/images/image1.png" style="width:500px;">
</p>

From the graph, we can see that there appears to be a huge peak at midnight, and then a sharp drop over the next hour. This might be because of people heading home after the new year countdown. Generally, the taxi availability increases over the day, with the lowest around early morning and the rush hour, and the highest at midnight. Also, the sharp drop in availability might be due to taxi bookings during the early morning rush hour, which then eases later.

Then, I made use of the ggmap package to obtain a map of Singapore, so that I could plot taxi locations. Geom_density_2d was preferred over geom_point as it would cause the points to be too concentrated (and that using an alpha of 0.05 would not help either). gganimate was then used to animate the transition.

<p style="text-align: center;">
<img src="https://raw.githubusercontent.com/clintonwxy/Exploring-Data.gov.sg/master/TaxiAvailability/images/image2.gif" style="width:500px;">
</p>
<p style="text-align: center;">
<img src="https://raw.githubusercontent.com/clintonwxy/Exploring-Data.gov.sg/master/TaxiAvailability/images/image3.gif" style="width:500px;">
</p>

From the 2 gifs, we can see clearly how the taxi locations change with time. Taxis start out initially not in any one general spot at midnight, where it decreases until the early morning. Then, we start to see a crowd of taxis around the south and east of Singapore, presumably where town and the airport areas are. This trend then continutes to persist throughout the day. From this, we can somewhat suggest that the greatest amount of taxis can be found in these two areas generally throughout the day. Finally, it would appear that taxis tend to prefer to not be in the West and North, relative to the Central area.

Notes:

- The graphs are drawn from a single day of data, on the first day of 2020. This might not represent the daily trend of commuters, which I may look into again in a separate post.
- The data set is scrapped using the datagovsgR package, with the data from the open developer tools available under the terms of the <a href="https://data.gov.sg/open-data-licence">Singapore Open Data License</a>  version 1.0
- My workings can be found on <a href="https://htmlpreview.github.io/?https://github.com/clintonwxy/Exploring-Data.gov.sg/blob/master/TaxiAvailability/TaxiAvailability.html">here</a>!