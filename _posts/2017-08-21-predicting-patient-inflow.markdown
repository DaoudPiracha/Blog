---
layout: post
title: Predicting Patient Inflow
date: 2017-08-21 13:32:20 +0300
description: This project was trying to optimise hospital staffing problem by predicting patient demand

img: healthcare2.jpg # Add image post (optional)
tags: [AI, Time Series, Internship]
author: Daoud # Add name author (optional)
---
I worked on this time series problem while interning with the wonderful team over at [Addo AI][addo-home]. Over 6 weeks we analysed the data and tried a number of modelling techniques.

I was involved heavily in preprocessing. Splitting trend and seasonality, shuffling data and monitoring lags made substantial effects on output. We used statistical modelling, Bayesian and M-ARIMA, initially. I implemented my own model, using LSTM and RNNs, which was comparable. For deployment, we used an ensemble model based on ward specific meta-learning.

Deployed, this model impacts 1.3 million patients annually and so has to be one of the most fulfilling AI projects I have worked on. 

[addo-home]: https://addo.ai/

___
Cover photo by Pina Messina on Unsplash