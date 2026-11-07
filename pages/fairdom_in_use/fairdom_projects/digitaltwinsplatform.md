---
title: DigitalTWINS platform 
description: Clinical and home-based healthcare applications from Auckland Bioengineering Institute
page_img: fairdom_in_use/...
type: project
---

## Overview of the DigitalTWINS project

### Project description
The Digital Twins Platform is a common infrastructure that aims to extend and apply the developments of the Physiome Project to clinical and home-based healthcare applications. It brings together a data catalogue, a harmonised data repository (SPARC Dataset Structure), workflow execution and a web portal to make computational physiology and digital twin research FAIR and reproducible.

### Installation and configuration   
The platform is a single Docker Compose project behind an nginx gateway, with Keycloak providing single sign-on. FAIRDOM-SEEK runs as one of its services. See the [architecture](https://github.com/ABI-CTT-Group/digitaltwins-platform/blob/main/docs/architecture.md#digitaltwins-platform-architecture) and [deployment](https://github.com/ABI-CTT-Group/digitaltwins-platform/blob/main/docs/architecture.md#digitaltwins-platform-architecture) guide.

### How the project uses FAIRDOM-SEEK 
SEEK is the platform's data catalogue, describing the research projects, tools and workflows, and who can access them. The Digital Twins Platform API registers items in SEEK and queries it on behalf of the signed-in user, using their Keycloak identity. See the [SEEK integration details](https://github.com/ABI-CTT-Group/digitaltwins-platform/blob/main/docs/seek-integration.md).


## Features

* Keycloak single sign-on for SEEK ("Sign in with Keycloak"), with SEEK accounts and profiles created automatically on first login
* Per-user API access: SEEK accepts Keycloak-issued tokens, so every request runs as the signed-in user and SEEK's sharing and visibility rules always apply.
* Datasets in the SPARC Dataset Structure, catalogued in SEEK, with import via the platform's APIs.
* SEEK acts as the catalogue for the wider platform: registered workflows and tools can be run via Airflow, JupyterHub, or as GUI tools in the web portal.
* Links to clinical metadata (FHIR) and medical imaging (PACS).
* Deployable for local development, production and locked-down environments.


## More information

* [Source code and documentation](https://github.com/ABI-CTT-Group/digitaltwins-platform)
* [FAIRDOM-SEEK integration](https://github.com/ABI-CTT-Group/digitaltwins-platform/blob/main/docs/seek-integration.md)
* Babarenda Gamage TP, Elsayed A, Lin C, Wu A, Feng Y, Yu J, Gao L, Wijenayaka S, Nash MP, Doyle AJ, Nickerson DP. Vision for the 12 LABOURS Digital Twin Platform. Annu Int Conf IEEE Eng Med Biol Soc. 2023 Jul;2023:1-4. [doi: 10.1109/EMBC40787.2023.10341138](https://doi.org/10.1109/EMBC40787.2023.10341138). PMID: 38083471.

