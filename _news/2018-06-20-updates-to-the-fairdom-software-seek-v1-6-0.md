---
title: Updates to the FAIRDOM software (SEEK v1.6.0)
---

**A new version of SEEK is now available, and the FAIRDOMHub has been updated with the changes.** 

Version 1.6.0

_Release date: June 8th 2018_

Integration with NeLS
We’ve been working with ELIXIR Norway to facilitate linking of SEEK with the [ELIXIR Norwegian e-Infrastructure for Life Sciences (NeLS)](https://nels.bioinfo.no/). This interlinking allows Norwegian life scientists the ability to store and compute Bioinformatics data in the NeLS portal, then link and share this data directly in SEEK. This is a leap forward for Norwegian life scientists in ensuring their data is FAIR.

## API

Our JSON API can now support researchers in reading data from SEEK, as well as writing and submitting new entries. 
This allows all users programmatic access to data published in SEEK, as well as for publishing in SEEK. 
The current write support covers Datafiles, SOPs, Models, Investigation, Studies and Assays and linking them together. 
More details about the api can be found in the [API Guide](http://docs.seek4science.org/help/user-guide/api.html). The API will facilitate researchers in embedding SEEK within their day to day data workflows, ensuring better adherance to the FAIR principles.

## Data Upload Workflow and Metadata Wizard

We’ve made some changes to the upload workflow that you will encounter when uploading DataFiles, and developed integrated support for templates that have RightField embedded metadata. Now, the dataFile is registered before additional metadata details are asked for. This allows any relevant metadata in the RightField tab of the DataFile to be read, extracted, and used to auto-populate the upload form where possible. The supported templates are now provided as part of the templates generated for Sample Types, but will soon be available more widely.

The Wizard for uploading DataFile metadata has also undergone a revamp, with it now being split into logical steps that can easily be stepped through.

You can find out more details here [https://docs.seek4science.org/help/user-guide/templates/master-v1.html](https://docs.seek4science.org/help/user-guide/templates/master-v1.html)

and

here: [https://docs.seek4science.org/help/user-guide/data-file-upload-wizard.html](https://docs.seek4science.org/help/user-guide/data-file-upload-wizard.html)

## Creating Assays from the DataFile

Ever got stuck when uploading a DataFile and wanting to link it to an Assay, 
but realising you haven’t created the Assay you want to link it to? Well, 
now Assays can be created and linked to the DataFile being submitted as part of the same process. 
This can either be manual or from the details provided within a template.

## New Document Asset Type

Have you ever wanted to upload a deliverable, report, meeting minutes or other project management document in SEEK, but not felt there was a suitable asset type? We have now created support for a new Document asset type. This allows you to catalogue general documents that do not fit as other asset types.

## Terms and Conditions

When you install and manage your own SEEK, it is important you are also able to provide your users with information about the **Terms and Conditions** that must be accepted as part of the registration process. This is now configurable by Admin of the SEEK installation.

## Simplified DOI creation

We have simplified the interface for creating **DOI’s** for individual items. It is now clearer when looking at an individual item how to mint a DOI for that item.

There have also been many other bug fixes and small improvements. 
A full list of changes included in this release can be found in the [SEEK Change Log](https://docs.seek4science.org/tech/releases#version-160).
