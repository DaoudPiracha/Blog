---
layout: post
title:  Generatively Adversarial ChatBots
date:   2017-08-19 13:32:20 +0300
description: Developing more human conversational AI
img: conversation_opt.jpg # Add image post (optional)
tags: [AI, Research, Current]
author: # Add name author (optional)
---
Motivated by the NIPS ConvAI Challenge, this project started at the ImplementAI Hackathon. Fortunately it lived past just a hackathon. This is credited to help and feedback recieved from the Adversarial Group at MILA and the Dialogue Group at RLL, McGill.

The idea is to use an adversarial approach to teach dialogue. My team was largely inspired by two papers:

- Adversarial Learning for Neural Dialogue Generation(Li et al. 2017) [[arvix]][Neural-dialogue]
- Generatively Adversarial Networks(Goodfellow et al. 2014) [[arvix]][GANs]

To train conversational AI to become more human, i.e have a better score on the Turing Test we propose:

- a Generator model that produces dialogue
- a Discriminator model that tries to simulate a Turing Test

We are training the generator as an ensemble of sequence models trained on different contexts. We are trying to train a ranker to help choose the model case to case using a Reinforcement Learning approach. For the discriminator, we are essentially training a binary classifier to categorize Human/Non Human Responses. As both get better while training we hope to achieve convergence to more intelligent and more context aware conversational AI.

Currently, we are trying to train several conversational models based on reddit data. We pick two comments from one subreddit e.g sports related (NFL etc.) and one comment from an unrelated subreddit e.g food related. The unrelated comment simulates a non Human Response as it is not context aware and less natural.

This is currently ongoing. I feel this is an exciting way to approach this problem. I would like to see if it leads to more interesting problems.

Here is a link to our [hackathon submission][devpost], and to the [pitch][slides] we gave. Both are a little predated, however, we do hope to update with exciting new progress soon.





[Neural-dialogue]: https://arxiv.org/abs/1701.06547
[GANs]: https://arxiv.org/abs/1406.2661
[devpost]: https://devpost.com/software/generative-adversarial-bots
[slides]: https://docs.google.com/presentation/d/1VbMb1zIpp8rhWiEq1d2tENOtkRslLD855vT8CAPw8eU/edit?usp=sharing

