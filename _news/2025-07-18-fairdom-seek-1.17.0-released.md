---
title: "FAIRDOM-SEEK version 1.17.0 released"
image: "images/news/seek-docs-banner.svg"
---

We are pleased to announce a new major version of [FAIRDOM-SEEK](/fairdomseek) is now available, which is version **1.17.0**

This is a large new version, and highlights include:

* A period of maintenance, doing various updates and spring cleaning, including:
    * Rails upgrade to 7.2
    * Ruby upgrade to 3.3
    * Updates of dependencies.
    * Addressing hard to maintain code and cleaning up technical debt.
* Integrated Institutions with [Research Organization Registry (ROR)](https://ror.org/)
    * When either editing or creating, Institutions can be searched via the ROR api and automatically populated.
    * Linking an Institution to an ROR persistent identifier, either through searching or manually.
    * Added a field for Department, for cases where more specific details are needed.
    * Update the API to include ROR details.
    * Institutions can still be registered manually, without ROR, for cases where it is missing from the registry.
* Extended support for [Fair Data Station (FDS)](https://fairds.fairbydesign.nl/)
    * Extended Metadata types and Sample types can now be easily created from an example output from FDS.
    * Asynchronous imports and updates using a background job, with current status displayed, to support large cases which would otherwise timeout.
    * Retaining a history of the FDS files used to import or update.
    * recognises disabled EMT's.
* Further integration with the ELIXIR Norway [NeLS](https://elixir.no/Services-bak/nels) system, to support more features that can be done directly in SEEK:
    * Browsing datasets, subtypes, files and folders.
    * Downloading files.
    * Creating datasets.
    * Creating folders.
    * Uploading files.
    * Updates required to use the latest NeLS API.
* [WorkflowHub](https://about.workflowhub.eu/) enhancements:
    * Git related api and documentation improvements.
    * Updates to the [EDAM](https://edamontology.org/page) controlled vocabularies to synchronise with their latest ontology - for topics, operations, data types and data formats.
* [DataHub](https://fair-dom.org/fairdom-in-use/Datahub) enhancements:
    * Dynamic table fixes and improvements.
    * Improve non-text attributes (e.g. related DataFiles, Samples) in Experiment view.
    * Fix to linking Sample types to Assay Streams.
* Added the ability to edit the title and description for ISA snapshots.
* Where SEEK is used together with a triple store, the RDF registered now correctly sets the data type, e.g. for datetime.
* A rework of exporting a list of publications, with a fix to correctly apply the visible filters applied.
* A configurable maximum number of filters (default 5) that can be applied by anonymous users, to reduce overheads from AI bots.
* Fixes related to deleting contributors.
* Fix to the Restart Background Workers feature available to administrators, as well as clearer indication of what are running and how many there should be.
* Admin feature to list all registered users with profiles.

  
... and much more.

More details about what changes are included can be found in the [1.17.0 Release Notes](https://docs.seek4science.org/tech/releases/#version-1170).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html).

Details on upgrading for Docker can be found on the page [https://docs.seek4science.org/tech/docker/docker-compose.html](https://docs.seek4science.org/tech/docker/docker-compose.html).