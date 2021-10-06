---
title: "FAIRDOM-SEEK version 1.11.2 released"
---

An update for FAIRDOM-SEEK, version 1.11.2, has been released.

This contains contains some improvements and bugfixes, including:

* Finalised Sample and Sample Type read/write API, along with completed documentation.
* Bioschemas improvements with greater compliance, and the addition of _conformsTo_ clause to indicate which version is
  currently being used.
* Recommended licenses, which appear at the top of the list. The FAIRDOM-SEEK admin has the ability to set and change these under Settings.
  The license ID is now also validated that it is recognised when set through the API.
* Fix to a critical issue with Sample and Custom metadata attributes of type Boolean, which prevented them being set through the UI.
  This also includes a fix to allows an empty value if the attribute is optional.
* Allow project join requests to be approved where the optional Institution Country is missing.
* Show the date a user joined on their profile page, visible to all logged in registered users.

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)