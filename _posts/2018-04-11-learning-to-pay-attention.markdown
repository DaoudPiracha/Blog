---
layout: post
title:  Learning To Pay Attention
date:   2018-04-11 13:32:20 +0300
description: Reproducing the ICLR 2018 paper by Jetley et al.
img: attention_opt.jpg # Add image post (optional)
tags: [AI, Current]
author: Daoud# Add name author (optional)
---
This is my current project and possibly one of the most exciting ones!! My team attempts teaching something innately human, **attention**, to AI. We do this by reproducing this [paper][paper-pdf]. We also assess the ease of reproducilibility. This is part of the [ICLR 2018 Reproducibility Challenge][iclr-2018].

For a brief overview, check out these [slides][google-slides]. We used them for a 3 minute spotlight presentation. I would also like to share our current [code][colab]. Note: Please set up Google Colab to view.

 The goal of this paper is to create attention submodules for VGG, a popular image classifictaion algorithm. We will be creating these modules at 3 layers. This will allow us to have attention wieghts that highlight the background, side objects and the main objects seperately.

Attention submodules are known to increase accuracy for classification. VGG with [Attention Submodules][paper-pdf] gives a **5.23**% and **22.97**% error on CIFAR 10 and CIFAR 100 respectively. For context, [ResNet - 164][resnet], currently one of the top image classifcation models, gives errors of 6.04% and 24.4% respectively on the same datasets.


Here is an illustration of attention maps based on CIFAR 10:


![Attention Map]({{ "/assets/img/att3-dp.jpg"}})

In the meanwhile, I am also thinking of cool hacks I can make using this. Immediately though, the attention map, is a quick way to apply images effects to certain pixels with higher attention/focus. I am looking to experiment with an autoblur hack. 

Also, how about blurring the person out? I think that makes a strong statement. It might just be art!

---
Cover Photo by Romain Vignes on Unsplash

[paper-pdf]: https://openreview.net/pdf?id=HyzbhfWRW
[google-slides]: https://goo.gl/nT9eN4
[colab]:https://goo.gl/Ahv3ru
[iclr-2018]: http://www.cs.mcgill.ca/~jpineau/ICLR2018-ReproducibilityChallenge.html
[resnet]: https://arxiv.org/pdf/1603.05027.pdf
