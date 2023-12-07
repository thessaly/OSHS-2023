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

# 2. Ideation and prototyping

OSH projects are, as any other projects, born out of a problem or necessity that a developer considers can be addressed by creating a new product. This need is afterwards turned into “features”, or things that the product should be able to do. Using rapid prototyping tools such as Arduino boards or 3D printing, developers can now prototype multiple hardware ideas quite easily. These can be tested quickly, in multiple iterations, gathering user feedback to improve the prototypes.

This way iterative and incremental way of developing technology is well-known in software{footcite}`larman2003iterative`. After many iterations and testing, a prototype can be selected for further development. The selected design, that solves a need but is not yet complete nor ready to be replicated (usually because some parts are not well documented or requires a lot of manual adjustments), is sometimes called a demonstrator. When the design and documentation are polished and are ready to be used by hardware producers, the hardware is usually labeled as a market-ready product{footcite}`the_turing_way_community_2023_7625728`.

```{figure} imgs/13.png
---
scale: 70%
name: stagesOSH-fig
---
Open technology readiness levels{footcite}`mies2022introducing`
```

Prototypes are not perfect and look nothing like a final product; they are just a way of testing specific features early on in the life of the project. For this reason, most teams start their documentation process at the demonstrator point({numref}`stagesOSH-fig`). However, open science enthusiasts advise being open from the beginning of the description of needs phase. This way, the rationale behind the project is also shared and others can learn from the team's decision-making process.

## Core elements of OSH projects

As in many technology products, technical development happens before thinking about users, contributors, forks or replications. However, it is crucial for projects to consider these aspects early on to avoid generating products that actually respond to no real need.

A consistent project should be able to answer the following questions:
- What does the device do?
- What changes because this project exists/Why are you doing this? (Value proposition)
- Who are the users? Are the same as potential contributors? If not, who are potential contributors?

Being able to communicate these points is crucial for onboarding new users, contributors, and potential investments. As we will see in following units, one of the key differentiators of successful OSH projects is communication. This means how effectively you communicate what your project does, so new users and contributors are attracted to it.

Although these questions sound simple, they are often quite complex. It is common to see new OSH projects starting because of just fun or learning a new technology. Other projects are market-oriented from the very start. Understanding your own motivations is key to avoid investing too much or too little energy on specific aspects of the OSH journey. As an example, writing documentation for potential manufacturers is absolutely different than documentation for teachers.

## A minimum viable product (MVP)
When a hardware project is aiming to become a marketable product, it is not uncommon to hear about the concept of "Minimum Viable Product" (MVP){footcite}`fi11020050`. Similar to what we earlier called the demonstrator, its goal is allowing to test the feasibility of a product or idea with minimal resources. At its core, an MVP represents the most basic version of a product that can be developed and launched to meet the initial needs of early adopters.

In the realm of hardware development, a Minimum Viable Product (MVP) represents the initial version of a physical product designed with the essential features required for functionality. Unlike software, hardware MVPs involve tangible, often complex, physical components. The goal is to introduce a simplified version of the product to the market, primarily to test its feasibility, gather user feedback, and assess its reception{footcite}`chen2016bringing`.

This iterative approach allows for rapid adjustments and improvements based on real-world usage and user insights. The hardware MVP is a strategic development tool, emphasizing efficiency in design, manufacturing, and cost management while providing a foundation for future iterations and enhancements. It serves as a crucial step in the hardware development lifecycle, enabling teams to validate their ideas, refine their designs, and make informed decisions for the product's evolution.

### MVPs in open source
Open-source MVPs are released early in the development process, inviting collaboration from a diverse community of developers, contributors, and users. This initial release is designed to be transparent and openly accessible, aligning with the core principles of the open-source philosophy. By making the MVP available to the community, developers encourage feedback, bug reporting, and active participation in the project's evolution.

The iterative nature of open-source development is key to the MVP approach. The initial release serves as a starting point, with subsequent iterations driven by feedback and contributions from the community. Features can be enhanced, refined, and expanded based on the diverse needs and perspectives of the contributors{footcite}`gibb2015building`.

By involving the community early in the development process, the project fosters a sense of shared ownership and responsibility. Contributors not only have the opportunity to submit code but also to engage in discussions, offer insights, and contribute to areas like documentation and testing. The open-source MVP also acts as a catalyst for building momentum around the project. Its early release attracts potential contributors, users, and advocates who are drawn to the project's goals and functionalities. This early engagement helps create a vibrant and supportive community ecosystem.

Clear documentation is paramount in the open-source MVP context. Thorough documentation helps contributors understand the project's purpose, architecture, and how they can actively participate. This transparency aids in onboarding new contributors and ensures a shared understanding of the project's objectives. License considerations are critical when releasing an open-source MVP. Choosing an appropriate open-source license is fundamental to defining how the software can be used, modified, and distributed within the community.

## Modularity

Modular design, or modularity in design, is a design principle that subdivides a system into smaller parts called modules. These can be independently created, modified, replaced, or exchanged with other modules or between different systems.

```{admonition} Tip
:class: tip
Modularity is an attribute of a complex system that advocates designing structures based on minimizing interdependence between modules so that they can be mixed and matched to obtain new configurations without losing the system’s functionality or performance{footcite}`baldwin2000design`,{footcite}`modularityAlto`
```

A modular design can be characterized by functional partitioning of a product architecture into discrete scalable and reusable modules, rigorous use of well-defined modular interfaces, and making use of industry standards for interfaces.

Modularity offers many benefits:

- Reduction in cost: customization can be limited to a portion of the system, rather than needing an overhaul of the entire system,
- Interoperability: when using standards it allows mix & match,
- Shorter learning time: it is easier to isolate features of interest to learn about rather than learning about whole systems,
- Design flexibility / configurability: it is easier to modify a feature if this one can be isolated,
- Easier to update or augment: malfunctions or upgrades can be isolated without changing the whole design

When developing projects in the open, it is useful to see what is available out there and how it could be incorporated in a project to save time and effort. In other words, if someone for example has already created a good system to measure temperature within given costs, performance and boundaries, there is quite often no point in starting from scratch and develop the same system again. More effective would be to replicate the already existing temperature measuring system and adapt it (where necessary) to the project's needs.

Modularity is used in open hardware projects because it makes it easier for others to take the parts that are useful to them and create derivatives or contribute to specific features. Modularity is also useful when a device breaks down, to easily detect and isolate a malfunction. Think of updates: if your design is modular, one module can become obsolete, but you will be able to update it without changing the whole device.

### Promoting reuse with modular design

One way OSH projects have for becoming widely adopted is to follow modular design principles. If the device can be separated in discrete portions which provide different features, it is much easier for other to interact with it. People can grab a module and change one small feature, instead of having to learn everything about the project at once.

If a project is modular enough and follows widely adopted standards, it will be easier for others to use it within their ongoing workflows. Modularity and standardization create compatibility, which makes projects much more attractive to work with.

Back to the temperature example. Project documentation should clearly state which are the exact components in the system that are responsible for temperature sensing, and how they communicate with the rest of the system. On hardware, the temperature sensing function should be self-contained within a group of specific components, that can be replaced or modified easily without affecting the overall functioning of the project.

In this way if another project wants to use just that function, it can easily find out what parts are needed and how it can be implemented somewhere else. Modularity is also useful within the project, as a certain module can be used more than one time in different parts of the system.

In short, once a module has been developed, it can be used by other projects (which increases the chances of that module being improved/supported over time), again in the same project and over time, in different projects by the same developers. Finally, this also helps with sorting components, as different projects with the same modules will require similar components. Modular design inherently combines the mass production advantages of standardization with those of customization.

## Interoperability
Interoperability is necessary to enable modular design and to realise some of the most commonly cited advantages of OSH. Howerver, it is not simple to embed interoperability within general OSH standards. Interoperability relies on a network of technology-specific standards for communication, software and data exchange between different components and devices, in addition to physical interoperability of components such as dimensions and thread size​.

It is often easier to find interoperability in specifications for specific domains. One example of such technology specific standard is the BioBrick{footcite}`shetty2008engineering`.It is a standard in the area of synthetic and molecular biology for the physical composition of genetic parts. The BioBrick can be counted towards technology specific Open Hardware standards since it is concerned with physical material (DNA), even if not of classical electro-mechanical kind. It specifies BioBrick "parts" as functional genetic sequences (genes) that use a defined set of sequences to interface with BioBrick "vectors" as the structural DNA backbone used to handle genes for cloning. The interface sequences that flank the genes are recognised by a defined set of restriction enzymes, which are needed to assemble and transfer parts in a universal manner.

A major area of growth and funding in open hardware are open Instruction Set Architectures (ISAs) such as [RISC-V](https://riscv.org/), where the RISC-V Foundation manages the standard specifications and RISC-V software is managed by respective open source software projects; these initiatives allow users to design interoperable microprocessors that can be hard-wired or programmed (for example in field programmable gate arrays - FPGAs). Open ISAs increase opportunities for OSH projects to adopt open approaches at multiple levels of design but the existing specifications do not address the desirability or enforceability of such decisions.

## Original, fork, replica
Once documented and published freely/open source, a project can be reused by others who may replicate it, adapt it to their needs or contribute new features. OSH projects can start as an original design that doesn’t reuse any open source components from other projects.

Others may interact with this project by replicating it as it is, without changing anything. People can also add their own features, translate documentation or improve UX components. These are not new projects; they are considered contributions as long as they are part of the project roadmap.

In some cases, people take OSH designs and adapt them to their own needs, departing from the development plan of the original design. This is what we call a derivative or fork{footcite}`gibb_making_2014`. There may also be what is called remixing in industrial design which can be found with simple 3D objects like on Thingiverse, the world’s largest website for sharing “user-created digital design files.”

Most projects in fact are made by individuals or small teams who share their own work for others to reuse it or notice it (broadcasting). In relative terms, there are quite few large-scale collaborative OSH development projects as in software with tens or hundreds of contributors.

Understanding the intended reuse is very important when choosing a license, because as projects get reused there may be compatibility conflicts between licenses, but more about this in the upcoming seminar on licensing.


```{figure} imgs/14.png
---
scale: 70%
name: clonefork-fig
---
Different pathways for working with projects by [TechTarget](https://www.techtarget.com/)
```

## The Open Hardware canvas
The OH Canvas ({numref}`ohcanvas-fig`) is a one-page format used for describing your project, developed by the [Open Hardware Makers](https://openhardware.space) team. It is a way of clarifying the core of an open hardware project, encouraging you to think strategically about project goals, plans, and resources.

It has three main sections:
1. At the centre of the canvas we find the value proposition, the project components and a short review of similar projects.
2. On the left side, “people” items: who are your users, contributors, how do you communicate with them and which documentation you need to engage them.
3. On the right side, hardware specifics: which resources you require, your BoM, assembly instructions, licenses.

The canvas was adapted from the [Mozilla’s Open Canvas](https://mozilla.github.io/open-leadership-training-series/articles/opening-your-project/develop-an-open-project-strategy-with-open-canvas/), which in turn was adapted from the [Lean Canvas](https://bmtoolbox.net/tools/lean-canvas/), a common tool in business applications.


```{figure} imgs/15.png
---
scale: 30%
name: ohcanvas-fig
---
The Open Hardware canvas is a tool for visualizing the core components of an OSH project at a gaze ([source](https://github.com/ohwmakers/ohcanvas))
```

The following units dive deeper into each of these components. If the project you are working on with the practice partner involves hardware prototyping, it is convenient for you to draft a first version of the OH canvas which we will review as the project advances.

## Slides for download
[Link to slides](slides/OSHS_unit3.pdf)

## Bibliography
```{footbibliography}
```
