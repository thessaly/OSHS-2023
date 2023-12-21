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

# 3. Collaboration in OSH

```{figure} imgs/16.png
---
scale: 70%
name: openinnov-fig
---
How open innovation allows firms to exchange information on R&D with new actors{footcite}`chesbrough2003open`
```

Collaboration in FOSS seems straightforward: someone downloads a source code, makes modifications and shares them back. But how does this process take place in hardware projects? We can contextualize OSH projects into what Chesbrough calls “Open Innovation”({numref}`openinnov-fig`). In his book{footcite}`chesbrough2003open`, Chesbrough describes how companies have shifted from so-called closed innovation processes towards a more open way of innovating.

Traditionally, new business development processes and the marketing of new products took place within the firm boundaries. This process has eroded due to several factors:

- Large amounts of knowledge exist outside the research laboratories of large companies due to increased mobility, collaboration and connectedness.
- When employees change jobs, they take their knowledge with them, resulting in knowledge flows between firms.
- Availability of venture capital has increased significantly recently (in the last decades), which makes it possible for good and promising ideas and technologies to be further developed outside the firm, for instance in the form entrepreneurial firms/spin-offs.
- Other companies in the supply chain, for instance suppliers, play an increasingly important role in the innovation process.

As a result, companies have started to look for other ways to increase the efficiency and effectiveness of their innovation processes. These include actively searching for new technologies and ideas outside of the firm, cooperating with suppliers and competitors to create customer value, or through user innovation.

Open innovation means combining internal and external ideas, in-bound and out-bound knowledge exchanges as well as internal and external paths to market to advance the development of new technologies/intellectual property.

## Clarifying terms
Since the 70s, people have been given more influence and room for participation within product design and development. Expertise in the informing, ideating, and conceptualising activities in the early design phases (also called the “fuzzy front end of the innovation process”), as well as product validation, were opened up to new actors.

```{admonition} Tip
:class: tip
Although the word “open” appears in many different contexts, it is necessary to introduce a very important distinction. Projects are OSH when they share product designs under free and open licenses. On the other hand, open innovation processes may not necessarily result in open source hardware. Firms can do open innovation and close down the inventions down the line.
```

"Co-design" is a term related to this process, that can often be found both in literature and practice{footcite}`sanders2008co`. By co-design we indicate collective creativity as it is applied across the whole span of a design processes (emphasise on plural form, see {numref}`collective-fig`). This change emerges from the realization that conventional design approaches cannot address the scale or the complexity of the challenges we face today. We are no longer simply designing products for users. We are designing for the future experiences of people, communities and cultures who now are connected and informed in ways that were unimaginable even 10 years ago.

```{figure} imgs/17.png
---
scale: 70%
name: collective-fig
---
Involving new actors in the design process{footcite}`sanders2008co`.
```

In co-design, through specific facilitation processes some users become co-designers. Researchers, facilitators and professional designers provide the necessary specialization to move towards production. In theory, OSH goes even beyond co-design, as it can engage external actors in the whole spectrum of activities from concept to design to manufacturing. However this does not happen quite so easily, as we will see later.

## Orchestrating collaboration in OSH

In an open hardware community, the span of collaborative practices is versatile. Similar to free and open source software, OSH work is done in two layers: a core team of developers and a broader layer of contributors ({numref}`collabprocess-fig`).

Typical tasks of the core team include defining tasks that are part of the project roadmap, evaluate contributions and validate them to be incorporated to the main project, and control of the “release” versions. A significant amount of work goes into documenting the new contributions as part of the efforts to increase reuse. Naturally, such open collaborative development activities for converging design outcomes can mainly be enabled once shared development goals have been identified and functional prototypes were built and can be shared.

```{figure} imgs/18.png
---
scale: 70%
name: collabprocess-fig
---
The open source product development process{footcite}`mies2022collaborative`.
```

Going back to the community practices that are happening already today ({numref}`collabpractice-fig`), research{footcite}`mies2022collaborative` shows that certain practices are already widely established in the community: separation of tasks, distributed contributions and reaching a collective understanding are widely adopted in the OSH field. People also publish their source files, in editable format so others can modify them.

There are however a number of practices that are known to enable collaboration, but are not widely implemented such as: issue tracking, defining contribution guidelines, sharing between contributions and having the FOSS spirit of do-ocracy that leads people to self-assign tasks. Reviews of contributions and providing feedback are still not widely implemented.

Clear gaps in practice include actively recruiting contributors, and providing regular updates, agile style. Working towards greater adoption of these practices can make the difference in greater OSH adoption.

```{figure} imgs/19.png
---
scale: 70%
name: collabpractice-fig
---
Degrees of adoption of collaborative practices in OSH {footcite}`mies2022collaborative`.
```
## A process view of OSH collaboration

As we have seen in previous units, OSH projects go through different iterative phases that can also be viewed as sets of activities. These include ideation out of a problem or need, prototyping and developing (“design activities”) and then production, use and disposal/end of life of a project{footcite}`boujut2019open`. Ideally, participation in these activities is open to multiple actors.

This poses a practical challenge for OSH projects, as described by Stirling & collaborators{footcite}`stirling2022hardops`:

> A key difficulty for open hardware projects is how to allow multiple designers to simultaneously contribute to a design, and for all contributors to have unfettered access to all of the product data [...] For open development, a system is needed which both gives each contributor full control to modify their copy of design, control over which external modifications are merged into their copy of the design, and robust data storage that ensures that each designer’s contributions are adequately recorded. This produces a rich design history, which is essential for issues ranging from design compliance to ownership and licensing agreements.
>
> [...] The toolchain and workflow for the open-source hardware development is also beginning to standardise. Distributed version control systems such as Git allow distributed teams to work on their own branch of development rather than relying on a traditional PDM. Git-based developer operations (DevOps) platforms such as GitHub and GitLab are seeing an increasing number of hardware projects, and CERN’s Open Hardware Repository (CERN 2021) is also an instance of the open-source GitLab platform. While adopting platforms originally designed for managing software has its drawbacks (Stirling et al. 2020), it also unlocks a number of powerful tools for automating time-consuming processes.

How would an automated workflow, similar to the one used in FOSS, work for OSH? {numref}`hwops-fig` illustrates what a DevOps approach would look like for OSH. In this system, automatically generated production files from designers directly reach production and prototyping teams via the Prepare and Verify stage, and the feedback from production and testing forms the inputs for future plans. This can bridge the gap between the design and production in a large organisation but can also automate enough tasks to allow a very small team to function with high efficiency and reproducibility. This is not happening today; it’s aspirational as some activists work on developing a full open toolchain for OSH{footcite}`stirling2022hardops`.

```{figure} imgs/22.png
---
scale: 70%
name: hwops-fig
---
A DevOps approach to OSH projects {footcite}`stirling2022hardops`.
```

## Collaboration in a business context
Beyond platforms and tools, companies aiming to incorporate OSH as part of their business operations may experience a significant clash of paradigms between their general modus operandi and an open source mindset{footcite}`mies2019harnessing`. For example, companies would need to understand that knowledge moves from being secret and exclusive towards a shared resource, and seek the collaborative advantage of this by forging connections with valuable external contributors ({numref}`companies1-fig`).

Another major switch implies moving from a globalised mass-production paradigm to a local distributed scale of OSH-enabled manufacturing. Venture capital funds and businesses in general aim to scale processes; however, in OSH the focus should be on producing highly personalised products to reach more users which may also be neglected due to underlying market failures.

```{figure} imgs/20.png
---
scale: 90%
name: companies1-fig
---
The open source product development process: for companies {footcite}`mies2019harnessing`.
```
Companies often work in hierarchical, rigid structures where knowledge flows vertically but is not necessarily shared across the organization. In OSH, development works differently, more similar to
an agile framework: work packages are released early, developers have autonomy and decide how to better work together, and management switches to a coaching more than managing role.

Working open source also means that errors will be “in the open”, which can be especially tough for companies (as much as this is often claimed to be the case). Treating failure as an integral part of learning and leaving room for emergent processes to take place, for example new directions, is key for companies aiming to adopt OSH ({numref}`companies2-fig`).

```{figure} imgs/21.png
---
scale: 70%
name: companies2-fig
---
The open source product development process: for companies (part 2) {footcite}`mies2019harnessing`.
```

This kind of flexibility combined with the technical capabilities needed is indeed mostly found in mature small and medium enterprises as well as some highly focussed and innovative start-ups. Corporate organisational structures are much more streamlined, so this clash of paradigms can quickly prove to be an unmanageable stretch for them and may require separate operational spheres and structures.

## Bibliography
```{footbibliography}
```
