---
title: A new version of SEEK is now available, version 1.7.0
---

**A new version of SEEK is now available, version 1.7.0.** 

Full details can be found at [https://docs.seek4science.org/tech/releases/](https://docs.seek4science.org/tech/releases#version-170)

Highlights include

## Programme wide sharing permissions

Researchers can now apply the fine-grained sharing permissions of assets in SEEK to share with whole programmes. 
This offers our researchers further support in making data [“as open as possible, as closed as necessary”](https://www.linkedin.com/pulse/open-possible-closed-necessary-european-commission-eudat/).

## ISA graph improvements

The ISA graph has been modified to provide better visuals for larger ISA structures. 
In addition we also offer a list-style view of the ISA structure for those wanting to navigate their assets with a more traditional view. 
You can find screen shots, and further information in our documentation [https://docs.seek4science.org/help/user-guide/isa-overview](https://docs.seek4science.org/help/user-guide/isa-overview)

## Changes to Sample Type visibility

A Sample Type now only become visible outside of a Project if it has public samples associated. This change has allowed us to open up Sample Type creation to all members of projects, where previously only project administrators were able to create sample types.

## Special support for for NCBI sample attribute types

Users can now select NCBI IDs as a special sample attribute. This allows automatic linking with Organisms registered in SEEK. This is part of our ongoing work to replace SEEK strains with a dedicated Sample Type.

## Linking Documents to Events, and vice versa.

There has also been quite a bit of back-end maintenance and tidying up.

The guide to upgrade is available at
[https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html). Note that with this
version Ruby 2.4 is required, using 2.2 or 2.3 will result in errors.

The fairdom/seek:1.7 docker image is also available, and upgrading for
Docker Compose can be found at the end of
[https://docs.seek4science.org/tech/docker/docker-compose.html](https://docs.seek4science.org/tech/docker/docker-compose.html)
