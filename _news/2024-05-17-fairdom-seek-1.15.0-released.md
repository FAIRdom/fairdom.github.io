---
title: "FAIRDOM-SEEK version 1.15.0 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/fairdomseek) is now available, which is version **1.15.0**

This is a large new version, and highlights include:

* **Licenses** have now been updated to be linked to [SPDX license identifiers](https://spdx.org/licenses/), with support for more open source licences.
* A **sitemap.xml** is generated for all public content, improving indexing by the main search engines, and support for Bioschemas scraping.
* **Duplicate Samples** that occur when extracted from a template are now detected and warning is given.
* **Allowing free text for Controlled Vocabulary** sample attributes, which can be set as allowed for the attribute as part of a defined Sample Type.
* **Controlled Vocabulary performance improvements**, both the user interface and backend, to allow one to be populated from a large number of terms from an ontology.
* **Ontology based Controlled Vocabulary's** can now be populated from **multiple root nodes** of the ontology hierarchy.
* **Performance improvements when deleting items**, especially large numbers of samples deleted at the same time as the source DataFile.
* **Performance improvements** to several of the **background jobs** that run, and also optimisations to the order and priority that they run and number that get created.
* **Automatic approval of Project requests** for the site-managed programme can now be set as a configuration option.
* **[RDA Data Management Plan Common Standard](https://github.com/RDA-DMP-Common/RDA-DMP-Common-Standard) support**, which can now be used to populate a Project.
* **Fix to LS Login** authentication configuration.
* **Generic OpenID Connect** can now be be configured to use as an alternative authentication mechanism.
* **Nested Extended metadata** has had some **UI improvements**, allowing sub sections to be expanded and collapsed and easier to differentiate.
* **Extended Metadata read and write API** has been extended and documented, along with read API's for finding information about the Extended Metadata Types.
* **Wild cards in search queries** are now supported, supporting _'*'_ for a group of characters, and _'?'_ for a single character. e.g _'[?orwe*n](https://fairdomhub.org/institutions?filter%5Bquery%5D=%3Forwe%2An)'_ to match Norwegian.
* **Mysql 8 is now the recommended database** to use, and our default Docker compose files have been updated and tested, together with testing switching existing installations. Mysql 5.7 had an issue with reusing primary keys after a crash, causing some problems in certain scenarios.
* [DataHub](https://datahub.elixir-belgium.org/home/about) is now approaching its first production release, and this version includes two particular hightlights:
    * **Single Page view** for visualising experiments.
    * Creation of **ISA-JSON compliant experiments** using Experiment Sample Templates.
  
... and much more.

More details about what changes are included can be found in the [1.15.0 Release Notes](https://docs.seek4science.org/tech/releases/#version-1150).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html).

Details on upgrading for Docker can be found on the page [https://docs.seek4science.org/tech/docker/docker-compose.html](https://docs.seek4science.org/tech/docker/docker-compose.html). 
We recommend switching to MySQL 8 by updating your [Docker compose file](https://raw.githubusercontent.com/seek4science/seek/seek-1.15/docker-compose.yml).
Whilst it upgrades the mysql database files, there will be a slight delay when it first starts, and will log WAITING FOR MYSQL for longer than usual.