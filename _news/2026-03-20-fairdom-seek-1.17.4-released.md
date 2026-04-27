---
title: "FAIRDOM-SEEK version 1.17.4 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/platforms/seek) is now available, which is version **1.17.4**

This is a patch release that includes some important bug fixes and improvements, in particular:

* Fix to BioModels external search throwing a 404 error in some cases.
* Fix to search indexing of markdown content, to correctly strip out HTML tags.
* Fix to permissions to download Sample type templates, they are now always available if the Sample type is visible.
* Institution departments are now shown when adding a new member to a Project.
* Fix to apply selected attributions when creating a new Data file.
* Fix to SPDX license information not being correctly imported from Workflow RO-Crates.
* Fix to an unexpected nil error during batch delete when using DataHub's dynamic table.
* Fix to include the latest instance name when downloading a spreadsheet from DataHub's single page view.


More details about the changes can be found in the [1.17.4 Release Notes](https://docs.seek4science.org/tech/releases/#version-1174).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)