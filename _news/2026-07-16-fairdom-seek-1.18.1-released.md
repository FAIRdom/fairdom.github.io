---
title: "FAIRDOM-SEEK version 1.18.1 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/fairdomseek) is now available, which is version **1.18.1**

This is a patch release that includes some bug fixes and improvements, including:

* Inline document preview, previously only available on Presentation pages, is now also available for SOPs, Documents, Data files and File templates.
* Institution pages now show a link to the full [ROR](https://ror.org/) profile, rather than just the ROR ID.
* SEEK now fails fast with a clear error if the database is unreachable at startup, rather than silently falling back to defaults and causing confusing behaviour.
* Improved database performance for Samples, through additional indexes.
* CSV files with non-UTF-8 encodings are now handled gracefully, rather than causing an error.
* [DataHub](https://fair-dom.org/fairdom-in-use/Datahub) improvements including:
  * Units can now be set, and locked, on attributes in global ISA sample type templates.
  * Fixes to registered Data files, Strains and SOPs not appearing correctly in the experiment view.
  * Fixes to applying Extended Study Templates when creating an Assay.
* [WorkflowHub](https://workflowhub.eu/) improvements including:
  * Updated support for the [RO-Crate](https://www.researchobject.org/ro-crate/) 1.3 specification.
  * Better validation and error handling when adding files to Git-backed workflow versions.
  * A fix to an error that prevented new workflow versions being submitted.
  * `CITATION.cff` files are now validated before being converted to BibTeX.
* Various library and security updates.

There are several more changes, details of which can be found in the [1.18.1 Release Notes](https://docs.seek4science.org/tech/releases/#version-1181).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)
