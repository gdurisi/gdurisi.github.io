---
title:  "Massive MIMO for URLLC?"
date: 2020-10-09
read_time: false
classes: wide
image: /images/2020/m-mimo-cell_resized.png
excerpt: "How should one design a massive MIMO systems so that it can support URLLC?"
header:
  teaser: /images/2020/urllc_resized.png
categories:
  - news-post
tags:
  - paper
---

![m-mimo-cell_resized](/images/2020/m-mimo-cell_resized.png)

Can massive MIMO be used to support ultra-reliable low-latency (URLLC) applications? And if so, how should it be set up? These are the questions we address in the following paper, which we have recently uploaded on arXiv:

* * *
J. Ostman, A. Lancho, G. Durisi, and L. Sanguinetti, “URLLC with Massive MIMO: Analysis and
Design at Finite Blocklength,” Sep. 2020. [<a href="http://arxiv.org/abs/2009.10550">arXiv</a>]
* * *

The design of massive MIMO for systems that require large throughput is by now [well understood](https://massivemimobook.com/wp/).
However, most of the design guidelines that have been obtained so far have been developed for the so-called **ergodic regime**, where each transmitted codeword spans a large number of coherence blocks.

URLLC applications often involve short packets, typically transmitted within the channel coherence time and coherence bandwidth.
So each codeword in URLLC applications experiences a quasi-static fading channel, i.e., a constant (but random) channel. 
This means that we are typically very far away from the ergodic regime.

In the paper, we show that the so called **outage framework** (outage capacity, outage probability), altough more pertinent to quasi-static channels than the ergodic scenario, cannot be used either. 
Indeed, it yields inaccurate performance predictions when applied to the combination of URLLC plus massive MIMO. 
And the same conclusion holds for approximations of the maximum coding rate achievable at finite block-length based on the central limit theorem (**normal approximation**).

It turns out that to analyze the performance of massive MIMO systems one has to use firm nonasymptotic bound from finite-blocklength information theory. 
In the paper, we show how to adapt such bounds to massive MIMO systems, and how to evaluate them efficiently and accurately using the so-called **saddle-point method**.

The setup we consider in the paper is fairly general and encompasses imperfect channel state information, pilot contamination, spatially correlated channels, and arbitrary linear spatial processing.

Here is the **punchline** of our paper: for a practical massive-MIMO setup involving a base-station with 100 antennas, a target error probability of $10^{-5}$ can be achieved over more that $90\%$ of each cell when transmitting short packets only if

- Multicell-MMSE spatial processing rather than the simpler MR spatial processing is used

- Pilot contamination is avoided by assigning orthogonal pilot sequences to all users in the system.