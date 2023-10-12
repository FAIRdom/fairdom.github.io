---
title: "FAIRDOM-SEEK version 1.14.0 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/platforms/seek) is now available, which is version **1.14.0**

This is a large new version, and highlights include:


* **Upgrade of Ruby**, from Ruby 2.7 to Ruby 3.1.
  * This gives improved speed and overall performance, along with keeping up with security patches.
* **Upgrade to Rails**, to the latest 6.1 release.
* **Nested [Extended Metadata](https://docs.seek4science.org/tech/extended-metadata)** (previously referred to as Custom Metadata).
  * Extended Metadata allows items to be customized with additional typed metadata, similar to samples, and was used to support MIAPPE along
    with some bespoke installations.
  * Extended Metadata can now be nested, i.e one Extended Metadata type definition can include a reference to another,
    and these will be nested together in a single form.
  * The inner Extended Metadata type can also now be defined as a list, with the form allowing new items to be added or removed.
* **Gatekeeper behaviour** refresh and fixes
  * Many bugs fixed, along with improvements and refinements.
  * Fixes to notifications for when a gatekeeper intervention is required.
  * Fixes to tracking items waiting to be published, and updating the list when they are rejected or approved.
  * Fix to better keep track of the full sharing permissions whilst a request to make public is being reviewed by the gatekeeper,
    and have them applied correctly when approved.
  * Users can now cancel a publishing request.
  * Added support for Samples.
  * Improved integration with DataHub and the Single Page View.
  * Updated [documentation](https://docs.seek4science.org/help/user-guide/roles.html#asset-gatekeeper).
* **Viewing of Excel files in the browser** for all asset types (previously only Data Files were supported).
* **Event filtering improvements**.
  * Includes the full set of common filters available for other items, plus the addition of Event specific filters.
* **Fix duplications in the ISA graph and tree**, particularly for publications.
* **Updated and unified auto complete text fields** to use an improved UI component and be consistent throughout.
  * Type ahead fields that autocomplete (e.g. tagging, sample controlled vocabularies) have now been updated to use [select2](https://select2.org/) throughout.
* **Programme creation request notifications** to adminstrators are now shown in the browser as well as by email.
* **Explanatory text for Programme creation** has been provided.
* **Navigating from broad search results across all types, to the full list** with filtering for a specific type has been made clearer .
* **Better phone and tablet support** for some places in the UI.
* **[FAIR Signposting](https://signposting.org/FAIR/) support** option added.
  * Data dumps containing aggregated Bioschemas metadata generated daily for each asset type.
* **bio.tools** support extended to API.
* **Workflow metadata improvements**.
  * Automatic identification of license from `LICENSE` etc. files in Git repositories or RO-Crates.
  * Recognize additional metadata from CFF files.
  * Add "Deprecated" as a maturity level option.
* **Citation improvements**.
  * Citations can now be generated from CFF files for resources without a DOI.
  * Citation style select list can now be filtered.



More details about the changes can be found in the [1.14.0 Release Notes](https://docs.seek4science.org/tech/releases/#version-1140).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)