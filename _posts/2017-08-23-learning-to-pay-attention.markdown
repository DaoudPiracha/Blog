---
layout: post
title:  Learning To Pay Attention
date:   2017-08-23 13:32:20 +0300
description: Reproducing the ICLR 2018 paper by Jetley et al.
img: attention.jpg # Add image post (optional)
tags: [AI, Current]
author: Daoud# Add name author (optional)
---
This is my current project and possibly one of the most exciting ones!! Teaching something so human, attention, is an interesting problem. The goal is to create attention submodules for VGG, a popular image classifictaion algorithm. We will be creating these modules at 3 layers. This will allow us to have attention wieghts for the background, side objects and the main objects seperately.

This is known to increase accuracy for classification. My team's goal here is to assess the reproducilibility of this [paper][paper-pdf]. We hope to have code up and a report on the project soon.

In the meanwhile, I am thinking of cool hacks I can make using this. Immediately though, the spatial map is a quick way to apply images effects to certain pixels with higher attention/focus. I am looking to experiment with an background autoblur hack. 

Also, how about blurring the person out. I think that makes a strong statement. It might just be art!


Cover Photo by Romain Vignes on Unsplash

[paper-pdf]: https://openreview.net/pdf?id=HyzbhfWRW

