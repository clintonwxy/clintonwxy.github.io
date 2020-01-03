---
layout: post
title:  "Do HDBs nearer to the MRT fetch a higher Resale Price?"
date:   2019-11-07
categories: Singapore
---

I chanced upon the HDB resale flat prices data set and noticed that it was one of the few data sets which did not aggregate the data. Naturally, I went to explore the data set as it was quite extensive.

<p style="text-align: center;">
<img src="https://raw.githubusercontent.com/clintonwxy/Exploring-Data.gov.sg/master/ResaleFlatPrice/images/image1.png" style="width:500px;">
</p>

<p style="text-align: center;">
<img src="https://raw.githubusercontent.com/clintonwxy/Exploring-Data.gov.sg/master/ResaleFlatPrice/images/image2.png" style="width:500px;">
</p>

Unsurpisingly, many of the variables were found to be associated with a HDB's resale price. For example, flats which are higher fetch a greater price; as with areas that are central such as Bukit Timah and Singapore. Also, flat in Yishun have the lowest resale flat price on average compared to all other towns. 

<img src="https://raw.githubusercontent.com/clintonwxy/Exploring-Data.gov.sg/master/ResaleFlatPrice/images/image3.png">

However, the data set did not provide information on the proximity of each location to the nearest MRT, which I was interested in. Hence, I made use of Google's geocoding api and geocoded each address, which is to translate each address to a longitude and lattitude value. Then, I calculated the closest distance between each address to all MRT locations, to find the shortest distance. From the graph, we can see that HDBs closest to MRTs fetch the highest price. However, this effect is only present for flats within 1km of the nearest MRT. The difference is quite staggering, at approximately $140 000 between a flat right next to the MRT and one 1km away. Beyond 1km, the effect is not prounounced, and this could be because beyond 1km, most Singaporeans take the bus, and that at that point it does not affect the house valaution as much. There is however, a slight increase between 1km to 2km, and I think this might be because a minority of Singaporeans prefer houses that are further away from the MRT as there might be lesser traffic and/or noise. 

Finally, the resale price sharply drops at 3.6km away from the MRT. Upon closer inspection, we find that these houses are all situated at Changi Village Road in Pasir Ris, which is as ulu as a HDB can get. Furthermore, they are all low-rise buildings and are 30-40 years into their lease, which explains the low resale price.

Notes:

- Data set is limited to the years 2017 onwards, and housing prices have been rounded to the nearest 1000.
- Data set can be found on [data.gov.sg](https://data.gov.sg/dataset/resale-flat-prices) under the terms of the <a href="https://data.gov.sg/open-data-licence">Singapore Open Data License</a>  version 1.0
- My workings can be found on <a href="https://htmlpreview.github.io/?https://github.com/clintonwxy/Exploring-Data.gov.sg/blob/master/ResaleFlatPrice/ResaleFlatPrice.html">GitHub</a>
