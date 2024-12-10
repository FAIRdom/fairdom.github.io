---
title: BioIndustry 4.0
description: FAIRDOM-SEEK as the metadata store within the BioIndustry 4.0 Data Fabric, supporting decision support systems and
  Digital Twins. 
page_img: fairdom_in_use/bioindustry-logo.png
type: project
---

## Introduction

[BIOINDUSTRY 4.0](https://bioindustry4.hub.inrae.fr/) (_"RI services to promote deep digitalization of Industrial Biotechnology - towards smart
biomanufacturing”_) is a cutting-edge initiative bringing together academia and industry in Europe to shape the future
of industrial biotechnology.

BIOINDUSTRY 4.0 is developing data-driven approaches, exploiting AI to empower novel decision support systems and
[Digital Twins](https://en.wikipedia.org/wiki/Digital_twin), the latter being to better design bio-processes and enable their real-time online control. To complete these
services, BIOINDUSTRY 4.0 is also developing data and metadata standards to generate high quality, interoperable
multi-scale bio-process data, the technical basis for trusted data networks and process analytical devices to provide
real-time online monitoring of bio-processes.

{% include image.html file="fairdom_in_use/bioindustry-digital-twin.png" alt="BioIndustry4.0 Digital Twin" class="
screenshot" %}

By refining these approaches the project aims to empower professionals from academia and industry to collaborate and
push the boundaries of bioprocess design and control – making the biomanufacturing process faster, cheaper, and more
sustainable.

## The role of FAIRDOM-SEEK

An essential part of the project is the seamless collection, movement and querying of data and metadata (both offline
and real-time), which can then be used to train
ML models and be used to influence the Digital Twin. This is described as the "Data Fabric", with FAIRDOM-SEEK acting as
the central metadata store.

FAIRDOM-SEEK is undergoing a number of enhancements to facilitate this, including:

* Integration with the [FAIR Data Station](https://fairds.fairbydesign.nl/) for metadata collection, validation and
  processing.
* Enhancements to the Extended Metadata Support, including addition of attribute persistent identifiers (PIDs).
* Introduction
  of [Observation Units](https://docs.fairbydesign.nl/docs/fairdatastation/template.html#observation-unit) (describing
  instances of observation and measurement) to satisfy the FDS model, and the Bioindustry information model for experiments.
* Enhanced RDF generation to include statements about the extended metadata and samples (where PIDs are available to
  provide the predicate).
* Revisiting the use of FAIRDOM-SEEK alongside an RDF triple store, to produce a knowledge graph and allow SPARQL queries over
  the metadata.

Along with the metadata, data files are also registered as references to entries in the Data Fabric data store, or another
repository. The data may be legacy files, or a reference to a live data stream being monitored by a bioreactor sensor.

{% comment %}
{% include image.html file="fairdom_in_use/bioindustry-fairdatastation-integration.png" alt="BioIndustry4.0 Digital Twin" class="
screenshot" click=true %}
{% endcomment %}

## Funding

This work is funded through the Horizon Europe (HORIZON) Programme’s Research and Innovation Actions (RIA) 2022 call for
next generation of scientific instrumentation, tools, and methods (_HORIZON-INFRA-2022-TECH-01_).

