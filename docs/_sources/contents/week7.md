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

# 7. Emerging business models
A business model is a conceptual framework that outlines how a business creates, delivers, and captures value. It describes the core aspects of how a company operates and generates revenue. A business model typically includes several key components. A value proposition describes the product or service the business offers and explains how it solves a problem or fulfills a need for customers. Revenue Streams detail how the business earns revenue (through product sales, subscription fees, licensing, advertising, or other means) while the cost structure describes the major costs and expenses associated with operating the business.

Business models can vary significantly across industries and are subject to change as companies evolve and adapt to market conditions. For many OSH project, creating a clear and sustainable plan for how an OSH-based business can operate and generate profit is essential for sustaining their work and growth{footcite}`EUanalysis`. A key question here is how firms can articulate sustainable business models that maximize the value of their assets and differentiate themselves from free riders{footcite}`aagerfalk2015software`.

```{admonition} Tip
:class: tip
The free rider problem is the burden on a shared resource that is created by its use or overuse by people who aren't contributing back to the resource. Free-riding in open source communities leads to overworked and underpaid individuals, and eventually to burnout.
```

As usual, the closest successful example comes from FOSS. There are less studies on OSH business models, though they are slowly emerging{footcite}`pujol2019obsessed`. These describe models of companies providing complementary services and products with the paradigmatic example of Red Hat providing support for Linux-based products, or releasing existing proprietary code as open source to boost its profit on a complementary segment. In hardware, complementary assets such as manufacturing, distribution, service, and branding, can become key differentiators. Community benefits are also relevant to extract continuous product improvements aligned with user needs and attracting potential customers{footcite}`dahlander2006man`.

## FOSS vs OSH business models

There are key differences between FOSS and OSH when it comes to business models{footcite}`pujol2019obsessed`.

OSH firms depend on multiple stakeholders for delivering a complex product: design, quality, testing, manufacturing, distribution, servicing. Complex hardware demands both the users and the hardware manufacturers to collaborate during the development process.

The marginal costs in software re-production approach zero, but in hardware the manufacturing costs of the physical artifact can be substantial. Distribution costs are also incurred for delivering the products.

The development of physical components requires that prototypes are distributed across users and manufacturers collaborating together in the hardware development. Building physical hardware entails revisions. Diffusion and implementation costs in OSH are generally higher and increase commensurately with product complexity and specificity of the installation.

The costs incurred in both OSS and OSH are related to the loss of property rights, a loss that makes realizing an economic return on the private investments impossible. Initial R&D investments for developing a first beta version in OSS can vary from low to high. OSH projects with high product complexity are initially significant compared to OSS. This requires effective incentives for developers to join the open development of the hardware, emphasizing stability of technology (standards) as well as profit-realization opportunities for participants.

## SMEs: strategic approaches
Research from the OpenNext project with OSH Small and Medium Businesses has found a set of six approaches. These are commplementary strategies that allow companies to sustain their OSH activities in a commercial sphere.

```{figure} imgs/41.png
---
scale: 70%
name: clonefork-fig
---
Strategic approaches model for OSH SMEs{footcite}`opennext3`
```

**Leverage through communities**    
The community sits at the very core of successful OSH development. Without buy-in from at least a few people (communities can be very small and still have a large impact) it is not possible to harness the collaborative dynamics that open source as a concept builds on. Community can leverage mass adoption of a product on even a global scale, and, as a consequence, help a product and brand
become a standard in the industry.

**Crowd- and third-party funding**    
Funding sources can include public funding such as grants and innovation support, which is offered by both private and public/state-run foundations. Given the commons-centered nature of open-source assets it is often easier to fit in with the altruistic frameworks of such pools of money.
Another option is Crowd-funding, where customers and community members alike pay upfront for your product and service. A good example is car manufacturer Sono Motors, who uses open source licenses for their add-ons; their initial crowdfunding campaign yielded over 50 million Euros in 2019 (see https://www.seedrs.com/sono-motors)

Donations from either private donors (community members, users, future customers, or simply well-meaning and even anonymous donors) or benefactor organizations (aid work organizations, interest groups, political interest bodies, or even activist organizations) are another option. This requires your product to have a clear transformational capacity which could become a central component in the fulfilment of the mission that drives such potential donors.

**Selling hardware products**     
Selling hardware products is the most classic strategic approach in hardware both OSH and traditionally: Make a good product that someone needs and fulfil that need in exchange for money. By open sourcing your product (or parts thereof) you waive the exclusive right to manufacture and
hence opens the floodgates for anyone, including your competitors, to do it alongside you.

**Platforming**      
Platforming allows suppliers of goods and services to connect directly with customers to cut out middlemen and learn about end-users’ needs directly from the source. Owning the platform grants such control that it often surmounts the value of being the entity supplying the goods. Airbnb (https://www.airbnb.com) is the most visible example of platforming business models.

Platforms can take several forms:
- Hubs for interaction for suppliers and receivers of information, goods, and services alike, either with a free (example: Thingiverse, an open platform for designs)
- Classical marketplace approach (example: OpenDesk, a platform of decentralized production)
- Development platforms where users share labour and exercise leadership for shared outcomes (example: Wikifactory, which connects makers, engineers, and industry manufacturers in shared product development)

A large strand in platforming takes the form of information hubs and forums for the sharing of knowledge and insights among peers. Many platforms even include a combination of these three main functions.

**Ecosystem infrastructure**     
Digging one or several layers deeper than the Platforming strategic approach, the Ecosystem infrastructure strategic approach focuses on providing key enabling services or resources for users in
a relevant ecosystem or professional industry in order for them to thrive: Making life easier for them or helping them do better and have more impact.

Examples include areas such as enabling digital connectivity (example: BRCK, expanding Wi-Fi-connectivity in marginal areas) or creating and distributing educational material that empowers users with information, tools, and even training to realize a shared mission.

It can also take the shape of creating and maintaining repositories of knowledge, blueprints, and
other similar resources, like databases (example: datahub.io, openwb.de).

**Consulting services**      
This is the keystone in the most classic business models of open-source software. By offering the software freely and benefitting from a vast public and ever-growing repository of code, you can customize solutions to your customers and hence add value worth paying for on top of the open-source asset. The very same goes for OSH, because whilst anyone can build and use your product as they please, it takes time to grow the expertise. And in many cases, users and customers will want to skip that learning curve by hiring experts.

Consulting services can include a plethora of activities. The most significant ones tend to be facilitating/hosting workshops, technical consulting either ad-hoc or on a subscription/retainer
basis, co-development of new products with customers, and, lastly, full enterprise solutions.

## Business models in Science

A paper from Joshua Pearce{footcite}`pearce2017emerging` discusses emerging business models in OSH for academic audiences. He distinguishes between business models to serve scientists who also are makers, those who are only users/buyers, and those who are outsourcerers.

**Business Models to Serve Scientists: Makers (Type 1)**     

1. Kit Suppliers      
- *Description:** Firms offer kits containing all non-printed parts ("vitamins") necessary for complex scientific hardware.
- *Example:** Adafruit, known for providing high-quality tutorials for building Open Hardware projects.

2. Specialty Component Suppliers      
- *Description:** Businesses provide custom parts in materials not commonly available for 3D printing, catering to customers who seek specialization.
- *Example:** Shapeways, enabling scientists to order custom-printed Open Hardware components in exotic materials.

3. Calibration and Validation Services       
- *Description:** Firms offer calibration and validation services for Open Hardware components, ensuring tools operate at specification.
- *Importance:** Provides researchers with confidence in the accuracy of measurements and functionality.

**Business Models to Serve Scientists: Buyers (Type 2)**     

1. Selling Libre Hardware       
- *Description:** Firms fabricate and sell hardware with fully documented and freely available designs.
- *Examples:** OpenTrans' $3,000 liquid handling robot, OpenPCR's $649 PCR machine.
- *Business Strategy:** Similar to traditional models; products often sold at a considerable discount compared to proprietary versions.

2. Selling Libre Hardware Services        
- *Description:* Firms sell services, support, and training related to Open Hardware products.
- *Strategies:* Subscription services, support and training, consulting for customized solutions, services to producer coalitions, and support for other Open Hardware firms.
- *Examples:* Red Hat providing services around its FOSS product line, Sparkfun's innovation strategy against cloners.

**Business Models to Serve Scientists: Outsourcers (Type 3)**

- *Description:* Firms offer online services based on Libre Hardware, performing experiments for scientists.
- *Example:* Science Exchange connects core labs with scientists needing experiment services.
- *Benefits:* Provides outsourced access to core facilities, connects labs and scientists, and monetizes the bartering system.

## White Rabbit case study

A research paper by Pujol Priego and Wareham{footcite}`pujol2019obsessed` makes a thorough case study of the White Rabbit project at CERN and the business models associated to it. Although CERN is a very particular case, we do recommend it and briefly describe here the three, complementary business models observed.

**Co-creation model**     
Under this model, the customer purchases WR hardware (product) and integrates the
technology in their experimental setting. This was the prevailing business model applied for the
first uptake of WR in the scientific industry. For instance: “We did feasibility studies and
implemented WR for the European Space Agency to synchronize European Space Agency tracking stations”.

As early adopters of the technology, the engagement of these customers is high, providing peer-to-peer support through feedback, bug reporting and design improvements. This first business model configuration had the effect of expanding the possibility of reusing the design in unexpected, experimental applications.

**Buyer model**    
Under this buyer model, customers come from diverse industry sectors, and they are not engaged in the R&D process of WR, yet they purchase the product of one of the suppliers without any supplementary service.

Within this business model, the customer completes the integration of WR in house. CERN
did not provide user applications, but companies selling the hardware started providing these in the form of starter kits. However, firms are not able to make enough profit.

**Time as a service**       
Under this model, the customer is approached by an intermediary organization (or WR supplier) that produces the product and provides diverse services, which include WR integration into the customer organization. It requires an understanding of a new industry and the specificities of customer needs. Here the margins are typically higher than in the other models and leverage a broader range of creative implementations of the technology in the diverse business settings.

Here, the supplier is not just a WR manufacturing firm but offers consulting, support and services. But due to the uniqueness of each client, and the vast diversity of sectors and business applications of the technology, suppliers are still struggling to “package” or standardize their services around WR.


## Slides for download
[Link to slides]()

## Bibliography
```{footbibliography}
```
