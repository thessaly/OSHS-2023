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

# 6. Licences & standards

## What is an open source licence?

Open source licenses are legal instruments that govern the use, modification, and distribution of open source products. OSH licences have historical precursors in FOSS licences and community definitions{footcite}`luis2019open`. These licenses are crucial components of the FOSS success, providing a framework for how software and hardware can be shared, collaborated upon and used by individuals, organizations, and communities.

Open licences are the concrete instruments were the freedoms for the user are established. This fosters a collaborative environment where individuals can contribute to and benefit from the collective knowledge and skills of the community. Contributors understand how their work can be used and how it can not, facilitating a transparent and cooperative approach to software and hardware development.

```{figure} imgs/31.png
---
scale: 70%
name: lic1-fig
---
Basic concepts on open source licencing {footcite}`beldiman2018bits`.
```

Licenses provide legal clarity on the terms and conditions under which the software/hardware can be used, modified, and distributed. But they also play a critical role in demonstrating transparency that builds trust among users and contributors. Open licences can be thought of as an agreement within communities, describing conditions, obligations and moral orientations for the circulation of hardware designs.

### Public domain, open-source...

When learning about open source licences it is not uncommon to be confused by other terms like public domain or copyright. These are different approaches to managing intellectual property rights. Public domain emphasizes complete freedom, copyright grants exclusive rights with limitations, and open licenses provide a structured way to share and collaborate while retaining copyright.

**Copyright** is a legal right that grants the creator of an original work exclusive rights to its use and distribution. These rights include the right to reproduce, distribute, perform, and display the work. Copyright restricts the use of a work without the explicit permission of the copyright holder. It provides a legal framework for creators to control how their work is used and to financially benefit from its exploitation. Copyright protection has a limited duration, which varies by jurisdiction. Once copyright expires, the work enters the public domain.

Works in the **public domain** are not protected by copyright and are freely available for use by the public. They may include works where copyright has expired, works explicitly dedicated to the public domain by the creator, or works for which copyright never existed. No copyright restrictions apply to public domain works, allowing anyone to use, modify, and distribute them without seeking permission.

Public domain status is typically achieved when copyright expires, which varies by jurisdiction. As examples, the works of William Shakespeare or Ludwig van Beethoven are in the public domain either by virtue of their having been created before copyright existed, or by their copyright term having expired. In other cases, like the [Smithsonian Open Access](https://www.si.edu/openaccess) initiative launched in 2020, copyright is explicitly waived and released into the public domain as Creative Commons Zero (CC0).

```{admonition} Tip
:class: tip
[Creative Commons Zero or CC0](https://creativecommons.org/public-domain/cc0/) "No rights reserved" enables scientists, educators, artists and other creators and owners of copyright- or database-protected content to waive those interests in their works and thereby place them as completely as possible in the public domain, so that others may freely build upon, enhance and reuse the works for any purposes without restriction under copyright or database law.
```
**Open licenses** are legal instruments that accompany creative works and grant permissions beyond what default copyright laws allow. They are used in open source and creative commons contexts to facilitate sharing and collaboration. Open licenses retain copyright but grant specific permissions to users. The permissions may include the right to use, modify, and distribute the work, often with the requirement that derivative works also carry the same open license.

```{figure} imgs/32.png
---
scale: 90%
name: pdom-fig
---
Key differences between public domain, open licences and all rights reserved copyright {footcite}`chae2014`.
```

### Approaches to licensing

**Copyleft** is a general approach to licensing in the context of open-source software that emphasizes the freedom to use, modify, and distribute software while imposing the condition that any derivative works must also be distributed under **the same license terms as the original work**. In this way it aims to preserve free and open source principles by imposing reciprocal obligations on contributors/forkers.

The concept of copyleft originated in the early 1980s within the context of the Free Software Foundation (FSF) and the GNU Project, both founded by Richard Stallman. Stallman initiated the GNU Project in 1983, with the goal of creating a free and open-source Unix-like operating system. The name GNU stands for "GNU's Not Unix," emphasizing the project's goal of creating a Unix-compatible system that respects users' freedom. In 1989, Richard Stallman introduced the GNU General Public License (GPL) as part of the GNU project. The GPL was designed to be a copyleft license, ensuring that software covered by the license remains free and open in perpetuity.

Copyleft, as embodied in the GPL, was conceived as a legal mechanism to guarantee that the freedoms associated with free software would be preserved. It achieves this by requiring that any modified or extended versions of GPL-licensed software also be distributed under the terms of the GPL. In this way it prevents lock-in, or the creation of proprietary versions that restrict user freedoms. On the other hand, some argue that the reciprocal nature of copyleft licenses may limit the ability of the software to be integrated into proprietary projects and therefore its broader adoption.

Over time, variations of the GPL and other copyleft licenses have been developed to address specific use cases. For example, the Lesser General Public License (LGPL) and the Affero General Public License (AGPL) are variations that adapt copyleft principles for different scenarios.

```{figure} imgs/33.png
---
scale: 70%
name: popularlicences-fig
---
Most popular open source software licences in 2021 {footcite}`rjjiii2023`.
```
**Permissive licenses** are a category of open-source software licenses that grant users extensive freedom to use, modify, and distribute the software with minimal restrictions. Unlike copyleft licenses, permissive licenses impose fewer obligations on users regarding how they distribute derivative works. These licenses prioritize flexibility and allow developers to incorporate open-source code into both open and closed source projects.

Permissive licenses grant users the freedom to use the software for any purpose, whether it be personal, commercial, or proprietary. Users are free to modify the source code of the software to suit their needs. There are typically no requirements to share modifications. Users can distribute the software and its modifications under different licenses, including proprietary licenses. There is no obligation to release the source code of derivative works.

Examples of Permissive Licenses include the MIT License, one of the most widely used permissive licenses. It allows for almost unrestricted use, modification, and distribution of the software, with minimal requirements. The BSD License (2-clause and 3-clause) permits users to do anything they want with the code, including creating proprietary derivatives, as long as the original copyright notice is retained. Finally, the Apache License allows for the use, modification, and distribution of the software, with additional provisions addressing patent rights and indemnification.

Permissive licenses aim to achieve a balance between openness and flexibility, allowing for broad usage and integration into various projects, including proprietary ones. They are suitable for developers who prioritize freedom of use and compatibility with commercial applications. However, as they do not require users to share modifications or improvements, this may limit contributions back to the open-source community.

```{figure} imgs/37.png
---
scale: 100%
name: permissionstable-fig
---
Permission overview for software licences{footcite}`the_turing_way_community_2023_7625728`
```

## Licences in OSH
Similar to open software licenses, developers have the opportunity of choosing from more than one available license. But the transposition of legal aspects of software to hardware isn't straightforward.

At the moment, there are three main hardware licenses available:

- [TAPR OHL](https://tapr.org/the-tapr-open-hardware-license/) - similar to GNU GPL license
- [Solderpad](https://http://solderpad.org/) - similar to Apache license
- [CERN-OHL](https://cern-ohl.web.cern.ch/) - its most recent version (v2.0) has three variants:
          - A strongly-reciprocal variant, CERN-OHL-S
          - A weakly-reciprocal variant, CERN-OHL-W
          - A permissive variant, CERN-OHL-P

We reproduce below an extract from Murillo et al (2019){footcite}`luis2019open` that provides a very complete background on the emergence of licences for open source hardware, and fully recommend reading the full report for those interested in the topic:

> To address the challenge of establishing a solid legal framework for OH, the legal scholar John Ackermann, with the help of the FOSS expert Bruce Perens, drafted the first reciprocal licence, "Tucson Amateur Packet-Radio Open Hardware licence” (TAPR OHL) in 2007. Created in the context of the HAM radio community for helping hobbyists share hardware designs, TAPR was also introduced to create awareness with respect to the pitfalls of flexible, copyright-based open licensing, such as Creative Commons, for hardware projects.
>
> Two key definitions were introduced with this pioneer licensing effort: the definition of “documentation” which describes the set of design files, engineering drawings, and explanatory text, and that of “product” which refers to the fabricated hardware or parts of distribution kits. The reasoning behind this distinction is that the physical instantiation of a design is beyond the scope of copyright, except for a piece of hardware that embodies an artistic expression (Beldiman, 2018). One of the key contributions of TAPR was to include a provision for patent licensing, extending its role to a fundamental
part of the “copyleft” mechanism in the licence by means of a fundamentally a binding contract in which licensor and licensee are granted patent immunity. For the open licensing provisions to be triggered, one must have “active participation in the life of the Documentation or Product” (Ackermann, 2009, p. 208).
>
>[...] In 2011, the European Organization for Nuclear Research (CERN) released the first version of the CERN Open Hardware licence (CERN OHL) as a TAPR derivative. The CERN OHL was motivated by the need for a legal instrument that is tailored for CERN as a publicly funded, multi-lateral research organisation. Key concepts and provisions in TAPR were kept for CERN OHL, such as the notion of “documentation” to establish the scope of what is to be licensed; and, of great importance, the preservation of the copyleft mechanism inspired by the concept of Free Software (Ayass and Serrano, 2012).
>
>The third and last provision kept in the formulation of CERN OHL was the patent licensing clause. In collaboration with the IP expert Myriam Ayass from the Knowledge Transfer group at CERN, the OHL was
designed primarily for transposing reciprocal provisions in the GNU GPL to the domain of hardware. In the words of Ayass’s co-author, CERN engineer Javier Serrano: “we were trying to achieve much more than we had before: the ability for anybody who sees a physical object to trace back to the actual design file [...] We are trying to do reciprocal licensing which is much more powerful than just no-IP” (interview, 05/01/2017).
>
> Another important OH licence was drafted by the legal scholar Eli Greenbaum with a focus on 3D printing: the "Three-Dimensional Printing Open licence" (TDPL). This reciprocal licence draws from other open licences, such a TAPR and CERN OHL, to stipulate provisions for the preservation of attribution and enforcement of access to 3D design documentation. [...] The 3D printing case is of particular interest given its focus on 3D design, which implicate copyright infringement when they are copied (without
authorisation) to the memory of a 3D printer and, then, transformed (sliced) for fabrication. It is this very possibility of triggering copyright restrictions through copying that Greenbaum utilises for establishing the TPDL reciprocal conditions.
>
> In principle, any object could be designed and fabricated, from flower pots to prosthetic devices, whereas copying (and converting) design files to the 3D printer is functionally necessary, generating a "one-to-one correspondence between the digital file and the object that is actually printed" (Greenbaum, 2012, p. 277) with notable differences with respect to the "resolution" which an object will be rendered by the printing equipment. This is not at all the case for other domains of hardware development, where different techniques as well as end results are involved, such as in "gateware" design with programmable logic devices (FPGAs) and application-specific integrated circuit (ASIC) technologies. This is yet another
difficulty with respect to hardware: the very nature of the design, fabrication, testing, and distribution channels varies greatly, introducing serious roadblocks for creating a common framework for hardware sharing.
>
> One of the latest efforts in OH licensing was the “Solderpad licence,” drafted by an attorney with long experience in open licensing, Andrew Katz. In 2010, Katz released a document on a public mailing-list with “tracked changes” on the Apache licence version 2 to create a “permissive” alternative for hardware. His intention was to demonstrate that little modifications would, in fact, be necessary to create a new licence, filling an important gap where reciprocal licences existed, such as TAPR, CERN OHL, and TDPL.
>
> Solderpad introduced a permissive option in the space of strong copyleft licences (Katz, 2012), allowing hardware licensors to extend the possibility of a particular hardware project to be converted into proprietary technology without the obligation of returning improvements and/or derivative versions to the electronic commons of Free and Open Source (software and hardware) projects. [...] The modification of Apache 2.0 text in Solderpad was intended to address the smaller set subset of issues which are relevant in a simple permissive licence. It also included provisions for dealing with patents and trademarks (adopting the Apache 2.0 approach) that are particularly salient in the domain of hardware
(Katz, 2012, p. 54)

## What can be licensed?

{numref}`OSHlicuse-fig` shows that the practices regarding licensing in OSH communities are still heterogeneous. Even when the recommended licences for OSH, recommended by OSHWA, are the three ones mentioned in the previous section, we still find many software and creative commons licences used ({numref}`OSHlicuse-fig`).

```{figure} imgs/38.png
---
scale: 100%
name: OSHlicuse-fig
---
Survey on licences used in OSH communities, 2020{footcite}`oshwasurvey`
```
One reason behind this is that most of the time there is a misunderstanding of what can be licensed and how in OSH. The OSHWA certification program explains these differences by calling to considerate four main components of an OSH project:

- hardware itself,
- software used to run the hardware (if applicable),
- documentation,
- project brand.

As OSH projects contain a mix of different types of material (designs, code, text), you should include multiple licenses, being explicit about which license applies to each part of the project.


```{figure} imgs/35.png
---
scale: 70%
name: iplicence2-fig
---
Multiple components, multiple licences {footcite}`oshwacert`.
```

If you are interested in certifying your project via the OSHWA program or if you want to learn more about how different regimes apply to different project components, we recommend you to visit the [OSHWA Certification Program guidelines](https://certification.oshwa.org/process.html).

## How to choose a licence
Choosing an open-source license for your project involves considering the goals you have for your software or hardware and understanding the implications of different license types. Key considerations include whether your priority is to encourage widespread use and adoption, foster collaboration within a community, or ensure that modifications to your project are shared back with the community.

If your aim is to maximize adoption and use, you might lean towards a permissive license. Permissive licenses, such as the MIT or Apache License for software, or the permissive CERN OHL, allow users to do almost anything they want with your code and designs, including incorporating it into proprietary projects. These licenses offer flexibility and are often chosen for projects with a commercial focus.

On the other hand, if you want to ensure that improvements or modifications to your project benefit the entire community, you might opt for a copyleft license. Copyleft licenses, like the GNU General Public License (GPL) or the strong CERN OHL, require that derivative works also be open source. This ensures that enhancements and modifications made by others are shared with the community.

It is also critical to consider the dynamics of your community and ecosystem. If there are existing projects or standards that you want to align with, choosing a license compatible with those projects can facilitate collaboration. Check the compatibility of licenses to avoid potential conflicts when combining code from different sources.

Think about the level of control you want to retain over the use of your project. Some licenses include clauses that require any modifications or improvements to be contributed back to the community, providing a level of control over the evolution of the project.

Common elements to think about are:

- Attribution: Should/must original authors be attributed or not?
- Derivatives: Are derivatives of the project allowed? and if so, how should/must they be shared?
- Commercialisation: can the project be used for commercial purposes?
- Appliccations: Is the project allowed to be used in any/all domains (e.g. is there text in the license that prohibits use in potentially harmful applications?)

The following tables ({numref}`lictable1-fig` & {numref}`lictable2-fig`, click to enlarge) aim to clarify the differences between licences to facilitate decision-making.

```{figure} imgs/39.png
---
scale: 70%
name: lictable1-fig
---
Main features of recommended OSH licences {footcite}`luis2019open`.
```

```{figure} imgs/40.png
---
scale: 70%
name: lictable2-fig
---
Main features of recommended OSH licences (cont.) {footcite}`luis2019open`.
```

We also recommend looking at the website [Choose a license](https://choosealicense.com/), which provides an interactive orientation guide which now includes licences for hardware.

<embed type="text/html" src="https://choosealicense.com/"  width="100%" height="300px">

## Standards in OSH
The adoption of Open Source Hardware (OSH) by businesses is still low, with most OSH production limited to non-commercial sectors: education, NGOs, academia, hobbyists, grassroots communities in science. Compared to Open Source Software (OSS), with a 30-year delay in development, OSH is still niche.

A key process in growth an expansion is standardization. FOSS counts with standards that are both ​de facto, i.e. adopted in practice by a community but not officially endorsed by a Standard-Setting Organisation (SSO), and ​de jure, ​meaning a specification from a recognised standardisation body​.

The lack of a consistent identity and widely accepted best practices makes defining and standardizing OSH challenging{footcite}`Bonvoisin-2020`. It is difficult to draw a straight line between the practices referred to as OSH and other more or less related practices; “openwashing” discourses from industrial practice{footcite}`lund2020profiting` also contribute to the confusion.

Bonvoisin et al. (2020) describes how the definition of hardware changed with time:

> In the early days of OSH, “hardware” was mainly understood as ​electronic hardware: the hardware on which FOSS would run. In line with this, the first hardware–specific open source license -- the TAPR OHL -- was designed to protect digital telecommunication devices. Since then, the word ​hardware in OSH has acquired a broader meaning, encompassing diverse technologies beyond electronics, such as mechanics or textile.

### Legal aspects & documentation
Counting with a consensuated definition enable the alignment of various standards and a minimun benchmark for compliance. Since 2018 OSHWA provides an **OSH self-certification scheme** based on transparent licensing of parts and products; it is of course aligned with the Open Source Hardware definition.

As a self-certification process that is broadly focused on licensing and aspects of intellectual property, this initiative does not contribute to standardisation of other dimensions of OSH. For example, OSHWA members may ​review the quality of documentation of submitted projects but the criteria used are not formalised, leaving a gap for further standards and certification development.

The community has worked significantly on **standardizing documentation formats**. Examples include DocuBricks, a documentation standard devised specifically for OSH and with a focus on modularity and interoperability - thus enabling different “bricks” with files and instructions to be combined into one project even with conflicting share-alike licenses. Git Building is a recent initiative, yet without major release, which aims to integrate Open Hardware documentations with Git-based version control repositories. Relying on Markup language, it is easily human readable without additional software, at the expense of modularity and machine readability.

Major documentation hosting platforms used by OSH projects do not currently use a documentation or content standard, which may either be due to a lack of development effort or due to the preferences of the largely hobbyist-focused community.

### Towards industry adoption
[DIN SPEC 3105 “Open Source Hardware”](https://www.beuth.de/en/technical-rule/din-spec-3105-1/324805763) is a standardisation effort initiated by Open Source Ecology Germany e.V. and officially launched by the German Standardisation Organisation DIN e.V. (Deutsches Institut für Normung e.V.) April 2019 (DIN 2019). The project was led under DIN’s “Publicly Available Specification” procedure (PAS) delivering a public document that can “be used as a basis for a full standard”. It involves “smaller, more agile working groups” and is an “effective marketing instrument [...] widely accepted by customers and potential partners alike”. It is the first de jure​rather than ​de facto​standard developed for OSH.

This standard contains two parts:

• DIN SPEC 3105-1 “Open Source Hardware - Requirements for documentation” aimed at delivering an unambiguous definition of the term Open Source Hardware based on objective and enforceable criteria.

• DIN SPEC 3105-2 “Open Source Hardware - Community-based assessment” builds upon the definitions provided by DIN SPEC 3105-1 to define requirements for an assessment procedure for OSH products based on reviews by OSH community members -- emulating the model of peer-review used in scientific publishing.

The main contributions of the standard include:
- Breaking down the OSHWA Definition 1.0 into clear, actionable ways to meet that requirement in terms of documentation content,
- Acknowledging that OSH is not only a matter of licensing but also a matter of documentation contents,
- Acknowledging that the content of the documentation to be shared depends on the hardware technologies embedded in the product under consideration (e.g. electronic hardware),
- Acknowledging that the content of the documentation also depends on the audience targeted by the documentation,
- Adopting a product life cycle perspective, considering that “making” a product is not only about manufacturing it, it is also about using, maintaining, updating and processing it at end-of-life.

The first release of DIN SPEC 3015 was published in April 2020. It is the first German standard to be published under an open license (CC-BY-SA 4.0) and to implement an open standardisation process. Viewing and using the standard is thus possible without costly licenses or permission from DIN e.V. or any further restrictions apart from copyleft and DIN’s trademark protection. The open process also provides a mechanism for the OSH community to adjust the standard to their needs in future versions.

### Increasing discoverability
The [Open Know-How Manifest Specification](https://www.internetofproduction.org/openknowhow) is an initiative from the Open Know-How Working Group, who focuses on standardised protocols for the exchange of Open Hardware related information online. The initiative is based on the observation that Open Hardware requires new networks of tools and information in order to ensure that users can find and access appropriate hardware designs, local physical tools to make them, and potentially customers to sell units to.

Established in 2019, it brings together a number of members from academia, NGOs, companies and OSH community groups with the objective of issuing standards to address three levels of sharing documentation information (Know-How) on OSH:

1. discoverability, i.e. the ability to find the documentation regardless of where it resides on the internet, in part through making documentation accessible to web crawlers;

2. portability, i.e. the ability to share documentation on different platforms or to transfer it from one platform to another;

3. platform interoperability, i.e. the ability to update, relate and join documentations across different online repositories and documentation formats.

The first standard released by the working group is the Open Know-How Manifest Specification 1.08 addressing discoverability ​(Open Know How Working Group 2019)​. The working principle of this standard is creating an additional file, called a “manifest”, for each Open Hardware documentation, which contains metadata relative to the documentation and to other files commonly shared next to hardware documentation, e.g. the applying license terms and the “readme” file.

The standard intends to promote discoverability of open source hardware by establishing a machine-readable format which enables search engines and web crawlers to index open source hardware documentation metadata from the internet. A demonstrator of such an index is provided by the working group. It gathers metadata from approx. 400 pieces of hardware and make them available in a single URL9. The manifest file may be written by hand by the authors or it may be auto generated by documentation repositories if the corresponding documentation is sufficiently structured, e.g. in the DocuBricks format, to assess its content automatically. The manifest file links to the documentation and can be thus placed anywhere online, in the documentation repository or in another dedicated location.

The standard delivers a template formatted in YAML markup language which is both machine-readable and easy to modify for non-expert users. The manifest file covers the following metadata:

- basic information such as contact person, licence, language and the locations of (i.e. links to) documentation, bill of materials and project homepage
- descriptive information such as intended use, keywords and development stage
- locations of (links to) some more advanced information such as risk assessments, quality control, or maintenance protocols;
- the ability to make basic relationships between OSH items more transparent e.g. by using "version", "variant-of" and the relationship term “derivative-of” to indicate that the design is derived from another and providing a link to that documentation.

This content makes manifest files fully compatible with the requirements from DIN SPEC 3105. The project has set a goal of 500 OSH projects adopting the Open Know-How Manifests by end of 2020 and is actively recruiting projects to publish a manifest and index it in their demonstrator10. Like DIN SPEC 3105, the standard has been a collaborative effort. It has open channels on the open standard editing platform StandardsRepo11 where feedback and improvements can be suggested by raising an issue or proposal.

The manifest may be the first a series of standards from the Open Know-How Group aimed at building an "Internet of Production", a network enabled by open exchange protocols to locally share and access Open Hardware documentation, as well as needed tools and the information how to use those. This essential infrastructure for Open Hardware may be aided by the creation of appropriate standards which ensure that diverse projects and platforms can exchange information effectively, and to avoid potential vendor lock-ins for the online infrastructure on which the community relies.


## Bibliography
```{footbibliography}
```
