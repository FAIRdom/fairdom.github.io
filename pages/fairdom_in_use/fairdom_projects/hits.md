---
title: HITS Publications Management Tool
description: The publication management platform for the Heidelberg Institute for Theoretical Studies. 
page_img: fairdom_in_use/hits-logo.svg
type: project
---

As of April 2020, the Heidelberg Institute for Theoretical Studies ([HITS](https://h-its.org/)) adopted [FAIRDOM-SEEK](https://fair-dom.org/fairdomseek) as its [publication management platform](https://publications.h-its.org/). This tool is designed to efficiently collect and manage the institute's research papers and outcomes. FAIRDOM-SEEK provides multiple methods for researchers to register their publications, including using identifiers like DOI or PubMed ID, importing from a BibTeX file for batch creation, or manually entering publication metadata.

{% include image.html file="fairdom_in_use/hits2.jpg" alt="HITS Groups and FAIRDOM-SEEK" click=true class='screenshot' caption="HITS uses FAIRDOM-SEEK to efficiently collect and manage the institute's research papers and outcomes." %}


Beyond registering metadata, FAIRDOM-SEEK enables users to upload the full PDF of their papers. While the metadata is always publicly accessible, users can control access to the actual PDF. With FAIRDOM-SEEK's flexible sharing permissions, users can specify who can view the paper, whether it's a particular individual or a specific group.

## Features
FAIRDOM-SEEK also offers a semi-automated mechanism to link publication authors to FAIRDOM-SEEK users, connecting their scientific publications with their other research work and outcomes. This feature helps users engage with the broader research community, enhancing the visibility of their work.

FAIRDOM-SEEK includes a REST API with both READ and WRITE capabilities, facilitating integration with other platforms or systems. The platform offers various criteria for filtering publications, such as tags, research groups, years, authors, and publication types. Currently, the HITS website utilizes metadata fetched from FAIRDOM-SEEK to generate publication lists for [individuals](https://www.h-its.org/people/priv-doz-dr-wolfgang-muller/) or [groups](https://www.h-its.org/research/mcm/publications/). Additionally, HITS uses the FAIRDOM-SEEK API to compile an annual publication list for the institute's [annual report](https://www.h-its.org/media/annualreport/).

