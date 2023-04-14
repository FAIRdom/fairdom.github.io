---
title: "FAIRDOM-SEEK version 1.13.2 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/platforms/seek) is now available, which is version **1.13.2**

A small patch release that contains several bug fixes and small improvements, including

  * Ability to tag Investigations and Studies, providing better overall consistency
  * Fix duplicate projects appearing in Workflow RO-Crates
  * Sort items by view or download counts in the filtered search index views
  * A new Sample attribute type, Controlled Vocabulary List, that supports multiple terms selected from a Controlled Vocabulary as an array
  * Fix to correctly provide the content length in HTTP headers for downloads that was missing in some cases, and also added the Content-MD5 header to include the md5 checksum
  * Programmes are now listed in MyItems, and related items generally, if the user is the Programme Administrator but not directly a member of a related Project
  * Space out daily background jobs so that they don’t all run at once, avoiding potential memory issues
  * Upgrade of Rails to the 6.1.7.2 version, and also Ruby to the 2.7.8 version


More details about the changes can be found in the [1.13.2 Release Notes](https://docs.seek4science.org/tech/releases/#version-1132).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)