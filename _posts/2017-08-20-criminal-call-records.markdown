---
layout: post
title:  What's weird about Criminal Calls
date:   2017-08-20 13:32:20 +0300
description: An overview of my experience analyzing crime records in Pakistan
img: crime2.jpg # Add image post (optional)
tags: [Data Science, Crime, Behaviour, Python]
author: Daoud # Add name author (optional)
---
Last summer, I investigated criminal behaviour in Pakistan using call records and official data. This was interesting since we had to deal with (very) noisy data. We were able to observe some interesting patterns criminals tended to follow:

- Main suspects tended to switch SIMs upto 2 to 3 times in the 72 hours before the crime.
- Analyzing the network, we found certain interesting individuals. Apparently dstinct individual were making the exact same calls!

 These people had different phone IDs and SIMs but they made calls to the same people and at the same time. These results were almost instantly visible using simple clustering techniques. This allowed us to reduce the edges and nodes in the suspect call graph significantly. It also increase the likelihood wieghts on certain individuals.

Unfortunately, with the nature of a developing country we couldnt prove observations to high levels of statistical significance. Nonetheless, the inisghts remain critical and may be useful to better utilization of police reosurces and faster suspect isolation in the future.

I hope to redo this study once we have more data to find significant evidence for the many hypotheses we developed investigating the issue. Here's to a safer world and a safer Pakistan. :)