---
title: "FAIRDOM-SEEK version 1.18.2 released"
---

We are pleased to announce a new version of [FAIRDOM-SEEK](/fairdomseek) is now available, which is version **1.18.2**

This is a patch release that focuses on performance, privacy and bug fixes, including:

* Performance improvements:
  * JavaScript is now minified when assets are precompiled for production.
  * The COPASI and Plotly libraries are only loaded on the model simulation page, reducing the gzipped bundle size from around 5.95 MB to 1.71 MB.
  * A new `obfuscate_filters` setting reduces crawler traffic by changing how filter links are rendered.
* Temporary sharing link improvements:
  * Pages visited through a temporary sharing link are no longer indexable by search engines.
  * Authorization codes in sharing links are now redacted from logs and error notification emails.
* Search fixes:
  * Search on a fresh Docker or Docker Compose installation no longer returns every viewable item instead of the matching ones.
  * Invalid year ranges in filters no longer trigger a database error.
* Project fixes, with roles now listed consistently across the project roles administration and overview pages.
* A fix to an error in the [DataHub](https://fair-dom.org/fairdom-in-use/Datahub) experiment view when viewed without being logged in.
* Various library and security updates, including Rails 7.2.3.2 and rubyzip.

There are several more changes, details of which can be found in the [1.18.2 Release Notes](https://docs.seek4science.org/tech/releases/#version-1182).

Details on installing SEEK can be found in our Documentation, at [https://docs.seek4science.org/get-seek.html](https://docs.seek4science.org/get-seek.html) – including running with [Docker](https://www.docker.com/).

The upgrade guide can be found in the usual place at [https://docs.seek4science.org/tech/upgrading.html](https://docs.seek4science.org/tech/upgrading.html)
