---
title: "FAIRDOM-SEEK version 1.17.2 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/platforms/seek) is now available, which is version **1.17.2**

This is a patch release that includes some important bug fixes and improvements, in particular:

* A new SPARQL view, that allows SPARQL queries to be made over the public graph directly in SEEK, if running together
  with the Virtuoso triple store.
    * Ability to execute queries and store the URL of queries for later re-use.
    * Configurable set of predefined example queries.
* Added support for registering DataCite based DOIs, in addition to CrossRef based DOIs. Alongside this the list of Publication
  types have been expanded to include those supported by DataCite.
* Fixes related to registering Publications as Bibtex files.
* Fix to the rendering of Publication abstracts.
* Expanded the list of Model types, execution environments and formats to support Machine Learning models.
* Enhanced the schema.org metadata support
    * to include identifiers for DOI, ROR and ORCID
    * added LabProtocol (from [Bioschemas](https://bioschemas.org/types/LabProtocol/0.5-DRAFT)) as a type for SOPs.
    * fixed the JSONLD endpoint to be available for all items that support schema.org metadata.
* Reduced the batchsize when reindexing all items from 250 to 50, and made configurable through `Seek::Config.reindex_all_batch_size`.
* Fix to better handle requesting invalid citation styles. Previously an invalid style would become the default style, leading to subsequent errors.
* DataHub specific:
    * Return to the single page view when cancelling from an items Manage page.
    * Fix propagating permissions to child Assays and Sample types.


More details about the changes can be found in the [1.17.2 Release Notes](https://docs.seek4science.org/tech/releases/#version-1172).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)