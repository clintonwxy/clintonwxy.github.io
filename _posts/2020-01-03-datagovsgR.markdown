---
layout: post
title:  "My first R package!"
date:   2020-01-03
categories: R, API
---

As part of my coursework, I created an R package which serves as an interface to the developer API tools on data.gov.sg/developers. datagovsgR is a R package used to access data-frames returned by Developer API Tools from Data.gov.sg. The package calls upon the real-time APIs, to obtain information such as taxi availability, real time weather readings, weather forecasts and PSI readings.	

Currently, the package supports almost all of the API endpoint from the website, with the exception of the IPOS applications API and Traffic images API (having difficulty downloading and displaying the image easily). The API endpoints provide a wide variety of data and I will be blogging about them soon!

Notes:

- datagovsgR can be found on my Github [page](https://github.com/clintonwxy/datagovsgR)