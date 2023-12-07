---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---
# 1. Introduction to OSH

Today, most of us are probably familiar with the concept of free and open source software (FOSS). So we are all in the same page, FOSS is software that anyone can access, study, modify or distribute it. The source code is shared online and its openness is protected through the use of a license.

```{admonition} Tip
:class: tip
FOSS is an inclusive term that covers both free software and open-source software, which have differing philosophical backgrounds. The [Free Software Foundation](https://www.fsf.org) defines free software in terms of users' freedoms, or "free as in free speech, not as in free beer". Open source software focuses more on the peer-to-peer development model.
```
FOSS is successful. Most of the web services we use today are using FOSS, from Google searches to the Android operative system, and even the backend of platforms like Facebook in huge data centres powered by Linux: open source is ubiquitous. This significant growth in the last 20 years has inspired people around the world to expand the concept of open source to other domains beyond software.

One of those emergent open source domains is open source hardware (OSH), sharing the “source code” of material objects. As researchers, one way we have of observing how the practice has grown in recent years is to look at trends in publications. Academic references reflect how much researchers are working ith a certain topic. A search of the term open hardware in Web of Science ({numref}`OSHcitations-fig`) shows that the topic is mentioned more and more in the last 20 years with a rising trend, that accelerates significantly in the last five years.

```{figure} imgs/1.png
---
scale: 80%
name: OSHcitations-fig
---
Open source hardware-related publications, extracted from [Web of Knowledge](http://webofknowledge.com/UA) on 20/11/2022
```

A closer look at the countries ({numref}`OSHcitationsbycountry-fig`) from which these publications originate, shows that the US leads the trend. However, when we combine all European countries, Europe becomes the most important region in the open hardware academic conversation.

```{figure} imgs/2.png
---
scale: 70%
name: OSHcitationsbycountry-fig
---
Open source hardware-related publications by country, extracted from [Web of Knowledge](http://webofknowledge.com/UA) on 20/11/2022
```

## Open source hardware definition and background

Before moving on, it’s necessary to make sure we all know what we mean when we refer to open source hardware, or OSH. The OSH definition is hosted by the [Open Source Hardware Association (OSHWA)](https://www.oshwa.org/), a US-based non profit


```{admonition} Tip
:class: tip
OSH can be defined as:
*"a term for tangible artifacts — machines, devices, or other physical things — whose design has been released to the public in such a way that anyone can make, modify, distribute, and use those things."*

Open source hardware gives people the freedom to control their technology while sharing knowledge and encouraging commerce through the open exchange of designs.
```

The open source hardware definition was the result of years of discussions and work in the open hardware community ({numref}`OSHhistory-fig`). The discussions can be traced back to very successful projects like [RepRap](https://reprap.org/wiki/RepRap) and [Arduino](https://www.arduino.cc/), in the early 2000s, that lowered access barriers to 3D-printing and electronics prototyping. This produced an explosion of creativity and projects worldwide, and the emergence of communities of practice around specific projects and technologies.

In this context of so much activity it was hard to understand what it meant to be open. The first open hardware licence to emerge was the [TAPR Open Hardware Licence](https://tapr.org/the-tapr-open-hardware-license/). It was written by the ham radio community in 2007 and was a little different from the open source licences we are used to, taking the format of a contract.

```{figure} imgs/3.png
---
scale: 70%
name: OSHhistory-fig
---
Highlights in a brief open source hardware history
```

Soon after, around 2009, prominent actors in the community started discussing what a unified definition of open source hardware would look like. Following these discussions and the first draft of the definition in 2010, in 2011 CERN launched its first version of the [CERN Open Hardware Licence](https://cern-ohl.web.cern.ch/).

Hardware engineers at CERN had been working on open hardware as a way of avoiding vendor lock-in of specific parts of the LHC. The licence was designed to be compatible with the open hardware definition, and soon became the most widely used one. In 2012 OSHWA was founded as a US-based non-profit to host the definition and provide a [certification program](https://certification.oshwa.org/). The non-profit also runs the annual [Open Hardware Summit](https://2023.oshwa.org/), the most important event of the community.

## Open source hardware in science
Most recently, in 2016, scientists and enthusiasts of science and education around the world created a new community, subdomain of OSHWA: the [open science hardware community](https://openhardware.science/), or GOSH. GOSH has been very active in the last five years, as the open science movement provides momentum for open hardware in science and there has always been a strong push from science in open hardware.

In research, open hardware should be considered an integral part of open science. However, most institutional open science programs today solely focus on access to open data and publications. The role of scientific instruments, both software and hardware, is often overlooked. Open hardware in science not only provides more reproducibility for research: the approach also allows researchers to prototype experimental settings, share them, improve them and access instruments that can be prohibitively expensive in a faster, more efficient way.

Open science hardware combines open hardware practices with the open science philosophy and ethos. In practice, open science hardware instruments should comply with the same definition hosted by OSHWA. Open source hardware was recognized as a key element of open science ({numref}`unesco-fig`) in the recent [UNESCO recommendation for open science](https://www.unesco.org/en/open-science/about?hub=686).

```{figure} imgs/4.png
---
scale: 70%
name: unesco-fig
---
UNESCO Open Science Recommendation (2021) including open hardware as open scientific knowledge{footcite}`pervsic2023open`.
```

## Openness in practice
One of the missions of the open source hardware definition is to clarify what it means to be open. To be recognised as OSH, designs should comply with certain requirements:

- The source files including blueprints, electronic schemes, software and other materials need to be publicly available so anyone can both access, modify, reproduce, distribute or sell the hardware;
- A license should specify the terms under which the hardware is released, but in no case the license can prevent others from making or selling derivatives;
- The license can require attribution, or for derivatives to carry different identifiers, or be strictly copyleft.

Projects can also use trademarks, as we will see in later sessions.

Today, if someone creates a project and wants to call it “open source hardware”, OSHWA provides the option of self-certifying it. This allows a project to use the open hardware logo and get an identification code. OSHWA provides [self-certification guidelines](https://certification.oshwa.org/) with details for opening hardware, software, producing documentation for others to understand how to interact with your project, and branding.

But what does this mean in practice? Research by Bonvoisin and Mies{footcite}`bonvoisin2018measuring` suggests that existing practices can be distinguished in two main categories: process openness, and product openness ({numref}`openometer-fig`). As part of this research project, the idea of measuring product and process openness was embedded in a concrete instrument: the open-o-meter. The idea behind it was not to ask whether hardware is open but how open it is. The indicator provides a progressive scale of openness in a project, moving from product to process, indicating which are the elements associated to each stage. It was intended to function both as a tool to monitor community practices and as a guide for improving those.

```{figure} imgs/5.png
---
scale: 70%
name: openometer-fig
---
OSH practices associated to process and project openness in a 0 to 8 rating{footcite}`bonvoisin2018measuring`.
```

A 2021 paper{footcite}`bonvoisin2021seven` explains the alternative routes for product development, including open source hardware ({numref}`openprocesses-fig`). Conventional development of products takes place within the Research & Development department of a firm. The norm is that designs are not shared outside the boundaries of the company: it’s both product and process-closed. One alternative that has become more popular recently is open innovation, where companies crowdsource ideas from the users community, or employ crowdfunding mechanisms. These processes open the ideation stage of product development, but most of the time lead to closed or proprietary outcomes.

Open source hardware, on the other hand, can be created in two different ways:

- As a public innovation: a specific group that does not innovate with others during the design process but shares the outcomes openly, e.g. for broadcasting or giving back to the OSH “community”;

- As open source product development: both the design stages and the product itself are opened to other actors.

```{figure} imgs/6.png
---
scale: 70%
name: openprocesses-fig
---
Open source hardware versus open design{footcite}`bonvoisin2021seven`.
```

## Motivations for engaging with OSH
One of the reasons why researchers are using and developing open source hardware is because of its
more accessible cost. A study by Joshua Pearce{footcite}`pearce2020economic` examines articles in the specialized journal [HardwareX](https://www.hardware-x.com/) and the [PLOS Open Source Toolkit](https://collections.plos.org/channel/open-source-toolkit/). They concluded that in some cases researchers could
save up to 87% costs by using open source hardware({numref}`pearce-fig`).

```{figure} imgs/12.png
---
scale: 70%
name: pearce-fig
---
OSH savings according to Pearce 2020{footcite}`pearce2020economic`
```
Researchers also engage with open source hardware to avoid the bureaucracy of dealing with
vendors when they want to try something new. Scientific instruments are made by a few specialized
companies. If researchers need a modification or repair in an instrument, they often face important
costs and delays. Open source hardware can then provide a way for bypassing the vendor and
quickly prototype a new experimental setting.

In the case of CERN{footcite}`kauttu2018open`, the very special requirements of the Large Hadron Collider made it ideal for imposing openness to suppliers. To avoid vendor lock-in with vendors, CERN developed the open hardware licence and fostered an open ecosystem where small and medium companies earn money by providing manufacturing and support services, while the designs are kept open for anyone to access.

In countries where import restrictions and distance from manufacturers play an important role,
open hardware can make the difference between running a research project or not{footcite}`arancio2023inequalities`. In the Global
South, the cost of installing an instrument is more expensive than closer to manufacturers.
Moreover, technical support is often not available and spare parts are hard to source.
Researchers in the Global South use open source hardware to overcome these limitations, design
more powerful experiments and adapt tools to their local conditions{footcite}`baden2015open`. As manufacturers are far away from implementation contexts, it is often necessary to modify tools so they become useful in situ.

From a policy perspective, open source hardware provides a way of fostering more participatory,
transparent and sustainable science practice. It opens a channel for non-academic actors to engage
with research in a creative way, and ensures that the results of investments of public funds remain
public{footcite}`arancio2022equitable`.

The GOSH community has been working recently on identifying which policies should change at
university to foster these open innovation ecosystems based on open hardware. An important
milestone was achieved in 2021, when the global UNESCO recommendation on Open Science
identified open hardware as an essential component of open science strategies, for the first time.

## Challenges of OSH practice
Since the OSH definition was adopted, there have been various initiatives aiming to standardize how to document, find and assess quality in OSH projects. When looking at what OSH projects and companies are doing in practice{footcite}`Bonvoisin-2020`, we can see clearly this trend.

However, there are some key challenges that are preventing efficient standardisation ({numref}`oshchallenges-fig`). Although the definition is more than a decade old, there’s still variety in the interpretations of what openness means, which translate to practice. Compared to FOSS, FOSH is a young field; the OSH definition is adopted in terms of licensing, but doesn't necessarily translate to other domains. It is not uncommon to find OSH projects using OSH licences but without documentation, or with very poor quality docs. This is a very important issue, as it determines if someone can truly use or contribute to a project.

```{figure} imgs/7.png
---
scale: 70%
name: oshchallenges-fig
---
Open source hardware versus open design{footcite}`Bonvoisin-2020`.
```

### OSH and standardization: COVID-19 pandemic
The need for and the nuance in standardisation can be better illustrated with an example. During the
COVID-19 pandemic, open source hardware played a key role in providing local access to essential
elements such as PPE and other devices{footcite}`bowser2021stitching`.

Many communities around the world started working on the ventilator shortage, thinking of producing a locally available open source hardware alternative. Given their envisaged use on patients and strict product certification requirements in medical technology, there was a need for testing to ensure that the equipment is safe. In industry, every product has its own testing routines that are not always easily comparable. How to ensure the OSH devices could be tested in an efficient and effective way?

The [VentMon](https://github.com/PubInv/ventmon-ventilator-inline-test-monitor){footcite}`read2021ventmon` project tackled this problem by creating an open hardware testing device and an IOT platform for openly recorded and publicly shared testing data.

```{figure} imgs/8.png
---
scale: 70%
name: ventmon1-fig
---
Open source hardware ventilator tester and monitor, Ventmon{footcite}`read2021ventmon`.
```

The device was given out for free to selected projects and the project team created an associated open access data standard. In the future, such practices could improve product certification regimes where life is at stake or public health is concerned.

## OSH applications

We gave a definition of open source hardware, showed how in practice openness is understood as
many different things, and therefore open source hardware projects available today are very
heterogeneous. However, a key question to understand this movement is what are people using
open hardware for?

```{figure} imgs/9.png
---
scale: 70%
name: oshwasurvey-fig
---
OSH fields of application, in the State of Open Source Hardware 2021 by OSHWA {footcite}`state2021`.
```

OSHWA publishes a periodic report based on a survey to the community, called the state of open
source hardware using data from their certification database. In the last 2021 report{footcite}`state2021` we see that science is gaining traction among very strong fields in open hardware, like electronics, 3D printing and education ({numref}`oshwasurvey-fig`).

The survey also asks participants about their motivations ({numref}`oshwasurvey2-fig`). We can also see that after the traditional hobbyist use of open source hardware, more people are now using OSH to learn about hardware itself. Because open hardware ideally comes with documentation that allows others to understand what is happening, it is an ideal practice to learn how devices work. In this 2021 survey we also see that almost a third of respondents mention they use open source hardware to teach or do research, which was not very frequent in previous years.

```{figure} imgs/10.png
---
scale: 70%
name: oshwasurvey2-fig
---
OSH motivations, in the State of Open Source Hardware 2021 by OSHWA {footcite}`state2021`.
```

Following up on the analysis of OSH publications, we can also disaggregate the results to illustrate which scientific fields are the most prominent({numref}`publications2-fig`). While computer science and engineering return the most results, the open hardware approach has been taken up within many other disciplines. Particularly in medical applications, open source hardware is gaining traction.

```{figure} imgs/11.png
---
scale: 70%
name: publications2-fig
---
OSH publications disaggregated by field of application, extracted from [Web of Knowledge](http://webofknowledge.com/UA) on 20/11/2022.
```

## Cases

### The White Rabbit project
[White Rabbit](http://white-rabbit.web.cern.ch/) is a project related to timing and data acquisition systems in high-energy physics experiments. Scientists and engineers at CERN needed to address the problem of minute data latency that was corrupting measurements in their distributed computing network. In 2006 they came up with White Rabbit, a piece of OSH that aims to provide a scalable and precise timing distribution system. The White Rabbit technology uses the Precision Time Protocol (PTP) to synchronize clocks across a network with sub-nanosecond accuracy.

Initially developed in collaboration with GSI Helmholtzzentrum für Schwerionenforschung and two Spanish companies, White Rabbit has evolved into a collaborative ecosystem involving various organizations. The technology's applications extend beyond the scientific industry, with examples including metrology research, neutrino telescopes, Cherenkov submarine detectors, and cosmic-ray observatories.

White Rabbit has found applications in diverse industries, including telecommunications, financial services (addressing MiFID II regulations), smart grids, air traffic control, and Industry 4.0. Notable adopters include Vodafone and the Frankfurt Stock Exchange, with applications in High-Frequency Trading (HFT) matching engines. The Madrid Stock Exchange is piloting White Rabbit for time distribution, and the technology has gained attention in the Smart Grid community.

Pujol & Warenham (2019){footcite}`pujol2019obsessed` interviewed members of the project and describe the benefits of an open source approach:

> First, an open source approach made it possible to avoid a vendor lock-in situation; given the initially high asset-specificity of the technology, there is a high risk of dependency on specific technology suppliers. Secondly, an open source model should offer a more diverse and rigorous evaluation of technology development [...] Finally, flexibility is a particularly important characteristic for researchers working on the edge of science who need customized, never-before-seen equipment to meet their exact needs and specifications in an uncertain and modular environment.

You can read an interview to the project members in the [OpenMake blog](https://www.openmake.de/blog/2022/10/20/2022-10-06-interview-white-rabbit/).

### The Smart Citizen project
The [Smart Citizen System](https://smartcitizen.me/) is a comprehensive set of modular hardware components designed for environmental monitoring. The system serves various purposes, including citizen science, educational activities, and advanced scientific research. It consists of a central data logger with network connectivity, to which different components are connected. The core sensing capabilities utilize low-cost sensors reviewed for environmental monitoring. The system is extendable and integrates non-hardware components like a dedicated storage platform and a sensor analysis framework.

The motivation behind the Smart Citizen System lies in addressing the dual needs of citizen science and more sophisticated scientific research. To fulfill these needs, two solutions have been developed: the Smart Citizen Kit for citizen science and awareness activities, and the Smart Citizen Station for more complex and accurate air pollution sensing.

The system allows for connection with a wide range of third-party sensors through an expansion bus. It aims to provide a low-cost sensing solution, an open-source end-to-end solution for scientific development, and an educational tool. The Smart Citizen System allows end-users to participate not only in measurement activities but also in the analysis and development processes.

A research paper in HardwareX{footcite}`camprodon2019smart` describes the hardware for both the Smart Citizen Kit and the Smart Citizen Station. The project builds on the legacy of previous generations of the Smart Citizen project and has been developed as part of the of iSCAPE (Improving Smart Control of Air Pollution in Europe) project, which is funded by the European Community’s H2020 Programme.
The [Smart Citizen System](https://smartcitizen.me/) is a comprehensive set of modular hardware components designed for environmental monitoring. The system serves various purposes, including citizen science, educational activities, and advanced scientific research. It consists of a central data logger with network connectivity, to which different components are connected. The core sensing capabilities utilize low-cost sensors reviewed for environmental monitoring. The system is extendable and integrates non-hardware components like a dedicated storage platform and a sensor analysis framework.

The motivation behind the Smart Citizen System lies in addressing the dual needs of citizen science and more sophisticated scientific research. To fulfill these needs, two solutions have been developed: the Smart Citizen Kit for citizen science and awareness activities, and the Smart Citizen Station for more complex and accurate air pollution sensing.

The system allows for connection with a wide range of third-party sensors through an expansion bus. It aims to provide a low-cost sensing solution, an open-source end-to-end solution for scientific development, and an educational tool. The Smart Citizen System allows end-users to participate not only in measurement activities but also in the analysis and development processes.

A research paper in HardwareX{footcite}`camprodon2019smart` describes the hardware for both the Smart Citizen Kit and the Smart Citizen Station. The project builds on the legacy of previous generations of the Smart Citizen project and has been developed as part of the of iSCAPE (Improving Smart Control of Air Pollution in Europe) project, which is funded by the European Community’s H2020 Programme.

## Slides for download

[Link to slides](slides/OSHS_units1and2.pdf)

## Bibliography
```{footbibliography}
```
