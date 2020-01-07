---
layout: post
title:  "A better representation of taxi locations after New Years Countdown 2020"
date:   2020-01-07
categories: Singapore datagovsgR Geospatial-Data GIF
---

The previous plot was not very nice as the heat maps were messy and not very interpretable. I had spend the past few days learning about sf objects in R, as I had not been previously exposed to working with geo-spatial data properly. This gif certainly seems a bit better than the previous one, though it can definitely be improved on more.

<p style="text-align: center;">
<img src="https://raw.githubusercontent.com/clintonwxy/Exploring-Data.gov.sg/master/TaxiAvailabilityUpdate/gif/animation1.gif" style="width:500px;">
</p>
<p style="text-align: center;">
<img src="https://raw.githubusercontent.com/clintonwxy/Exploring-Data.gov.sg/master/TaxiAvailabilityUpdate/images/image1.png" style="width:200px;">
</p>

While the animation is better, the inferences do appear to be the same!

Notes:

- The graphs are drawn from a single day of data, on the first day of 2020. This might not represent the daily trend of commuters, which I may look into again in a separate post.
- The data set is scrapped using the datagovsgR package, with the data from the open developer tools available under the terms of the <a href="https://data.gov.sg/open-data-licence">Singapore Open Data License</a>  version 1.0
- My workings can be found on <a href="https://htmlpreview.github.io/?https://github.com/clintonwxy/Exploring-Data.gov.sg/blob/master/TaxiAvailabilityUpdate/TaxiAvailabilityUpdate.html">here</a>!