---
layout: post
title: Multiple Object Image Classification
date: 2017-08-26 13:32:20 +0300
description: A Classifier to find the largest digit in a modified version of MNIST that contains multiple digits.
img: multi-classifier.jpg # Add image post (optional)
tags: [Python, AI]
author: Daoud # Add name author (optional)
---

I made this with Nadeem Ward as part of [COMP 551: Applied Machine Learning][551-home], a (very cool) course I'm taking.

We were tasked to find the largest digit in an image that may contain upto 3 rescaled digits from MNIST. Feel free to read up on the [problem statement][ass4-problem] for more details.

One of the reasons I loved this [project][multi-gh] was the freedom it allowed. After the first submission, we were able to and encourage to anything and everthing under the sun to increase accuracy. By nature of a Kaggle competition we had to be competitive.

## Preprocessing

As in most Kaggle competition, preprocessing was key. We were quick to notice that after rescaling, the MNIST digits were now significanly darker. We applied a threshold and bounding box to reduce the problem significantly, this sadly cost us 3% of the data, it was only so accurate. We also choose to ratio by pixel counts, taking advantage of the geometry and area of each number. We couldn't possibly let a small, fat 8 overtake our larger but skinny 1, now could we!

## Methods

Some of the things we tried:

- CNN's (several architectures to adjust for modifications)
- Transfer Learning
- CNN + SVM
- Ensemble Models

#### CNNs
We modified the vanilla architecture on models that worked on MNIST. We noticed digits were thicker and, as a result of rescaling, edges were blurry and larger. Hence we played with kernel size to significantly boost results.

#### CNN + SVM
We tried using CNNs for feature generation. We simply removed the last layer and fed to an SVM instead. We got interesting results here as well.

#### Transfer Learning
We trained on MNIST and froze lower level feature generating layers and retrained on our data. We trued a number of approaches, choosing which layers to freeze. We got the best results with the first layer unfrozen and the rest of the convoltional layers frozen. This gave comparable performance. We believe it mostly benefitted the ensemble approach.

#### Ensemble 

As is practice, we too implemented majority voting. This gave us a significant boost and was a solid win.

## Acknowledgments

A huge shoutout to my teammate **Nadeem Ward**. He was a great person to work with and taught me a lot. All the best Nadeem.





Check the [code][multi-gh] out on Github.

Alternatively, read our [report][report-pdf], for more details. It's all formal if you're into that.

[report-pdf]: https://drive.google.com/file/d/1TnLDsUWK4jxWH44Kvv7pd39TBNhc_D6f/view?usp=sharing
[multi-gh]: https://github.com/DaoudPiracha/Multiple-Object-Classification
[551-home]: http://sarathchandar.in/teaching/2018/winter/comp551-001/
[ass4-problem]: http://cs.mcgill.ca/~rlowe1/comp551/Comp_551_Project_4.pdf

___
Cover Photo by [Nick Hillier](https://unsplash.com/@nhillier) on Unsplash
