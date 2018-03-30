---
layout: post
title:  AirBnB Price Predictor
date:   2017-08-22 13:32:20 +0300
description: Given an AirBnB listing this model generates an estimate price
img: airbnb.jpg # Add image post (optional)
tags: [AI, Data Science, Python]
author: Daoud # Add name author (optional)
---
We made a deep learning algorithm that provides a suggested price for potential Airbnb listings in Montreal based on historic prices and Local Logic API data. We used Local Logic to get location specific features like ratings for amenties, restaurants etc. 

Overall we were accurate to within $10 on our testing dataset.

This was done for the DataDive 2017 Hackathon. We ended up as one of the winnings teams. Here is a [link][devpost] to our submission on Devpost. Also feel free to check out the [code][github] on Github!! 

Fun Fact: To actually use Local Logic, we had issues with their API call. We ended up calling their widget and scraping the HTML from there for each location. Calls for some serious hacker cred!!


Cover Photo by Adrian Schwarz on Unsplash

[devpost]: https://devpost.com/software/airbnb-price-generator
[github]: https://github.com/DaoudPiracha/local-airbnb-pricer
[prediction]: https://github.com/DaoudPiracha/local-airbnb-pricer/blob/google-maps/images/screenshot3.png

