---
layout: post
title:  AirBnB Price Predictor
date:   2017-08-25 13:32:20 +0300
description: Given an AirBnB listing this model generates an estimate price
img: airbnb2_opt.jpg # Add image post (optional)
tags: [AI, Data Science, Python]
author: Daoud # Add name author (optional)
---
This project means a lot since it won me my first hackathon prize.

This was done for the DataDive 2017 Hackathon. We ended up as one of the winnings teams. Here is a [link][devpost] to our submission on Devpost. Also feel free to check out the [code][github] on Github!! 

I made a deep learning algorithm that provides a suggested price for potential Airbnb listings in Montreal based on historic prices and Local Logic API data. Local Logic gave ratings for  ratings for amenties, restaurants etc and so was helpful in finding additional location specific features. 

Overall we were accurate to within $10 on our testing dataset.

Fun Fact: To actually use Local Logic, we had issues with their API call. We ended up using their widget and scraping the HTML from there for each location. This calls for some serious hacker cred!!


Cover Photo by Adrian Schwarz on Unsplash

[devpost]: https://devpost.com/software/airbnb-price-generator
[github]: https://github.com/DaoudPiracha/local-airbnb-pricer
[prediction]: https://github.com/DaoudPiracha/local-airbnb-pricer/blob/google-maps/images/screenshot3.png

