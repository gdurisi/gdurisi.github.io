---
title: "Plenary talk at ITW 2021"
date: 2021-10-23
read_time: false
excerpt: "Plenary talk at the 2021 Information Theory Workshop"
categories:
  - news-post
tags:
  - talks
header:
  teaser: /images/talk2.png
---
It was a great pleasure to give a plenary talk at this year [Information Theory Workshop (ITW)](https://www.itw2021.org). 
My talk was entitled "Short packets over wireless fading networks". 
The slides can be downloaded [here](https://chalmersuniversity.box.com/s/rfqz5w5w4g93icjfh67mcwwlb107t6oi). 
A video recording is available on the ITW website for registered users and will also be made available to everyone on the Information Theory Society [website](https://www.itsoc.org).

The theme of the talk was to show how to use finite-blocklength information-theoretic tools to optimally design wireless fading networks supporting the transmission of short packets.

What do I mean by short packets? In a nutshell, I refer to "short packets" as  wireless traffic where one wants to deliver around hundreds of bits within around hundreds of degrees of freedom per user. 
This regime turns out to be relevant for both ultra-reliable low-latency communications (URLLC) and massive machine-type communications (mMTC).

More specifically, I asked in the talk the following question.
Assume that we want to design a resource allocation algorithm, or maybe a user scheduling algorithm, for a wireless system that needs to support short packets.
Which information-theoretic formula shall we use to model the physical layer? Or more specifically, 
what should we replace the typically used asymptotic $\mathbb{E}[\log(1+\text{sinr})]$ ergodic-capacity lower bound with?

In the talk, I provide an answer to this question: it involves the use of an achievability bound in finite-blocklength information theory called the *random coding union bound with parameter $s$*, the use of *pilot-assisted transmission* and *nearest-neighbor mismatch decoding*, and of the *saddlepoint method* in statistics to evaluate the resulting bound in a computational effective way.

I also clarify why the so called *normal approximation* should probably not been used when designing URLLC systems, and in particular why taking ergodic SINR expression and inserting them into AWGN-based normal approximation formulas does not lead to information-theoretic rigorous expressions.

Finally, I provide study cases relevant for  $5G$ and beyond, which illustrate that the proposed approach can be applied to real-world wireless communication networks involving base stations with large-antenna arrays, realistic propagation models, multiuser interference, and imperfect acquisition of channel state information. 




