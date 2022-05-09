---
title: "FAIRDOM-SEEK version 1.12.0 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/platforms/seek) is now available, which is version 1.12.0


* **Collections** - the ability to bundle together items that are conceptually related into an ordered list, which can
  then be shared together as collection.
* **New customisable front landing page** - a cleaner front page, with more useful information, that can be customized
  and configured per SEEK instance.
* **Sample attributes enhancements** - attributes can be provided a description, which provides more details when
  entering or viewing a sample. They can also be given a persistent identifier, to provide a semantic definition of the
  attributes meaning.
* **Improvements to how creators can be credited** - there is now an improved UI for crediting the creators, or authors,
  of assets. Extra information, such their as ORCID and affiliation, can now be added for each creator, even if they are
  not registered in SEEK. The exact order of how creators appear can also be specified.
* **Explicit ordering of Investigations, Studies and Assays** - each can be provided with an explicit order within the
  other, rather than the order they are added. They can re-ordered at any time.
* **Ability to link a Sample to multiple other samples** - previously, a sample could only be linked to a single other
  sample. This has now been updated to allow a one to many relationship as long as the samples are of the same type.
* **EDAM annotations for workflows** - describe the workflow operations and topics from the EDAM ontology. This is also
  planned to be reused to describe data types and formats.
* **Simpler branding settings** - for SEEK administrators, the settings to give particular branding to an instance were
  complicated and confusing. This has now been simplified, and organised in logical groups.
* **Moved related items into a tab** - the list of related items associated with the item shown have now been moved into a separate tab, rather than needing to
  scroll to the bottom of the page. There are also plans to move other information, such as versions and files, into
  additional tabs.
* **Fixes and improvements running to under a relative URL** - for those running SEEK under a relative URL (
  e.g. https://mysite.com/fairdom-seek/), some issues were found with incorrect links. These problems have now been
  fixed, for both Docker and Bare-metal installations, and the testing process improved.
* **Batch registration of Samples through the API** - it is now possible to register Samples in batches through the API,
  rather than one by one, to reduce the number of necessary calls and performance.
* **Updated to use latest version of Apache Solr** - the Apache Solr that was being bundled with SEEK, was no longer
  being maintained and updated. This locked SEEK to an older version of Java. Solr has now been separated, that can be
  installed separately using the latest version, along with an updated configurations. A new updated Docker image is
  also now available.
* **Workflow API enhancements** updates to support the GA4GH TRS API, allowing one click execution of Galaxy workflows, and support for registering an RO-Crate through the API.
* **Extending the items a workflow can be linked to** - ability to link a workflow to Datafiles (as test, example and training data),
  Documents, SOPs, and Presentations as well as Publications.
* **User defined workflow types** - users can now add to the selection of workflow types, if they can't find the one
  they need, when registering a workflow.


More details about the changes can be found in the [1.12.0 Release Notes](https://docs.seek4science.org/tech/releases/#version-1120).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)