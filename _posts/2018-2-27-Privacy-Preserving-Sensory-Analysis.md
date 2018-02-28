---
layout: post
title: Privacy-Preserving time-Series Data Analysis
---

An increasing number of sensors on mobile, Internet of things (IoT), and wearable devices generate time-series measurements of physical activities. Though access to the sensory data is critical to the success of many beneficial applications such as health monitoring or activity recognition, a wide range of potentially sensitive information about the individuals can also be discovered through access to sensory data and this cannot easily be protected using traditional privacy approaches.

Specifically, there are two ways of drawing sensitive inferences from time-series of sensory data :
(1) *Temporal Inferences*, that means each section of time-series can be assigned to a specific inference, sensitive or non-sensitive (including  desired information that users gain utility from sharing them).
(2) *Concurrent Inferences*, that means information available in each section of time-series can be used to make both sensitive and non-sensitive inferences.


| <img src="https://raw.githubusercontent.com/mmalekzadeh/motion-sense/master/materials/temporal_inf.png" class="img-responsive"> | <img src="https://raw.githubusercontent.com/mmalekzadeh/motion-sense/master/materials/concurrent_inf.png" class="img-responsive"> |
|:---:|:---:|
| Temporal Inferences | Concurrent Inferences |

Recently, we have been working on enabling privacy-preserving techniques for time-series data. This is an area where solutions are slightly more challenging than traditional methods used in databases or spatial data like Differential-Privacy or k-anonymity. Through the works of PhD candidate [Mohammad Malekzadeh]( https://mmalekzadeh.github.io/){:target="_blank"} We have been investigating new method to address the challenges in this space.

1) Replacement AutoEncoder: A Privacy-Preserving Algorithm for Sensory Data Analysis
Paper: [https://arxiv.org/abs/1710.06564]( https://arxiv.org/abs/1710.06564)

In this paper, we propose a privacy-preserving sensing framework for managing access to time-series data in order to protecting *temporal inferences*. We introduce *Replacement AutoEncoder*(RAE), a novel algorithm which learns how to transform discriminative features of data that correspond to sensitive inferences,  into some features that have been more observed in non-sensitive inferences, to protect users' privacy. This efficiency is achieved by defining a user-customized objective function for deep autoencoders.
We also used [GAN]( https://en.wikipedia.org/wiki/Generative_adversarial_network){:target="_blank"}s to see if an attacker can detect when non-sensitive activity inferred from data is actually a replacement of a sensitive one, not a real non-sensitive activity. We show that this will only be possible if a GAN is trained on the users' original, unmodified data.

| <img src="https://github.com/mmalekzadeh/motion-sense/blob/master/materials/rae.png" class="img-responsive"> |
|:---:|
| Replacement AutoEncoder (RAE) |


2) Protecting Sensory Data against Sensitive Inferences
Paper: [https://arxiv.org/abs/1802.07802]( https://arxiv.org/abs/1802.07802)


In this paper we propose a data transformation architecture inspired by GANs for protecting *concurrent inferences*. Here, we set up a GANs-like game between a data transformer model (Guardian) and an information extractor model (Estimator), in a way that Estimator helps Guardian to efficiently transform data for providing a good utility-privacy tradeoff. As a usecase, we show that it maintains the usefulness of the transformed data for activity recognition (with around an average loss of three percentage points) while almost eliminating the possibility of gender classification (from more than 90% to around 50%, the target random guess). 

| <img src="https://github.com/mmalekzadeh/motion-sense/blob/master/materials/gen.png"  height="300" width="400"> |
|:---:|
| Guardian Estimator Neutralizer (GEN) |

I hope you find these useful and interesting. We are always looking forward to comments and interesting ideas.
