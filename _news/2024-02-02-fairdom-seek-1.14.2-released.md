---
title: "FAIRDOM-SEEK version 1.14.2 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/platforms/seek) is now available, which is version **1.14.2**

This is a patch release that includes some important bug fixes and improvements:


* Significant performance improvements for jobs updating the authorization tables.
* Stop displaying usage metrics (views, downloads) from list items, due to a large overhead. The metrics are still available when viewing an individual item.
* Allow users to override http response code validation, but with a warning, when attempting to register and item via a URL - as some servers do not always provide the correct response code.
* Fixes to the BioModels search to better handle unexpected JSON responses, or where information is missing.
* Fix to parsing Excel spreadsheets which have errors reported in the logging, but the errors don't prevent the spreadsheet being successfully parse.
* Keep the "External Search" box ticked between searches.


More details about the changes can be found in the [1.14.2 Release Notes](https://docs.seek4science.org/tech/releases/#version-1142).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)