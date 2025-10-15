---
title: "FAIRDOM-SEEK version 1.17.1 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/platforms/seek) is now available, which is version **1.17.1**

This is a patch release that includes some important bug fixes and improvements, in particular:

* A minor update to Rails (7.2.2.2) and various libraries for bug and security fixes.
* An update to use the version 2 of the [ROR](https://ror.org/) API.
* Projects can now specify a Scientific disciplines, which can then be used for filtering. The disciplines are defined
  by the [OpenAlex classification](https://help.openalex.org/hc/en-us/articles/24736129405719-Topics).
* There is now a check that creators exist before creating a DOI, notifying the user if missing to avoid an error.
* A fix to prevent errors occurring following the deletion of a Collection avatar.
* UI improvement to allow multiple lines of copyright text to be configured.
* UI improvements to the registration page, when there are 3rd party authentication options configured (e.g. LS Login).
* Licenses are now displayed to also include the short form, which is sometimes more familiar to users.
* Fix to correctly display the preview of the name of a Creator when typing.
* Fix to an incorrect date being displayed when close to a timezone difference.
* Improvements and fixes to manually providing Publication authors, including now searching for registered users
  and better support for pasting a comma separated list.
* WorkflowHub improvements including:
  * Scientific disciplines are propagated from Projects (Teams) to Workflows automatically.
  * Workflow RO-Crate fixes to include datePublished, and removed WorkflowSketch as the type.
* DataHub improvements including:
  * Dynamic Table improvements.
  * JSON-ISA export fixes.
  * Units should be transferred from Templates to Sample Types.
  * Added ISA compliance as a filtering option.
  * Assay stream fixes.
  * Fix for downloading samples as Excel.


More details about the changes can be found in the [1.17.1 Release Notes](https://docs.seek4science.org/tech/releases/#version-1171).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)