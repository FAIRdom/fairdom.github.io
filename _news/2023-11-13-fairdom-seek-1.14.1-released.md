---
title: "FAIRDOM-SEEK version 1.14.1 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/platforms/seek) is now available, which is version **1.14.1**

This is a patch release that includes some important bug fixes and improvements:

* Fixed a problem that prevented extracted samples that include links to other samples being successfully registered.
* Fixed an error that was occurring when a sample attrribute PID was inadvertently set to an invalid IRI.
* A fix to some cases where the submit button was always disabled when attempting to "Request membership" to a Project.
* The integration with the Ontology Lookup Service has been updated to use version 4.
* The sample attribute type "Registered Sample (multiple)" has been renamed "Registered Sample List" to be consistent with other types.
* The sample attribute type "Ontology" has been removed, as it was just duplicate of "Controlled Vocabulary". We are looking at ways to distinguish between
  plain CV's and ontology based CV's in the UI.
* Allow a Controlled Vocabulary that has been populated from an ontology via the Ontology Lookup Service to now also allow additional terms to be manually added.


More details about the changes can be found in the [1.14.1 Release Notes](https://docs.seek4science.org/tech/releases/#version-1141).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)