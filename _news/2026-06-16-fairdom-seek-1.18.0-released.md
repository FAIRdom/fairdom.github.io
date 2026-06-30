---
title: "FAIRDOM-SEEK version 1.18.0 released"
image: "images/news/seek-docs-banner.svg"
---

We are pleased to announce a new major version of [FAIRDOM-SEEK](/fairdomseek) is now available, which is version **1.18.0**

This is a large new version, and highlights include:

* DOI enhancements:
    * Presentations can now have DOIs minted and retracted, alongside other asset types.
    * Resources with DOIs can now be deleted, with automatic DOI retraction and metadata storage.
    * Publication types are automatically detected when querying DOIs during registration.
* New administrator options:
    * Prevent local file uploads, requiring remote URLs instead.
    * Disable built-in username/password login to enforce SSO-only access.
* Search improvements:
    * Samples are now fully supported in API-based searches and returned in search results.
    * External search adapters can be toggled via the admin settings UI.
    * Search now handles punctuation correctly (hyphens, parentheses, etc.).
* Extended Metadata improvements:
    * Controlled vocabulary attributes can now accept free text when configured.
    * Nested Extended Metadata attributes export as blank nodes in RDF.
    * [Fair Data Station](https://fairds.fairbydesign.nl/) imports correctly reject type mismatches with required fields.
* Events now support event types with hybrid, online, and offline location options, and end date auto-sets to 1 hour after start date selection.
* ISA & [DataHub](https://fair-dom.org/fairdom-in-use/Datahub) enhancements:
    * Temporary sharing links for ISA assets (Investigations, Studies, Assays, Observation Units), providing time-limited access via authorization codes.
    * ISA input tag now available through the API.
    * Global sample type templates can now reference registered assets.
    * Extended metadata fields are now included in spreadsheet exports.
* Workflow enhancements:
    * New workflow versions can be created via [RO-Crate](https://www.researchobject.org/ro-crate/) upload.
    * [Bioschemas](https://bioschemas.org/)/[schema.org](https://schema.org/) properties expanded for workflows, including `creativeWorkStatus`, `contributor`, `citation`, and `datePublished`.
* Multiple security vulnerabilities (XSS) addressed.
* PDF preview rendering greatly improved.

... and much more.

More details about what changes are included can be found in the [1.18.0 Release Notes](https://docs.seek4science.org/tech/releases/#version-1180).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html).

Details on upgrading for Docker can be found on the page [https://docs.seek4science.org/tech/docker/docker-compose.html](https://docs.seek4science.org/tech/docker/docker-compose.html).

**Please note** that this upgrade requires some additional attention in two areas:

* **Solr configuration** — to pick up the search improvements, the Solr configuration needs to be updated. Details can be found at [https://docs.seek4science.org/tech/setting-up-solr#updating-the-solr-configuration](https://docs.seek4science.org/tech/setting-up-solr#updating-the-solr-configuration).
* **Docker Compose** — the compose files follow a new structure, and the Solr service has been updated to use the official Solr image directly, with configuration files now needing to be provided under `solr/seek/conf`. Full details are at [https://docs.seek4science.org/tech/docker/docker-compose#updating-the-solr-configuration](https://docs.seek4science.org/tech/docker/docker-compose#updating-the-solr-configuration).
