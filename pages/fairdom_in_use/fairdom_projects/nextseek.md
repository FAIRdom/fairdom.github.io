---
title: "NExtSEEK, Network Extended SEEK for Active Data Management"
type: project
description: A wrapper for FAIRDOM-SEEK for active data management at MIT BioMicro Center.
page_img: fairdom_in_use/mit-biomicro-logo.png
---

## Introduction

NExtSEEK is a variant of SEEK that converts SEEK into an active data management platform. This project has been developed out of the [MIT BioMicro Center](https://openwetware.org/wiki/BioMicroCenter) / Koch Institute Integrated Genomics and Bioinformatics Core Facility.

NExtSEEK is a wrapper, built around the FAIRDOM-SEEK Infrastructure, to allow for active data management of ongoing research projects, as opposed to SEEK’s focus as a repository. It accomplishes this by introducing mutable "hard sample typing" and transforming assays from nodes into edges. This approach creates a network model of a study that more accurately reflects the experimental process. A comprehensive distinction between SEEK and NExtSEEK exists here:

* Pradhan D, Ding H, Zhu J, Engelward BP, Levine SS. [NExtSEEK: Extending SEEK for Active Management of Interoperable Metadata](https://jbt.pubpub.org/pub/nextseek-interopaerable-data-management/release/1). Journal of Biomolecular Techniques. 2022;33(1). doi:10.7171/3fc1f5fe.db404124

NExtSEEK can be best run as a private instance that hosts pre-publication research data, where groups/consortiums can share data and metadata amongst themselves. At the time of publication, data and metadata can be easily deposited into FAIRDOMHub to adhere to FAIR data standards.

Documentation on how to [install](https://igb.mit.edu/data-management/seek-and-nextseek) or [use](https://koch-institute-mit.gitbook.io/mit-data-management-analysis-core/uploading) NExtSEEK exists here.

## Projects

NExtSEEK is used by the MIT BioMicro Center / IGB to support several projects including:

* [HI-IMPAcTB](https://www.niaid.nih.gov/research/immune-mechanisms-protection-mycobacterium-tuberculosis)

* [The MIT SuperFunder Research Program (SRP)](https://superfund.mit.edu/)

* [Metastasis Network of Cancer (MetNet)](https://reporter.nih.gov/search/yoc2JaX_LU23-SGX943zLA/project-details/10271565)

* [Cancer System Biology Consortium (CSBC)](https://www.cancer.gov/about-nci/organization/dcb/research-programs/csbc)

* [Break Through Cancer (BTC)](https://breakthroughcancer.org/)

Published Datasets for these projects exist in a [centralized location on NExtSEEK](https://nextseek.mit.edu/published-studies/), or by Project on FAIRDOMHub ([HI-IMPAcTB](https://fairdomhub.org/projects/222), [MIT SRP](https://fairdomhub.org/projects/221#studies), [MetNet](https://fairdomhub.org/projects/340#studies), [CSBC](https://fairdomhub.org/projects/441)).

[![HI-IMPActB logo](/images/fairdom_in_use/imactb-logo.png)](https://www.niaid.nih.gov/research/immune-mechanisms-protection-mycobacterium-tuberculosis)
[![SRP logo](/images/fairdom_in_use/srp-logo.png)](https://superfund.mit.edu/)
[![MetNet logo](/images/fairdom_in_use/metnet-logo.png)](https://reporter.nih.gov/search/yoc2JaX_LU23-SGX943zLA/project-details/10271565)
[![CSBC logo](/images/fairdom_in_use/csbc-logo.jpg)](https://www.cancer.gov/about-nci/organization/dcb/research-programs/csbc)
[![BTC logo](/images/fairdom_in_use/btc-logo.png)](https://breakthroughcancer.org/)