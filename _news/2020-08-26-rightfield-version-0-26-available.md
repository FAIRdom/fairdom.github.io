---
title: RightField version 0.26 available

redirect_from:
    - /2020/08/26/rightfield-version-0-26-available/
---

A new version of the [RightField](/platforms/rightfield/) software has been released, version 0.26.

This version includes the following enhancements

* Ability to select invididual terms that will appear within the dropdown list. The previous behaviour forced all subclasses or instances. From the list of terms at the bottom right, multiple terms can be selected by holding down CTRL, or SHIFT to select a range. By default all are selected. Many thanks to Andreas Weidemann for this contribution.
Tooltips are shown to display the term URI when browsing the ontology or selecting terms – this is to help resolves ambiguities.
* Increased the default JVM to 1Gb, and increased the timeout limit when loading ontologies. This provides support for larger ontologies.
Please bear in mind, that for some ontologies you may need to be patient for them to load. For example the EFO ontology can take 2-3 minutes on my laptop.
* An upgrade of all dependencies, and Apache POI in particular.

The new version can be downloaded from [https://rightfield.org.uk/download.html](https://rightfield.org.uk/download.html)

For some details and background regarding running on Mac OS X please see the [Release Forum Post](https://groups.google.com/forum/#!topic/rightfield/iMUeLQsM33o)