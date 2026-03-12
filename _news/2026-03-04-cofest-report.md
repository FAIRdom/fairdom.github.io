---
title: "Knowledge exchange at FAIRDOM CoFest 2026"
---

![Fairground image](/images/news/fairground-bluegrey-wide.png)

In March 2026, we hosted the first FAIRDOM Collaboration Fest (CoFest) online. Users, developers, leaders and advocates from nine institutions in six countries created an opportunity to collaborate, discuss and progress a range of matters and features which will be of benefit to the wider FAIRDOM-SEEK community. We also welcomed those interested in learning more about FAIRDOM-SEEK and how it could benefit their work.

The mini CoFest format allowed us to discuss and plan upcoming work, without needing to commit any code immediately. We presented two topics, covering a range of concepts and teams.


## Recap of FAIRDOM-SEEK features released in 2025
The session opened with a brief review of the [FAIRDOM-SEEK features released](https://docs.seek4science.org/tech/releases/) since the [Mini Hackathon event we ran in February 2025](/news/2025-03-13-connections-made-at-fairdom-mini-hackathon). 
These include improved support for [FAIR Data Station](https://fairds.fairbydesign.nl/), enhanced Schema.org metadata support, a new SPARQL view, support for DataCite-based DOIs for publications, and improvements to [WorkflowHub](/fairdom-in-use/workflowhub) and [NeLS](/fairdom-in-use/digitallifenorway). 
Such features were possible thanks in part to your contributions at the Mini Hackathon.

## Topic 1: Knowledge Graph and Linked Data
Knowledge graphs are an increasingly useful method for representing research data. 
[FAIRDOM-SEEK](/fairdomseek) can easily be configured to publish a queriable public knowledge graph of all open content, and optionally a private graph of all content.
This project, led by Stuart Owen (University of Manchester) with Xiaoming Hu (Heidelberg Institute for Theoretical Studies) and Phil Reed (University of Manchester), provided a comprehensive overview:

- Introduction to **Linked Data and RDF**, and their benefits
- How FAIRDOM-SEEK supports Linked Data by describing objects using **JERM**-based RDF, **Schema.org** and **Bioschemas** markup, and **JSON-LD**
- How FAIRDOM-SEEK includes **Extended Metadata** and **Sample** properties within the RDF
- How FAIRDOM-SEEK uses the **Sample** bioschemas type, and includes custom properties using **PropertyValue**
- The new **SPARQL view** in FAIRDOM-SEEK, providing access to the **public knowledge graph**, with customizable **example queries**
- A brief overview of the interoperability and integration between FAIRDOM-SEEK and **FAIR Data Station**
- A demonstration of **how to set up** the knowledge graph on your SEEK instance using Virtuoso 
- A look at **how RDF is generated** from a customizable lookup table

The presentation concluded with a look at the future plans for developing knowledge graphs in FAIRDOM-SEEK. Suggested work includes the addition of Schema.org in the knowledge graph, enriching the RDF with external identifier info (ROR and ORCID), and discussing how RO-Crate might be included in the graph. Also under consideration is to include Extended Metadata in the Schema.org markup. These plans are subject to change; please follow the [Roadmap](https://docs.seek4science.org/tech/roadmap) to keep updated.


## Topic 2: Neo4J, Visualization and LLM enabling

The FAIRDOM-SEEK platform enables the building of project hubs where investigators can store, share, access, connect and interact with digital objects generated from their research, and use them in their own analyses.
MIT BioMicroCentre uses a private hub called [NExtSEEK](//fairdom-in-use/nextseek) within the MIT facility to coordinate project management during the running of a project. 
The second topic at the FAIRDOM CoFest was led by Charlie Demurjian (MIT), and described how NextSEEK is developing an agentic team to interpret natural language to query its database. Highlights of the presentation:

- NextSEEK provides **active data management** as a wrapper around FAIRDOM-SEEK.
- Samples in NextSEEK can be **visualized** in a tree, powered by Noe4J. 
- To make something **"LLM Ready"**: separate the work into small agentic tasks, give specific instructions in a workflow, where each agent has concrete input and output schemas and contexts.
- Develop the processes using published data, in this case, 50,000 samples. 
- Start on use cases that are things you can already do on the website, establish a base truth, keep the human in the loop. 
- Work up to queries such as "Build me a GEO Submission for D.SEQ-221031SHA-67-PUB and D.SEQ-221031SHA-65-PUB". NextSEEK Assist can build a [GEO](https://www.ncbi.nlm.nih.gov/geo/) spreadsheet for two given samples. The agents will go up and down the tree to map to the correct fields in the GEO, generate an Excel workbook with strategy, treatment and protocols for the researcher as their starting step. This will make researchers' lives easier.

The presentation concluded with a look at the roadmap for LLM-supported work in NextSEEK. One path is network ingestion (to populate the SEEK database), another is to interoperate with sequencing pipelines (from a repository submission, given sequencing files, run a Nextflow pipeline and bring the results back into SEEK). Many of the approaches and lessons learned could be shared across the FAIRDOM consortium and may apply to other instances of FAIRDOM-SEEK.


## Following up

Slides 

- Main Presentation, Topic 1 -- link TBA
- Topic 2 -- link TBA

Video

- Main Presentation, Topic 1 -- link TBA

If anyone is interested in collaborating with any of the presenters above, please get in touch directly (or [contact us](/contact)). Our next FAIRDOM user meeting will run in early autumn 2026, check back here for details.
