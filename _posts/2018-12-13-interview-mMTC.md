--- 
title:  "My view on massive machine-type communications "
read_time: false
excerpt: "Interview on massive machine-type communications for the Cognitive Networks Technical Committee Newsletter"
header:
  teaser: /images/connected.png
categories: 
  - blog
tags:
  - papers
---
![image-left](/images/connected.png){: .align-center}

I recently presented my view on massive machine-type communications (mMTC) in an interview for the [Cognitive Networks Technical Committee Newsletter](http://cn.committees.comsoc.org/files/2018/12/NewsLetter_Dec_2018.pdf).
An excerpt of this interview is reported below.
Do not hesitate to [get in touch](mailto:durisi@chalmers.se) if you have questions/comments. Also, I have some [openings](/news-post/2018/11/19/vacancies/) in this area. 

***
*Question:*

How do you define future massive machine-type communication (mMTC) networks, and what will be the business cases for such 5G networks? 

*Answer:*

Machine-type communications (MTCs), i.e., machine-centric rather than human-centric communications, will form the backbone of the upcoming automated society. In 5G, they will come in two flavors: 

* ultra-reliable, low-latency communications (URLLC), which will target wireless connections with stringent requirements on both latency and reliability;  

*  massive MTC (mMTC), which will focus instead on providing connectivity to a large number of devices that transmit sporadically a low amount of traffic.

I see mMTC as the key technology needed to scale up the internet of thing (IoT), from its current limited use in the consumer sector, to its general use by enterprises and public entities, including municipalities. 

The country I live in, i.e., Sweden, has the objective to become best in the world in using the opportunities brought by digitalization. I believe that deploying mMTC solutions systematically at an enterprise and municipality level will be key to achieve this goal. 
Once available, such IoT connectivity solutions will bring many advantages, which span from increasing revenues by enabling new business models, to improving effectivity and decreasing costs. Pilot projects are already ongoing in different parts of the world where IoT technology is used for smart lightening, waste disposal, asset tracking, process monitoring and optimization, etc...

Connectivity solutions for mMTC are currently under development both in the licensed part of the spectrum (LTE and 5G) and the unlicensed part (low-power wide-area network (LP-WAN) solutions such as SigFox and LoRaWAN). One critical challenge in developing general mMTC solutions is that MTC devices will be extremely heterogeneous in terms of computational capabilities, cost, energy consumption, and transmission power. It will probably be hard to develop a single cellular technology able to address such heterogeneity, and there will be business opportunities for alternative specialized technologies, especially in the LP-WAN area.

***

*Question:*

Could you please explain the most pertinent mMTC techniques/scenarios for 5G?

*Answer:*

When I think of mMTC, I have in mind the following scenario: a wireless technology able to provide connectivity to a massive number of low-cost, low-complexity devices, which transmit sporadically small payloads. Supporting such a traffic typology requires a profound redesign of the radio-access network of current cellular systems, which are typically designed to maximize the throughput of only few active users.  

For example, the presence of a massive number of sporadically active users calls for asynchronous random-access protocols. Small payloads cause finite-blocklength effects that need to be accounted for to obtain accurate performance estimates. Furthermore, latency and energy efficiency considerations call for a redesign of control plane, aimed at minimizing protocol overheads. Finally, novel security and privacy protocols need to be developed, especially in the practically relevant use case in which low-complexity mMTC devices are connected to a powerful, but not necessarily trustworthy cloud server.

***

*Question:*

Could you please elaborate on the main role of mMTC in key vertical industries? How does the telecoms sector engages with them during the standardization phase? How does it actually build these state-of-the-art networks? Is 2020 a realistic deadline?

*Answer:*

Possible scenarios for mMTCs include structure and environmental monitoring, asset tracking, and process monitoring and optimization. The volume necessary for the success of such technology will come only if mMTCs will be used extensively in many of the services offered by municipalities. Examples may include maintenance of road signs and lightening, as well as smart waste disposal.

One challenge is that mMTCs as currently defined in 5G appear too heterogeneous for a single technology to cover all use cases. And this is true even if we focus on a single vertical scenario, say factory automation, where different MTC-enabled applications come with completely different throughput, latency, and reliability requirements. Compare for example the requirements on a wireless link used to control an actuator with the requirements on a link allowing an operator to access sensor data on a mobile device for monitoring purposes. 

Telecoms are heavily involved in pilot projects in different vertical industries. For example, Chalmers is part of a successful project in the area of [5G-enabled manufacturing](https://research.chalmers.se/en/project/8452) together with Ericsson, SKF, Volvo, and Siemens in which demonstrators for manufacturing system design, deployment, operation and maintenance are under development.

The 2020 deadline for 5G standardization seems very ambitious as far as both mMTC and URLLC are concerned. I am sure that these use cases will be at the center of several subsequent releases after 2020.


***

*Question:*

Could you please briefly introduce the most recent research project that you have done in mMTC?

*Answer:*

Over the last 6 years I have been working extensively together with many collaborators on the problem of developing communication-theoretic tools for the design of the physical layer of short-packet transmission systems. This [toolbox](https://github.com/yp-mit/spectre) is now fairly mature and ready to be used as ingredient for complex system designs beyond the physical layer.

In this respect, I have recently started two projects whose focus is precisely mMTC design. The first project, which is conducted together with two Swedish companies, [QAMCOM](https://www.qamcom.se/) and [Blink Services](https://blink.services/), and is sponsored by the [Swedish Foundation for Strategic Research](https://strategiska.se/en/about-ssf/), aims at investigating novel LP-WAN designs to support mMTC. One specific objective of the project is to optimally design a virtual network connecting LP-WAN owned by different service providers, to enable the deployment of services on a national scale.

The second project, which is supported by the [Swedish Wallenberg AI Autonomous Systems and Software Program](http://wasp-sweden.org), deals with security and privacy in mMTC. Specifically, the project has the goal of designing low-latency, massive multi-client, verifiable delegation-of-computation protocols that provide the highest possible level of security and privacy compatible with the computational resources available at the mMTC devices.

***

*Question:*

Beyond your own work, are there any resources that you would like to recommend, specially to those who are new in the field and want to learn more about mMTC? What are three key papers in the area?

*Answer:*

There are many excellent works on the design of mMTCs. I would like to highlight the following three works, which have heavily influenced my view on this subject:


* C. Bockelmann, et al., “Towards Massive Connectivity Support for Scalable mMTC Communications in 5G Networks,” IEEE Access, vol. 6, pp. 28 969–28 992, 2018.

This paper offers a comprehensive review of recent research activities on the design on mMTC for 5G, performed in the context of the Horizon2020 European Project FANTASTIC-5G. 

* Y. Polyanskiy, “A perspective on massive random access,” in IEEE Int. Symp. Inf. Theory (ISIT), Jan. 2017.

This article offers a novel framework for the information-theoretic analysis of random-access protocols. One take-home message of this article is that the currently available random-access solutions are highly suboptimal in terms of energy efficiency.

* M. Berioli, G. Cocco, G. Liva, and A. Munari, Modern random access protocols, ser. Foundations and Trends in Networking. now Publishers, 2016.

A large body of work on random access protocols has been developed over the last decade in the context of satellite communications. This book reviews the most promising strategies---a sure source of inspiration for the design of novel mMTC protocols.

***

*Question:*

What are the most important open problems and future research directions towards mMTC?

*Answer:*

The work by Polyanskiy (2017) has illustrated that classic random-access protocols, which were originally developed to maximize throughput, perform poorly when analyzed through the lens of energy efficiency. Many researchers have recently developed alternative coding schemes, which approach the fundamental limits unveiled by Polyanskiy (2017). However, most of these analyses are performed on simplified channel models. Assessing whether these alternative solutions are robust against the impairments typically encountered in mMTCs (asynchronism, lack of channel knowledge, phase noise) is an important research direction.

Next-generation 5G networks will need to support other traffic types than just mMTC. How to guarantee optimal coexistence between drastically different service types is a crucial research question.  As for the case of fading in a multiuser environment, one should be able to exploit this heterogeneity in the protocol-design phase to improve performance, a concept we referred to as "reliability diversity" in a recent [contribution](https://arxiv.org/abs/1804.05057). 

A final important research issue is privacy and security. Short payloads combined with latency constraints, and limited computational capabilities at the devices make it hard to adapt current cryptographic methods to mMTC. Recent nonasymptotic information-theory results have given us a precise way to characterize the tradeoff between reliability, energy efficiency, and throughput in the transmission of short payloads. However, very little is available on the characterization of the latency and energy overheads required to implement security and privacy protocols.

The massiveness and the sporadic nature of the MTC traffic pose unique novel challenges that the research community has started investigating only very recently. I believe that there are many opportunities to bring novel research ideas into practice, both in 5G and in LP-WAN.

To conclude, I would like to thank the following persons for the many interesting discussions on the topic of mMTC: Martin Edofsson, Johan Lassing, [Gianluigi Liva](http://www.wirelesscoding.org), [Yury Polyanskiy](http://people.lids.mit.edu/yp/homepage/), [Petar Popovski](http://petarpopovski.es.aau.dk), [Osvaldo Simeone](https://nms.kcl.ac.uk/osvaldo.simeone/index.htm), Kasper Fløe Trillingsgaard, and Andreas Wolfgang.


