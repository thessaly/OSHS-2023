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

# 8. OSH communities & governance

```{figure} imgs/42.png
---
scale: 80%
name: gov1-fig
---
Source: [Community Rules](https://communityrule.info)
```
A governance model refers to the structure, processes, and mechanisms put in place to ensure effective decision-making, control, and oversight within an organization, community, or any structured group. It defines how authority, responsibility, and accountability are distributed and exercised.

Governance models define how decisions are made within the organization including mechanisms for gathering input, deliberation, and final decision-making. They also describe the formal hierarchy, roles, and responsibilities, reporting lines, roles of leadership, and the overall structure of the entity.

It makes explicit which are the rules, guidelines, and standard operating procedures that govern the organization. These may cover a wide range of areas, including ethics, compliance, and operational protocols. They also describe how the implementation of these is evaluated, and what happens when these are broken. How individuals or entities within the organization are held accountable for their actions and decisions?

Probably the most important aspect of governance models is that they outlien processes for resolving disputes or conflicts within the organization. This can include mediation, arbitration, or other conflict resolution mechanisms.

Governance models are crucial for ensuring that organizations operate transparently, ethically, and efficiently. They provide a framework for decision-making that aligns with the organization's goals and values, and they help establish a system of checks and balances to prevent abuses of power. Governance models can vary widely depending on the type of organization, its size, purpose, and the regulatory environment in which it operates.

## Communities in OSHS
Communities in OSH are heterogeneous, focusing either on projects, platforms or networks of networks. Some open hardware projects and their communities became so popular that you will hear about them, or the paradigm they represent, really often. One of these examples is Arduino, which enabled thousands to prototype electronic designs in an accessible way. Another example of huge activity is the 3D printing community, where you can find contributors everywhere working on models that go from the first RepRap to one of its current popular grand-grand-daughters, Prusa.

Other communities gather around the field of application of what they are building. You will hear often about the Do It Yourself (DIY) or “maker” community, tweaking and creating designs for hobbist or educational purposes. When it comes to science, the Global Open Science Hardware (GOSH) is a "community of communities" bringing together people in or outside academia building tools for science and education. Specific fields have their own communities, like open source biology or open source optics.

Networks like Hackteria gather lots of artists working with open hardware and DIY biology, while platforms like Appropedia collect open designs of tools for sustainable living. Online communities also form around platforms for sharing designs (Hackaday, Instructables, Hackster, KitSpace, etc) or tools needed for designing and building hardware.

## How is work organized in OSH?
Open-source communities tend to emerge and organise themselves organically{footcite}`sadowski2008transition`, starting with a very specific need of an individual or small group of individuals. Communities are made up of volunteers and, sometimes, sponsored participants. Governance structures tend to appear much later, in response to growth and the need for responsive work, the emergence of conflic or new interactions with companies.

The Onion model is a popular way of conceptualizing work in FOSS communities. It categorizes participants following a core-periphery structure according to their contributions to source code, and therefore their power to make decisions about a project. Core developers are often in charge of managerial work, like approving contributions, while the periphery often performs support work, like fixing bugs{footcite}`rullani2013periphery`.

```{figure} imgs/43.png
---
scale: 70%
name: onion-fig
---
The “onion model” in open source communities {footcite}`crowston2003social`
```
Due to OSH being so recent, there are less studies on the community dynamics of OSH projects and their governance. Recent research{footcite}`boujut2019open` on OSH projects shows that there is also a "core" made up of a small number of participants. However, there is no standard way of organizing work. In some cases, but not at all the majority of them, projects followed a similar work division to design in industrial contexts: those who design, develop and prototype are different people. However in many others participants take part in at least two activities: those who design also develop and sometimes even prototype objects.

```{figure} imgs/44.png
---
scale: 70%
name: oshcollab2-fig
Profile of OSH participants according to design activities{footcite}`boujut2019open`
---
```

## Governance models for open source
Governance models are used in every organization, but as we mentioned in the beginning, they are often implicit in FOSS and OSH. Groups form and grow before they can consider how they will share power and deal with the conflicts that inevitably arise.

[Community Rules](https://communityrule.info) is an interactive tool developed by a team of researchers at University of Colorado Boulder. It presents governance models and their components with examples, as building blocks that people can use to generate their own customized governance.

**1. Benevolent Dictator**

In this model, a single individual, often the project founder or a highly respected leader, holds significant decision-making authority over the project. This person is colloquially referred to as the "benevolent dictator".

Participation is open to anyone who wants to join, but the benevolent dictator can remove participants at will. The benevolent dictator has authority and can change the group’s governance as necessary. The benevolent dictator can invite participants to help with managing the group. When the group is sufficiently mature, the benevolent dictator will establish a more inclusive structure.

The benevolent dictator is responsible for implementing—or delegating implementation of policies and other decisions. If participants are not happy with the benevolent dictator’s leadership, they may voice their concerns or leave the group

```{admonition} Example
:class: tip
**Python.** Its creator, Guido van Rossum, served as the benevolent dictator before stepping down from the position in 2018. Upon van Rossum’s resignation, the Python Software Foundation adopted an elected board model of governance. The new model employs a five-person steering committee elected by core developers that determines standardized practices for the programming language.
```

**2. Circles**

Units called circles have the ability to decide and act on matters in their domains, which their members agree on through a council. To join, a person must be welcomed into a particular circle according to its
policies.

Representatives of circles regularly meet in a council to coordinate efforts and determine the domains of each circle, as well as to add or remove circles from the council. A circle can create roles for its members and assign authority over specified sub-domains. Circles and the council use consent to make decisions. Consent means that nobody presents a serious objection to a proposal.

```{admonition} Example
:class: tip
**[Meerkat Media](https://MeerkatMedia.org).** Artists associated with the Meerkat Media Collective receive a monthly stipend to pursue independent or collaborative projects. Commissioned projects are democratically run through the Meerkat Media Workers Cooperative
```
**3. Consensus**

Decisions that affect the group collectively should involve participation of all participants. New participants may join as long as no others object. Participants may be removed if a proposal to do so passes the consensus process.

People who make proposals that the group agrees on is responsible for its implementation, delegating as necessary and as participants are willing to help. Any participant may make a proposal at any group meeting to which all participants are invited. The proposal should be discussed and modified through
open conversation in order to address all concerns. A decision is made only if there are no serious objections remaining.

```{admonition} Example
:class: tip
**[CECOSESOLA](https://Boell.de/en/2016/01/21/venezuela-we-are-one-big-conversation).** CECOSESOLA is a consensus-based cooperative based on mutual trust and respect. Everyday decisions can be made by individuals or subgroups but must adhere to a common criteria that is established and revised through member consensus.
```

**4. Do-ocracy**
Those who take initiative to do something in the group can decide how they do it. New participants may join as long as no others object. Participants may be removed if a proposal to do so passes the consensus process.

People who make proposals that the group agrees on is responsible for its implementation, delegating as necessary and as participants are willing to help. Any participant may make a proposal at any group meeting to which all particpants are invited. The proposal should be discussed and modified through
open conversation in order to address all concerns. A decision is made only if there are no serious objections remaining.

```{admonition} Example
:class: tip
**[Social.coop](https://Social.coop/about).** Tasks are done through voluntary committees, although some roles come with small stipends. Any member may make a proposal for a policy, which can be passed through a vote of the membership. All financial transactions are public.
```

**5. Elected board**
An elected board determines policies and organizes their implementation. The board sets policies for membership and removal.

A board is responsible for making decisions and implementing them, including by delegating necessary work to others. Any community participant can be a nominee for board positions. In regularly scheduled elections, the nominees with the largest number of votes become board members. The board makes deci-
sions by majority vote.

```{admonition} Example
:class: tip
**[SEWA Cooperative Federation](https://SewaFederation.org/about-us).** The federation’s members, which are themselves cooperatives governed by their worker-members, elect a board of nine to fifteen members. This board governs the federation and elects its president.
```
**6. Jury**
Proposals are shaped and decided on by randomly selected juries. Juries set policies for membership
and removal.

Temporary juries form by a random selection. All participants have the right to initiate proposals, sign them, and serve on juries. If a certain percentage of participants signs a proposal, a jury is formed to study it, revise it, and agree on it unanimously. A proposal agreed on by a jury becomes binding for the group.

```{admonition} Example
:class: tip
**[Forest of Dean District Citizen Jury](https://CNDP.us/forest-of-dean-citizens-jury).** A group of eighteen residents were selected to form the jury responsible for determining the location of the new
hospital. The jury considered demographics, potential population growth, and transportation before voting on a final location.
```

**7. Petition**
All participants can propose and vote on proposals for the group. Petitions set policies for membership
and removal; any structures must be established by petition.

All participants have the right to initiate proposals, sign them, and vote in resulting referendums. If a certain percentage of participants signs a proposal, it goes to a referendum. If a majority of
participants vote for it within a certain period of time, it becomes binding for the group.

```{admonition} Example
:class: tip
**[Decide Madrid](https://Decide.madrid.es).** The Madrid City Council encourages citizen involvement in governance through the use of Decide Madrid. Citizens work together to produce and ratify legislation that benefits the entire community
```

**8. Self-appointed board**
A board that selects its own members determines policies and organizes their implementation. The board sets policies for membership and removal.

A board is responsible for making decisions and implementing them, including by delegating necessary work to others. The board elects its own members and makes decisions by majority vote.

```{admonition} Example
:class: tip
**[Facebook Oversight Board](https://OversightBoard.com).** The initial board members were chosen by Facebook in collaboration with consulting firms and executive search firms. Facebook interviewed
nominees and selected four co-chairs for the board who then helped choose the remaining sixteen board members. Although anyone can be nominated to serve as a board member, Facebook and the board approve new board members.
```

## Implications of governance (non)choice
The absence of a governance model in an open source project can lead to various challenges and implications, potentially impacting the project's sustainability, community dynamics, and overall success.

Probably the most immediate consequences are related to decision-making. Without a defined governance model, there may be a lack of clarity on how decisions are made and who has the authority to make them. This can result in confusion and uncertainty among contributors. Decisions may be made inconsistently, leading to disputes and disagreements within the community. In the absence of a structured process, decisions might be influenced by individual preferences rather than project goals.

The community can start witnessing how participants disengage. Contributors may become frustrated if they perceive a lack of fairness or transparency in decision-making. This frustration can lead to a decline in contributions, diminishing trust within the community. Contributors may be hesitant to invest time and effort into a project if they are uncertain about the project's future and decision-making processes.

Projects without a governance model may struggle to evolve and adapt to changing circumstances. Lack of clear leadership and decision-making processes can result in project stagnation. In the absence of a clear path for resolving disagreements or addressing dissatisfaction, contributors may choose to fork the project, creating a separate, independent version. This can lead to fragmentation and a loss of the collaborative benefits of a unified community.

A governance model helps ensure that decisions are made inclusively, considering the perspectives of various community members. Without such a model, there is a risk of excluding certain contributors or groups from the decision-making process. Adressing and resolving instances of community member misconduct may be challenging. A code of conduct without a mechanism for enforcement is not effective.

A lack of governance, in conclusion, affects sustainability. Projects with no governance model may be overly dependent on individual contributors. If key contributors leave or lose interest, the project may die. There may be no clear process for selecting new leaders or maintainers, which can jeopardize the project's long-term viability.

```{figure} imgs/46.png
---
scale: 70%
name: oshcollab2-fig
---
Implications of model choice in everyday practice
```

## Bibliography
```{footbibliography}
```
