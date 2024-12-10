---
title: "FAIRDOM-SEEK version 1.16.0 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/fairdomseek) is now available, which is version **1.16.0**

This is a large new version, and highlights include:

* **FAIR Data Station Integration** - new work carried out as part of [BioIndustry4.0](https://fair-dom.org/fairdom-in-use/bioindustry4.0) and with contributions from
  [PhenomUK](https://phenomuk.org/) (for improved MIAPPE support).
  [FAIR Data Station](https://fairds.fairbydesign.nl/) provides a lightweight approach to gathering, validating, and ingesting metadata through the use of
  spreadsheet templates and following FAIR principles.
  Current support includes:
    * The introduction of (optional) [Observation Units](https://docs.fairbydesign.nl/docs/fairdatastation/template.html#observation-unit), that fall between Study and Sample in the ISA structure.
    * Ability to import the metadata produced by the FAIR Data Station, following validation of a spreadsheet template. And
      also afterwards should the template change, allowing updated, additions and items moving (but not
      deletion).
    * Allows the registration and updates of the full Investigation, Study, Observation Units, Samples, Assays and
      registration of Data Files.
    * Matches metadata attributes configured in FAIR Data Station with those of pre-configured Extended Metadata Types
      which are then automatically applied.
    * _This is currently an experimental feature_, disabled by default (but can be enabled in the settings), with
      documentation planned, and also automatic creation of Extended Metadata Types, tighter coupling through API's and
      [RO-Crate](https://www.researchobject.org/ro-crate/) support.
* **Explicit Sample Type permissions** - previously, Sample Type visibility was automatically derived according to the
  Projects it is shared with and the visibility of related Samples.
  This has now been updated to allow the permissions to be explicitly defined and under user control. When upgrading
  SEEK
  permissions will be set that mirror the old derived permissions.
* **Fewer constraints on editing Sample Types** - previously, once a Sample Type has Samples created from it, the
  ability to change the attributes was limited.
  This has been relaxed to allow some changes to be made that won't invalidate existing Samples, including adding new
  optional attributes, changing attributes from required to options, the title attribute, the attribute pid and
  description, and changing the name of an attribute.
* **Creating new Extended Metadata Types** - an instance administrator of SEEK can now create new Extended Metadata
  Types through the user interface, using a simple JSON file that defines the type and attributes.
  The JSON has a corresponding [schema](https://docs.seek4science.org/tech/extended-metadata/extended-metadata-type-schema.json) against which it is
  validated. There is new [extensive Documentation](https://docs.seek4science.org/tech/extended-metadata/extended-metadata-type.html) including on
  on how to create, and we are also planning on supporting doing so with an Excel template.
* **Deleting Extended Metadata Types** - in addition to being able to disable, an administrator is now able to delete
  Extended Metadata Types.
* **RDF support** extended to support **Extended Metadata** and **Samples** - RDF generation will now include Extended
  Metadata when present for the attributes that include an identifier, and similarly some basic RDF is generated for
  Samples.
* **[DataHub](https://fair-dom.org/fairdom-in-use/Datahub) enhancements** including
    * Implementation of Assay Streams to group multiple assays that share similar traits like the technology type.
    * Better integration of ISA-JSON compliant items.
    * Improved sample querying using the Experiment Sample Template Attributes.
* **Registering multiple Datafiles via a zip file** - a contribution from PhenomUK, that allows multiple DataFiles to be
  registered at once by uploading a zip file.
* **Search improvements** - to better support non-ASCII characters, such as umlauts and accented characters. Now both
  the original and closest ASCII representation are indexed.
* **COPASI model simulation** - enables the interpretation and manipulation of [COPASI](http://copasi.org/) models
  directly within the SEEK client interface, using [COPASI.js](https://github.com/copasi/COPASI.js).
* **[WorkflowHub](https://about.workflowhub.eu/) enhancements** including
    * Improved support for importing workflows from Github, which is also now configurable and handles versions better.
    * Improved support for RO-Crates, and submitting RO-Crates through the API.

  
... and much more.

More details about what changes are included can be found in the [1.16.0 Release Notes](https://docs.seek4science.org/tech/releases/#version-1160).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html).

Details on upgrading for Docker can be found on the page [https://docs.seek4science.org/tech/docker/docker-compose.html](https://docs.seek4science.org/tech/docker/docker-compose.html).