---
title: 'BioHackEU25 report: METRICS - Monitoring of Key Performance Indicators for ELIXIR Services'
title_short: 'BioHackEU25 #15: METRICS'
tags:
  - KPIs
  - ELIXIR Services
  - Metric Measurement
authors:
  - name: Nils-Christian Lübke
    orcid: 0009-0009-4801-9978
    affiliation: 1
    role: Conceptualization, Writing – review & editing
  - name: Helena Schnitzer
    orcid: 0000-0000-0000-0000
    affiliation: 1
    role: Conceptualization, Writing – review & editing
  - name: Julia Koblitz
    orcid: 0000-0002-7260-2129
    affiliation: 2
    role: Software, Writing – original draft
  - name: Sebastian Beier
    orcid: 0000-0002-2177-8781
    affiliation: 3
    role: Software
  - name: Saskia Lawson-Tovey
    orcid: 0000-0002-8611-162X
    affiliation: 4
    role: Writing - original draft
  - name: Kristyna Kvizdova
    orcid: 0009-0000-9827-1359
    affiliation: 6
    role: Writing - original draft
  - name: Séverine Duvaud
    orcid: 0000-0000-0000-0000
    affiliation: 3
    role: Conceptualization
  - name: Manuel Feser
    orcid: 0000-0000-0000-0000
    affiliation: 10
    role: 
  - name: Nicola Soranzo
    orcid: 0000-0003-3627-5340
    affiliation: 7
    role: Writing - review & editing
  - name: Daniel Arend
    orcid: 0000-0000-0000-0000
    affiliation: 10
    role: Conceptualization, Writing – review & editing
affiliations:
  - name: Forschungszentrum Jülich GmbH - IBG-5; de.NBI & ELIXIR-DE
    index: 02nv7yv05
  - name: Leibniz Institute DSMZ-German Collection of Microorganisms and Cell Cultures, Braunschweig, Germany
    index: 2
    ror: 02tyer376
  - name: Institute of Bio- and Geosciences (IBG-4 Bioinformatics), Bioeconomy Science Center (BioSC), CEPLAS, Forschungszentrum Jülich GmbH, 52425 Jülich, Germany
    index: 3
  - name: Centre for Musculoskeletal Research, The University of Manchester
    index: 5
  - name: Earlham Institute, Norwich Research Park, Norwich, NR4 7UZ, UK
    index: 7
    ror: 018cxtf62
  - name: 
    index: 8
  - name: 
    index: 9
  - name: 
    index: 10
date: 7 November 2025
cito-bibliography: paper.bib
event: BH25EU
biohackathon_name: "BioHackathon Europe 2025"
biohackathon_url:   "https://biohackathon-europe.org/"
biohackathon_location: "Berlin, Germany, 2025"
group: Project 15
# URL to project git repo --- should contain the actual paper.md:
git_url: https://github.com/biohackrxiv/publication-template
# This is the short authors description that is used at the
# bottom of the generated paper (typically the first two authors):
authors_short: Nils-Christian Lübke \emph{et al.}
---

# Introduction

More and more research stakeholders asking for Key Performance Indicators (KPIs). Funders want to measure the impact of projects and related services they fund or research organisations want to track the service use for decision making. Service providers themselves are also interested in monitoring their services to gather feedback and improve service quality. KPIs are a simple but powerful tool for these purposes. Additionally, several nodes provided relevant documents in advance which were reviewed and considered during the project.

As part of the BioHackathon Europe 2025, we report on the activities of the METRICS project, which addresses the need for consistent and transparent evaluation of research infrastructure services across ELIXIR and related initiatives using KPIs. The project brings together experts from multiple nodes and domains to identify, harmonize, and semantically model KPIs that reflect service quality, usage, sustainability, and impact. By exploring existing evaluation frameworks and processes, metadata models, and ontological approaches, the team aims to design a flexible yet coherent foundation for KPI monitoring of services. This report summarizes the project’s motivation, current landscape analysis, and initial steps toward developing an ontology-driven framework for KPI representation, fostering interoperability and supporting evidence-based management of life science infrastructures.

## Current ELIXIR landscape
<!--
* As in ELIXIR -> not a lit research
* Leave DFG and NFDI out for the moment
* paragraph interview
-->

The foundation of the project was a comprehensive analysis of the current KPI landscape. Various representatives from different ELIXIR nodes were approached in advance and invited to participate in the project. They were asked to provide insight into known processes, workflows or, if already available, existing KPI sets or guidelines. The information gathered in this process is summarized below.

The following ELIXIR Nodes kindly shared their experiences:

* Germany
* Norway
* UK
* Czechia
* Netherlands
* Ireland
* Spain
* Italy
* ELIXIR Hub

### de.NBI & ELIXIR Germany (Nils)

Within the de.NBI & ELIXIR Germany networks, there are a couple of stakeholders regarding Services and indicator collection. The service providers, based in one of the 24 contractual de.NBI & ELIXIR-Germany partners or at one of the associated sites, are offering their Service via de.NBI & ELIXIR- Germany. Service providers are responsible for running and maintaining the Services. 
Within de.NBI & ELIXIR-Germany the members of the network are scattered across so called "Service Centers". These centers are not clustered geographically but by topic. In every Service Center or at every associated partner site at least one Principal Investigator (PIs) needs to be formally responsible for an offered Service. This is part of the governance structure of ELIXIR-DE Services.
The administration office of de.NBI & ELIXIR-DE offers support efforts and coordinates all services across de.NBI & ELIXIR-DE, e.g. to be displayed on the [website](www.denbi.de). 
Beyond a working group for Service Providers and every interested Person from the network called "Service and Service Monitoring" (SaM-Ag) was established. The group is lead by two PIs from the network and connected to the service coordinator from the administration office.

Discussion about indicator collection, key performance indicator selection, and possible tools to measure them are started and refined by the SaM-Ag supported by the administration office. Results are subsequently ratified by the central coordination unit (CCU), the decision making body of the network. In this way community voices are incorporated in the process, service providers are able to share their thoughts and possibilities, and the administration office can share their thoughts on coordinating the efforts.

In 2021, the first set of indicators and KPIs was published by the network. The SaM-Ag worked out the suggestions, ratified by the CCU.
The list of indicators was divided by the type of Service - database, workflow/pipeline, library/API, consulting service, tool/application - and categorised into "mandatory" and "not mandatory" indicators. 
The mandatory ones need to be collected by a defined time frame - once per month.
The administration office asks for the KPIs from the Service Providers and does annual "check-ups" of the service. These check-ups evaluate general data of the service:

* All known persons are still responsible for the service.
* The service team is responsive -> test mails to publicly available contact email address. 
* The service is still running and used.
* The website of the service on the de.NBI website is still up-to-date.
* All links are functional.

The full set of listed KPIs can be found [here](https://www.denbi.de/images/Service/20210624_KPI_Cheat_Sheet_doi.pdf) or on Zenodo. These KPIs are all quantitatively measured.


Mandatory indicators are mostly centered around user interest -> visits, downloads, unique users.
That being said, "user interaction" would be a good profile to work with, but is incredible hard to collect. There is a user feedback survey, which results can also be incorporated into a general self-assessment scheme for service providers and their service. 

Main KPIs collected are - number of:

* #Actions
* #Citations
* #Downloads
* #Support tickets
* #Unique Users
* #Users 
* #Visits 

KPIs might be differently defined or measured depending on the type of service. Not all "mandatory KPIs" apply for all kinds of Services. 
All KPIs should be measured without "robot hits" being counted.

Turning to the tools used to measure and collect the indicators, the de.NBI & ELIXIR-DE network relied on their service providers' suggestions. The network's community brought their already used tools into the discussion. Hence, some indicators and KPIs are measured or are recommended to be measured with different tool possibilities - e.g. Matomo or Google as Web analytics. 


### ELIXIR Norway (Espen)

ELIXIR Norway collects and monitors KPIs to evaluate the usage, impact, and perfomance of its national services. For the first implementation phase, a core set of primary KPIs has been selected to establish a consistent monitoring baseline across Norwegian services. These include:

* #Unique visitors (nb_uniq_visitors)
* #Visits (nb_visits)
* #Downloads (nb_downloads)
* #Actions (nb_ actions)
* #Page views (nb_pageviews)
* #Actions per visit (nb_actions_per_visit)
* #Average duration (avg_time_on_site)

A set of secondary KPIs, such as returning users, new users, returning visits, new visits, and outlinks, will be introduced in subsequent iterations to provide deeper insights into user engagement and behaviour.

A special KPI, Users (nb_users), requires enabling User ID tracking in Matomo. This measure allows a more precise understanding of user activity but also involves managing unique identifiers (e.g. usernames or email addresses) and therefore most comply with GDPR regulations. 

A dedicated session at ELIXIR Norway's All Hands Meeting was organised to discuss the further development of an automated review process and a monitoring system within NeLS (Norwegian e-Infrastructure for Life Sciences) to support continuous data collection. KPI statistics, including service uptime, are already being gathered. 
The meeting also addressed how parts of the KPI monitoring could be connected to openEbench.

### ELIXIR-UK (Nicola)
ELIXIR-UK captures KPIs when services apply to be an ELIXIR-UK service. There are usually 1 or 2 calls for applications per year; service providers, through a [form with free-text questions](https://docs.google.com/forms/d/e/1FAIpQLSeGfxmEMitfEDXAx3GJCN7NPipxF7OYdEOIFWZ6_MCKIFsqGw/viewform ), describe various service KPIs and vital information for ELIXIR-UK to assess whether the service should be accepted as an ELIXIR-UK service. These applications are then reviewed by ELIXIR-UK's Scientific Development Group (SDG, a committee including domain experts from UK and other ELIXIR Nodes) before acceptance and onboarding as an ELIXIR-UK service [@citesAsRelated:Hancock2017].

Key KPIs captured:

- **Service KPIs** (e.g. usage numbers, uptime) - applicants define their own metrics to showcase their service's relevance within its field.
- **Evidence of community adoption** - this includes KPIs such as number of citations and users, if the service has been mentioned/adopted in projects, and the number of installations or submissions. These KPIs should be comparable to similar ELIXIR services.
- **Connections & collaborations** which includes:
    - *ELIXIR services* - is the service registered on or does it use existing ELIXIR services (e.g. bio.tools, TeSS)?
    - *Is the service connected to other platforms/projects, including ELIXIR platforms?*
    - *How does the service align with the ELIXIR Scientific Programme?*
    - *Does the service collaborate with any ELIXIR communities and/or 'external' partners in the EU and beyond?*
- **Service sustainability** - to ensure the service will be maintained and sustainable in the long-term, applicants provide indicators on the current service funding, including length of time, and any submitted or planned funding applications.

Key issues surrounding KPIs experienced by ELIXIR-UK:
- **What is an ELIXIR service?** - this is not well defined and is therefore difficult to measure KPIs in a structured and systematic way (e.g. software vs training service).
- **Limited resource and capacity** - whilst KPIs are captured when services apply to be an ELIXIR-UK service, there is not currently the time or resource at a Node-level to regularly monitor ELIXIR-UK service KPIs. A re-review of an existing service by the UK Node Office or by the SDG may be initiated in response to reported issues with the service.

### ELIXIR Czech Republic
The interim KPIs evaluation for Czech infrastructures follows the methodology (Methodology for international peer-review assessment of large research infrastructures of the Czech Republic) published by Ministry of Education, Youth and Sports. 

The KPI portfolio complies with RACER criteria but services do not need to provide all KPIs. The RACER criteria are as follows:
- **Relevant** (i.e. closely linked to the objectives of large research infrastructure over a particular period of time)
- **Accepted** (i.e. adopted by the large research infrastructure and Ministry of Education, Youth and Sports, otherwise there would be a limited implementation)
- **Credible** (i.e. unambiguous and easy to interpret to non-experts)
- **Easy to monitor** (i.e. gathering of the data collections should be possible at low cost)
- **Robust** (against manipulation, etc.)

The portfolio of KPIs fixed for the international peer-review assessment includes a set of 13 KPIs such as #user requests for access, #users served or # publications.

Besides these KPIs, the following metrics are also monitored:

- **Summary analysis of R&D and innovation results reached by the operator** (Excellent Science (publication); Applications (non-publication))
- **Summary analysis of R&D and innovation results reached by the users (open access)** (Excellent Science (publication); Applications (non-publication))
- **Summary analysis of LRI's user community in terms of share of domestic and foreign users**

Expenses, FTEs, services and users, number of events and tramping metrics are also being monitored.


### ELIXIR-NL
In ELIXIR-NL, there is an ongoing effort to create a Research Software Directory to measure the maturity of Dutch research software projects and services. This directory will allow ELIXIR-NL to assess whether software is [FAIR](https://www.nature.com/articles/s41597-022-01710-x) and open, and GitHub KPIs can be used to support this. There is also some overlap between the directory and [OpenEBench](https://openebench.bsc.es).

Currently, ELIXIR-NL is reaching out to universities and university medical centres to ask about the software tools they use. Additionally, ELIXIR-NL does already capture KPIs on services that form part of their national health and life sciences data infrastructure.

***MIJKE to provide more info***


### ELIXIR-IE
ELIXIR-IE have a template for service selection in place. This template does not currently capture KPIs, but there are ongoing discussions around this. 

Key issues surrounding KPIs experienced by ELIXIR-IE:
- **User and service provider fatigue**

***MORE from Gavin?***


### ELIXIR-ES

ELIXIR-ES initially collects service KPIs when services apply to be an ELIXIR-ES service. Some key KPIs are also collected roughly every three years to support the Scientific Advisory Board in reviewing ELIXIR-ES services.

Key KPIs collected:
- **Service KPIs** - these are open to the service provider to provide but can include indicators such as unique users per year, number of downloads, data traffic, etc.
- **Connection to ELIXIR** - how is the service connected to ELIXIR platforms, communities, focus groups, or ELIXIR commissioned services?
- **Sustainability** - how is the service funded and for how long?

An important factor when ELIXIR-ES is collecting KPIs is the workload this places on service providers. They try not to ask too much of the service providers, and do not always ask about KPIs, hence the decision to ask for KPIs roughly every 3 years.


### ELIXIR-IT

ELIXIR-IT is the home of [Apicuron](https://apicuron.org/) which is already used as a collector and dashboard of curation activites within and beyond the ELIXIR network. Apicuron collects the following KPIs:
- Number of unique contributors
- Number of contribution events
- Date the resource started using Apicuron (to help justify any gaps in historical data)
- Last activity by the resource (to show consistency in reporting and activity of the resource)

In the longer-term, they would like to incorporate more service KPIs into Apicuron.

### ELIXIR Hub
The ELIXIR Hub has several resources which could capture various service-related KPIs. These are:
- The **Service Delivery Plan** (SDP) which is reviewed by the ELIXIR SAB before publishing.
    - The [Service Selection process](https://elixir-europe.org/platforms/interoperability/guides/node-service-selection-process) provides some guidance on indicators nodes may consider when selecting services.
- **ELIXIR-specific resources** (all peer reviewed)
    - [Deposition Databases](https://elixir-europe.org/services/tag/elixir-deposition-databases)
    - [Core Data Resources](https://elixir-europe.org/platforms/data/core-data-resources)
    - [Recommended Interoperability Resources](https://elixir-europe.org/platforms/interoperability/rirs)

The ELIXIR Hub shared their perspective on streamlining administrative and coordinative efforts regarding Service portfolio management. 
Services are submitted to be ELIXIR-Services via the Service Delivery Plan (SDP). Every Node is mandated to submit an SDP to the ELIXIR Hub. A SDP is a key element of the collaboration agreement every Node needs to sign to be a member of ELIXIR. Further, the ELIXIR network and all of its members do have a mutual interest to offer Services of good quality to the research community.
Every SDP from every given Nodes needs thus to be run by ELIXIR strategic advisory board. If the review is successful, the Node’s services will be incorporated into the ELIXIR Service list.
Once a year, Nodes need to fill a document reviewed by the [collaboration agreement oversight group (COG)](https://elixir-europe.org/about-us/governance/collaboration-agreement/oversight-group). The document currently also asks about possible changes in the Service list of the given Node.
The Hub is also trying to establish Service portfolio management. Hence, the Hub is in favor of a streamlined approach to KPIs provided to all Nodes and all Service providers within the Nodes. 


**ELIXIR Community Databases**

There are ongoing discussions within ELIXIR to create an ELIXIR Community Databases (ECD) concept to support the visibility and co-development of ELIXIR data resources which aren't categorised as Common Data Resources (CDR) or ELIXIR Deposition Databases (EDD). This ECD process will aim to help non-CDR/EDD resources to mature and potentially strengthen a resource's eligibility for CDR/EDD accreditation.

Part of this planned process includes collecting key data resource KPIs to grant a database provisional ECD status. A simple self-assessment check-list collects the relevant information:
- Basic information on data resource uniqueness, relevance to ELIXIR communities, and related publications.
- Time data resource has been live
- Resource involvement in ELIXIR workplans/projects/workshops etc.
- Whether the resource already has service KPIs in place,  including uptime, monthly users, response time
- Sustainability - including funding to cover staff and hardware, the N of staff that would halt development/support if they left the project, plans for long-term storage/back-up
- Indicators to signify how FAIR the data resource is


After 1 year, KPIs monitoring resource uptime will be used to complete a 1-year health check on the resource. These uptime KPIs will be used to assess whether to grant a database full EDC status or not. Future health checks using KPIs will be conducted at the 3-year mark.



## Ontologies on KPIs for research infrastructures

Ontologies offer a powerful means to formally describe and connect Key Performance Indicators (KPIs) across diverse research infrastructures. By providing a shared vocabulary and explicit semantics, they enable interoperability between heterogeneous systems, comparability of service metrics, and integration of monitoring data with other knowledge sources. Although several ontologies for KPIs exist in domains such as business intelligence or smart systems [@citeAsRelated:KPIOWL], none currently capture the specific context of scientific service infrastructures—where services range from data repositories and web tools to computational workflows, each with distinct evaluation criteria. 

To address this gap, a domain-adapted ontology is needed that models not only KPIs and their relationships to services, but also the underlying data collection methods, temporal aspects, and user perspectives. Such an ontology would establish a common framework for transparent, evidence-based evaluation of research infrastructure performance and impact.

The recently developed NFDI-core ontology [@citesAsRelated:NFDIcore] provides a valuable foundation for this effort, as it models key concepts of research infrastructures and can inform the design of a KPI ontology. However, its focus lies on describing the structural and organisational aspects of infrastructures rather than on defining measurable indicators or performance relationships. Therefore, while NFDI-core serves as an important conceptual reference, a dedicated KPI ontology is needed to capture the quantitative, temporal, and evaluative dimensions of service monitoring in a more granular and operational way. 

# Mid-term
## Mid-term report poster
On Day 3 of BioHackathon Europe 2025, we presented our mid-term project poster. We covered why our project is important, our achievements so far, and our future focus. 

By Day 3 we had:
- Interviewed representatives from 10 ELIXIR nodes and the Hub;
- Created a strategy for progressing the project;
- Started mapping service KPIs (to create an ontology).

Most importantly, we asked the community for help. BioHackathon participants from different communities and nodes gave us their suggestions for KPIs we should include in our project and were invited to fill in a survey, to gather more information about their KPI knowledge and current practices.

![20251105_172248](https://hackmd.io/_uploads/BkYJhkqJ-g.jpg)

## Survey to evaluate interest in indicators

Survey data were collected during the Biohackathon week, and the survey remains open for further responses with analysis ongoing. The survey aimed to gather information about participants' interest in and knowledge of KPIs. Responses were analysed to identify levels of awareness, familiarity, and perceived relevance of KPIs within the ELIXIR community.

## Survey Results
A total of 30 responses were received with participants representing 7 ELIXIR Nodes. The survey remains open for additional contributions.




1. Involvement in KPI-related activities
![1activities](https://hackmd.io/_uploads/BkujjNqyWl.png)

*Two thirds* of respondents are involved in activities that are evaluated using KPIs, meaning *one third* of respondents are not.

2. Knowledge and understanding of KPIs
![2Knowledge](https://hackmd.io/_uploads/H1UPhNqJ-x.png)

*47%* said they think they are **not** well-informed about KPIs, including what they are, and how to collect and evaluate them, while *53%* felt that they were well informed.

3. Awareness of KPI tracking tools

Despite over *50%* responding they are well-informed about KPIs, only *47%* said they knew of tools to track KPIs. 

When asked to list the tools they knew, participants listed: Scorpion, Matomo, Google Analytics, Excel, Google Scholar, OpenAlex, specific website KPI features (e.g. on bio.tools), the de.NBI and NFDI guidance for KPIs, and some self-developed tools.

4. Tracking of ELIXIR activities using KPIs

*50%* said they did not track their ELIXIR activities with KPIs, while *40%* did. *3 respondents* gave 'other' responses and described partly using KPIs on their main projects, tracking deliverables, and tracking KPIs via de.NBI.

The *40%* who said they did track their ELIXIR activities with KPIs were asked to give examples. These examples fell into several categories: 
- **Selected ELIXIR services** - either at a node, tool, or life science community level
- **National services and node KPIs** - including node performance, services part of national infrastructure
- **KPIs linked to existing ELIXIR initiatives** - such as the ELIXIR Impact toolkit, the Core Data Resources, and the Recommended Interoperability Resources. 

There were also some examples of the specific KPIs collected:
- **Service KPIs** - N of users/downloads/integrations/page visits, service uptake/usage, issues, user activity
- **Funding** - cost
- **Impact** - service impact (including N of citations), service use in training events & materials, involvement in consulting, environmental footprint

5. Node affiliation
Responses were received from participants affiliated with *7 Nodes, including ELIXIR Germany, ELIXIR Netherlands, ELIXIR Switzerland, ELIXIR Czech, ELIXIR France, ELIXIR UK, and ELIXIR Italy*. 

## Summary and Observation

During the project, it has become apparent that the KPI landscape in ELIXIR, as well as within the institutions in the nodes themselves, is highly fragmented. For example, ELIXIR-DE, ELIXIR-Norway or ELIXIR-CZ have already defined KPI sets that are, in some cases, very comprehensive and concrete, while others only record KPIs very loosely and without clearly defined descriptions. Also when having the way of measuring KPIs we saw that there are already some technicla solutions available, but with different mat

### KPI Sheet

After collecting all information during the first 2 days of the project, we set-up a Google Sheet to create a comprehensive list of all KPIs. The sheet is separated into the different nodes and captures the name of the KPI and its definition, alongside additional relevant information such as the type of indicator (qualitative/quantitative), the type of measurement and if its a mandatory or optional KPI. The condensed document was shared and reviewed by all attendees of the project. The idea was to use this overview to identify potential overlaps of collected KPIs across the different nodes, as well to define potential service categories and KPIs which are relevant for a dedicated category.

### "Tool Overview" (working title)


#### Scorpion

For collecting indicators in dashboard-like manner, the [Scorpion tool](https://scorpion.bi.denbi.de/) was introduced. Scorpion was developed for [Nationale Forschungsdaten Infrastruktur](https://www.nfdi.de/?lang=en) to support the collection of indicators and key performance indicators (KPIs). Networks can agree on a set of indicators or KPIs to be incoporated as templates in Scorpion. Service Provider subsequently share their collected indicators - either manually entered or automatically included - with the tool. With this approach using Scorpion informed decision making is promoted.

#### Webanalytics 

* Google Analytics 
* Matomo

#### others

# "Paragraph for the end" (working title)
## Ontology development

![A first schema of the proposed research infrastructure metrics ontology (RIMO)](https://hackmd.io/_uploads/rJ4H_XckZx.png)


## KPI collection
## Summary of "interviews/dialogues"



# not defined where to put yet

* Collaborative Sheet with list of KPIs
* inital mapping of overlaping KPIs --> Basis for ontology





# Outlook or continuing work

* Maybe guided interviews during an elixir event
* reach out to tech group
* reach out to nodes
* unclear time frame/ time schedule

## Acknowledgements

@all please add your funding or whatever acknowldegments

This work was performed during the ELIXIR BioHackathon Europe 2025 organized by ELIXIR in November 2025. 

SLT is supported by the National Institute
for Health and Care Research (NIHR) Manchester
Biomedical Research Centre (BRC) (NIHR203308).

SB was funded by ELIXIR, the research infrastructure for life-science data and by the Federal Government of Germany and the county of North Rhine-Westphalia (de.NBI - the German Network for Bioinformatics Infrastructure)

This work was supported by the German Research Foundation (DFG) within the project “Establishment of the National Research Data Infrastructure (NFDI)” in the consortium FAIRagro (www.fairagro.net, project number 501899475) and NFDI4Biodiversity (www.nfdi4biodiversity.org, project number 442032008).

## References

NFDIcore: https://doi.org/10.48550/arXiv.2410.01821
KPIOWL: https://doi.org/10.1016/j.ijinfomgt.2019.10.003
EDAM: https://doi.org/10.7490/f1000research.1118900.1
de.NBI KPI Cheat Sheet:https://doi.org/10.5281/zenodo.6597826
Hancock2017: https://doi.org/10.12688/f1000research.10473.2



























--- 

# Formatting

This document use Markdown and you can look at [this tutorial](https://www.markdowntutorial.com/).


## Tables

```markdown
Table: Note that table caption is automatically numbered and should be
given before the table itself.

| Header 1 | Header 2 |
| -------- | -------- |
| item 1 | item 2 |
| item 3 | item 4 |
```

This gives:

Table: Note that table caption is automatically numbered and should be
given before the table itself.

| Header 1 | Header 2 |
| -------- | -------- |
| item 1 | item 2 |
| item 3 | item 4 |

## Figures

A figure is added with:

```markdown
![Caption for BioHackrXiv logo figure](./biohackrxiv.png)
```

This gives:

![Caption for BioHackrXiv logo figure](./biohackrxiv.png)

Figures can be scaled by adding the width or height to the Markdown like this:

```markdown
![Caption for BioHackrXiv logo figure](./biohackrxiv.png){ width=50px }
```


# Citation Typing Ontology annotation

You can use [CiTO](http://purl.org/spar/cito/2018-02-12) annotations, as explained in [this BioHackathon Europe 2021 write up](https://raw.githubusercontent.com/biohackrxiv/bhxiv-metadata/main/doc/elixir_biohackathon2021/paper.md) and [this CiTO Pilot](https://www.biomedcentral.com/collections/cito).
Using this template, you can cite an article and indicate _why_ you cite that article, for instance DisGeNET-RDF [@citesAsAuthority:Queralt2016].

The syntax in Markdown is as follows: a single intention annotation looks like
`[@usesMethodIn:Krewinkel2017]`; two or more intentions are separated
with colons, like `[@extends:discusses:Nielsen2017Scholia]`. When you cite two
different articles, you use this syntax: `[@citesAsDataSource:Ammar2022ETL; @citesAsDataSource:Arend2022BioHackEU22]`.

Possible CiTO typing annotation include:

* citesAsDataSource: when you point the reader to a source of data which may explain a claim
* usesDataFrom: when you reuse somehow (and elaborate on) the data in the cited entity
* usesMethodIn
* citesAsAuthority
* citesAsEvidence
* citesAsPotentialSolution
* citesAsRecommendedReading
* citesAsRelated
* citesAsSourceDocument
* citesForInformation
* confirms
* documents
* providesDataFor
* obtainsSupportFrom
* discusses
* extends
* agreesWith
* disagreesWith
* updates
* citation: generic citation