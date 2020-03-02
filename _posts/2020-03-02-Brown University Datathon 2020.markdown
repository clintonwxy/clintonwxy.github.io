---
layout: post
title:  "Brown University Datathon 2020"
date:   2020-03-02
categories: Machine Learning
---

Last week, I went over to Brown University for their annual Datathon. Several data sets were provided for data analysis, from reknowed organisatations such as Citizen's Bank, Fidelity and Dassault System. Given my recent interest in Geo-spatial data, my friend and I went with the data set provided by Citizen's Bank, which consisted of the zip9 (zipcodes) within the United States, accompanied by financial, demographical information and number of home buyers within each zip9. Our goal for the 24 hours we had, was to analyse and predict the number of home buyers for the next 3 months. Naturally, I started with looking at if there were correlations between the number of home loans, with any of the financial information for a given zip9. However, to our surprise the correlations were all exceedingly low, and hence even if we had used all the variables in a machine learning model, the results would not be accurate. Our approach then was to then analyse the data geographically, and we decided to plot the number of 
home buyers

<p style="text-align: center;">
<img src="https://raw.githubusercontent.com/clintonwxy/Exploring-Data.gov.sg/master/TaxiAvailability/images/image1.png" style="width:500px;">
</p>