---
title: 'Designing URRLC via nonasymptotic information theory
'
date: 2018-06-19
permalink: /posts/fbl-tutorial-1/
category: blog
tags:
  - FBL_tutorial
---

## Part 1: introduction



One objective of next generation wireless communication systems is to provide mission critical links that can deliver short information packets with high reliability and low latency.
The availability of such links, which are named ultra-reliable low-latency communications (URLLC) will enable a large range of novel applications such as vehicular communication for autonomous driving and traffic safety, and wireless-powered factory automation.


So how do we optimally design URLLCs? This is a tricky question, even if we just stop at the physical layer. Are our system models accurate enough to design systems operating at $10^{-6}$ frame error rate? 

But there is an even more fundamental problem. The physical-layer design of current systems relies largely on guidelines provided by information-theory analyses. For example, the well-known formula for the capacity of the AWGN channel

$$C= W\log_2\biggl(1+ \frac{P}{N_oW}\biggr)$$

 tells us that when we have limited bandwidth $W$ at our disposal, doubling the transmit power $P$ when $P$ is large, results in a capacity increase of merely a single bit per channel use. Significant rate gains must come from other sources than power. Such a consideration has spurred the development of multi-antenna systems, which provide a linear rate gain by exploiting the spatial dimension.

But to approach capacity, we need to use codes with large blocklength. And large blocklengths often mean large latency. So we cannot use classic performance metric such as ergodic capacity or outage capacity to benchmark the performance of URLLC. Neither we can use these capacity metrics to conduct joint queuing-coding analyses or to design resource allocation and scheduling algorithms.

So what we can do instead? We must replace asymptotic information-theory results with nonasymptotic finite-blocklength ones!
Over the last 10 years, the information-theory community has developed many such nonasymptotic results. Some of them, like the so-called normal approximation on the maximum coding rate achievable over an AWGN channel [^1], are now widely used in the URLLC literature.

Over the next couple of months, I plan to provide on this blog an accessible  introduction to some of the key results in finite-blocklength information theory, and discuss how they can be used to optimally design URLLC.

The plan is to start from a simple binary-input AWGN model, and then move to more sophisticated models including, e.g., fading and channel-estimation overhead, multiple antennas, HARQ, and queuing delays.



[^1]: Eq. (296) in Y. Polyanskiy, H. V. Poor, and S. Verdú, “Channel coding rate in the finite blocklength regime,” IEEE Trans. Inf. Theory,  2010.


