---
title: "FAIRDOM-SEEK version 1.13.0 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/platforms/seek) is now available, which is version **1.13.0**

This is a large new version, and highlights include:


* **Maintenance period** - code tidying, removing old unused features, refactoring.
* **Rails 6.1 upgrade**.
* **Workflow support improvements**:
    * **Git** repository support:
        * Import from git repository,
        * Add and modify files dynamically,
        * Preview and download individual files,
        * Versioning via Git.
    * **Bio.tools** integration for workflow steps,
    * **Citation CFF** support,
    * **Jupyter** notebook rendering,
    * **RO-Crate** parsing and creation fixes,
    * Improved workflow **diagram** generation,
    * Workflow **maturity flag** and filter,
    * **LifeMonitor** integration - filter by test status.
* **Sample enhancements**:
    * Extraction performance improvements,
    * Improved error handling and reporting during sample extraction,
    * Sample types have contributor shown, and now supports creators,
    * Filtering and search view now available for samples and sample types.
    * JSON API improvements.
* **Integrated [TeSS](https://tess.elixir-europe.org/) search** for Events.
* **Timezone information** provided for Event start and end dates.
* **Search improvements**:
    * Fix to the order of search results,
    * Improvements to indexing.
    * Harmonization between general search and searching and filtering.
* **Show the last person** that updated an item (shown only to project members).
* **Improvements to the table view** of items, adding more columns and making more consistent.
* **Tagging projects from the EDAM** ontology, and made easier to extend with other ontologies in the future.
* **API testing and documentation** improvements.
* **Project creation and join requests** fixes and improvements, including:
    * Other administrators are notified when a request is responded to.
    * Ability to delete a request without responding, for handling spam or duplicates.
* **Descriptive help text** for each creatable entry, show in the Create or Browse pages that link off to documentation where available.
* **IBISBA enhancements**:
    * iPOP - to populate a Project and ISA information from a spreadsheet template,
    * File templates and Placeholders.
* **Publication improvements**:
    * Option to support the upload of full text PDF or link,
    * Any number of related links,
    * Option to allow editing imported publications.
* **Settings caching** - giving a page load speed improvement
* **Cookie consent banner** improved to give more control over which cookies are set, and when content from other sites can be embedded.



More details about the changes can be found in the [1.13.0 Release Notes](https://docs.seek4science.org/tech/releases/#version-1130).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)