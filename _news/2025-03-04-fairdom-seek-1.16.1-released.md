---
title: "FAIRDOM-SEEK version 1.16.1 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/platforms/seek) is now available, which is version **1.16.1**

This is a patch release that includes some important bug fixes and improvements, in particular:

* Increased the request/response timeout limit for the Docker containers to 5 minutes.
* Fix to avoid an error, and instead warn, when registering items from an HTTPS url with a self-signed certificates.
* Performance improvement when regenerating all RDF.
* RDF export is now in Turtle format instead of RDFXML.
* Better messages when querying Samples in DataHub.
* Support non text based attributes in DataHub's dynamic table.
* UI fix to prevent the title Template being repeated whilst generating a Sample Type template.
* UI fix for displaying some Workflow diagrams that caused an error.
* UI fix for handling tables in item descriptions.
* Several improvements and fixes around support for Observation Units from FAIR Data Station.

More details about the changes can be found in the [1.16.1 Release Notes](https://docs.seek4science.org/tech/releases/#version-1161).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)