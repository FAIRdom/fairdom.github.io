---
title: Increasing plant data findability and MIAPPE
---

## EOSC-Life and Plant A+ Demonstrator

The collaboration began with supporting the [Plant A+ Demonstrator](https://www.eosc-life.eu/d8/)
from [EOSC-Life](https://www.eosc-life.eu/). The objective of the Plant A+ project is to cross data from different
domains: phenomics, genetics and environmental data and develop tools to integrate, analyse and visualize these data in
a FAIR manner, and aims to improve data harmonisation and standards to better re-use and integrate existing data in
plant science. For this they chose to use [FAIRDOM-SEEK](/fairdom_framework).

This initially involved extending FAIRDOM-SEEK to
support [Minimum Information About a Plant Phenotyping Experiment (MIAPPE)](https://github.com/MIAPPE/MIAPPE) metadata
within the [ISA](https://isa-tools.org/) structure. This was provided by joint development between **FAIRDOM**
and [INRA-URGI](https://urgi.versailles.inrae.fr/) to add what we called "_Custom Metadata_".

Very similar to the Samples, Custom Metadata allowed FAIRDOM-SEEK entities to have their metadata extended with
key/value pairs, controlled by metadata types that can be validated, and set as required or optional. Custom Metadata for MIAPPE were specified and
applied to the Investigations and Studies, along with an Excel template to populate multiple Studies as a batch process. 
Support for ontology based controlled vocabularies, derived from the [Ontology Lookup Service (OLS)](https://www.ebi.ac.uk/ols/index), 
was also added, for both Sample metadata and the Custom metadata extensions.

{% include image.html file="collaborations/plants-miappe/custom-metadata.png" alt="MIAPPE Custom Metadata" click=true %}

The Custom Metadata was designed to be generic and be reused to support other standards beyond MIAPPE and extend the
metadata of any FAIRDOM-SEEK entities beyond those related to ISA. This was included in
the [1.11.0 release](news/2021-06-23-fairdom-seek-version-1-11-0-released) of FAIRDOM-SEEK, and is being reused
within [DataHub](/Datahub) and explored for other use-cases. There are plans to add a user interface for FAIRDOM-SEEK
administrators to define their own Custom metadata extensions.

Overall ...

* Custom Metadata
* Possibility to add any Metadata Scheme
* Default configuration for MIAPPE Investigation and Study
* Configurable with other scheme in the future
* Batch registration of Studies though an Excel template  
* Ontology based Controlled Vocabularies from OLS

## Increasing Plant data findability and reuse beyond ELIXIR

The work continues with the ELIXIR implementation
study [Increasing Plant data findability and reuse beyond ELIXIR](https://elixir-europe.org/about-us/commissioned-services/increasing-plant-data-findability)
.

We will be extending the MIAPPE support in FAIRDOM-SEEK to
include [Observed Variables and Observation Unit](https://github.com/MIAPPE/MIAPPE/tree/master/MIAPPE_Checklist-Data-Model-v1.1)
. The Observed Variable corresponds to an ISA Assay, and will be linked to the Study through the MIAPPE Custom Metadata.
These are important for [Plant Breeding API (BrAPI)](https://brapi.org/) compliance.

The work will also improve interoperability between FAIRDOM-SEEK, [COPO](https://copo-project.org/), and
the [ISA-Tools](https://isa-tools.org/), and support deposition to data repositories, in particular the
EBI [European Nucleotide Archive (ENA)](https://www.ebi.ac.uk/ena/browser/home).


