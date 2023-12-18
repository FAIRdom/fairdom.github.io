---
title: MIAPPE, Plant Data Integration and Findability 
---

## EOSC-Life and Plant A+ Demonstrator

We  actively collaborate with the [EOSC-Life](https://www.eosc-life.eu/) [Plant A+ Demonstrator](https://www.eosc-life.eu/d8/) project providing support to improve best practices and FAIR data sharing in plant sciences. 

The objective of the Plant A+ project is to develop tools to integrate and analyse data from phenomics, genetics and environmental domains and eventually visualize these data in a FAIR manner. As a result, the Plant A+ project chose [FAIRDOM-SEEK](/fairdom_framework) to improve data harmonisation and standards to better re-use and integrate existing data in plant science. This involved extending FAIRDOM-SEEK to support [Minimum Information About a Plant Phenotyping Experiment (MIAPPE)](https://github.com/MIAPPE/MIAPPE) metadata within the [ISA](https://isa-tools.org/). The extension called “Custom Metadata” was jointly developed by the *FAIRDOM-SEEK team* and [INRA-URGI](https://urgi.versailles.inrae.fr/).  

Custom Metadata allows FAIRDOM-SEEK entities to have their metadata extended with key/value pairs, controlled by metadata types that can be validated, and set as required or optional. Custom Metadata for MIAPPE were specified and applied to the Investigations and Studies, along with an Excel template to populate multiple Studies as a batch process. Support for ontology based controlled vocabularies, derived from the [Ontology Lookup Service (OLS)](https://www.ebi.ac.uk/ols/index), was also added, for both Sample metadata and the Custom metadata extensions.

{% include image.html file="collaborations/plants-miappe/custom-metadata.png" alt="MIAPPE Custom Metadata" click=true %}


In summary, during the first phase of support to the Plant A+ demonstrator project FAIRDOM-SEEK was extended to achieve the following:  

  * Custom Metadata
  * Possibility to add any Metadata Scheme
  * Default configuration for MIAPPE Investigation and Study
  * Configurable with other scheme in the future
  * Batch registration of Studies though an Excel template
  * Ontology based Controlled Vocabularies from OLS
 
The Custom Metadata is designed to be generic such that it can be reused to support other standards beyond MIAPPE and be able to extend the metadata of any FAIRDOM-SEEK entities beyond those related to ISA. This was included in [1.11.0 release](news/2021-06-23-fairdom-seek-version-1-11-0-released) of FAIRDOM-SEEK, and is being reused within [DataHub](/Datahub) and explored for other use-cases. 

In future, we plan to add a user interface for FAIRDOM-SEEK administrators to define their own Custom Metadata extensions.


## Increasing Plant data findability for ELIXIR and beyond

Following on, FAIRDOM was included in a successful bid for an ELIXIR implementation study, [Increasing Plant data findability and reuse beyond ELIXIR](https://elixir-europe.org/about-us/commissioned-services/increasing-plant-data-findability), where we will continue to build upon the previous achievements.

For use in ELIXIR and beyond we will be extending the MIAPPE support in FAIRDOM-SEEK to include [Observed Variables and Observation Unit](https://github.com/MIAPPE/MIAPPE/tree/master/MIAPPE_Checklist-Data-Model-v1.1). The Observed Variable corresponds to an ISA Assay, and will be linked to the Study through the MIAPPE Custom Metadata. 
The work will also improve interoperability between FAIRDOM-SEEK, [COPO](https://copo-project.org/), and the [ISA-Tools](https://isa-tools.org/), and support deposition to data repositories, in particular the EBI [European Nucleotide Archive (ENA)](https://www.ebi.ac.uk/ena/browser/home).
