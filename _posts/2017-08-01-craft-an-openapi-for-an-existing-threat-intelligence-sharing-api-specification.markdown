---
published: true
layout: post
title: Craft An OpenAPI For An Existing Threat Intelligence Sharing API Specification
date: 2017-08-01T16:00:00.000Z
tags:
  - API Evangelist
  - Security
  - Standards
  - Definitions
image: >-
  https://s3.amazonaws.com/kinlane-productions/bw-icons/bw-threat-info-sharing-api.png
---
<p><img src="https://s3.amazonaws.com/kinlane-productions/bw-icons/bw-threat-info-sharing-api.png" align="right" width="40%" style="padding: 15px;" /></p>[I wrote about the opportunity around developing an aggregate threat information API](http://apievangelist.com/2017/07/10/opportunity-to-develop-a-threat-intelligence-apis-json/), and got some interest in both creating, as well as investing in some of the resulting products and services that would be derived from this security API work. As part of the feedback and interest on that post, I was pointed in the direction of the [Structured Threat Information Expression (STIX)](https://oasis-open.github.io/cti-documentation/), a structured language for cyber threat intelligence, and [Trusted Automated Exchange of Intelligence Information (TAXII)](https://oasis-open.github.io/cti-documentation/), and transport mechanism for sharing cyber threat intelligence.

This is why I write about my projects openly like this, so that my readers can help me identify existing approaches for tackling whatever I am focusing on. I prefer to never reinvent the wheel, and build on top of any existing work that is already available. I'm thinking the next step is to craft an OpenAPI fo TAXII, and STIX. Creating a machine readable blueprint for deploying, managing, and documenting a threat intelligence API. I couldn't find any existing work on an OpenAPI definition, so this seems like a logical place to begin working to build on, and augment the work of [the Cyber Threat Intelligence Technical Committee](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=cti). Clearly, the working group has created a robust set of specifications, but I'd like to help move it closer to implementation with an OpenAPI.

[I have created a Github organization to help organize any work on this project](https://github.com/threat-intelligence). I have forked the project for STIX and TAXII there, as well as started [a planning repository](https://github.com/threat-intelligence/planning) to coordinate any work I'm contributing to the conversation. I have also created a repository for working on and publishing the OpenAPI that will define the project. Once we have this, I'd like to start thinking about the development of a handful of server side implementations in maybe Node.js, Python, PHP, or other common programming language. Here are the next steps I'd like to see occur around this project:

- **OpenAPI** - Create an OpenAPI for STIX and TAXII to provide a single representation of a threat intelligence sharing API.
- **Threat List** - Take the [threat intelligence list I originally published](http://apievangelist.com/2017/07/10/opportunity-to-develop-a-threat-intelligence-apis-json/), and identify how any of the sources would map to OpenAPI.
- **Storytelling** - Tell stories throughout the process to attract the attention of other players, contributors, and investors, so that this project can live on.

I'm not looking to own this project 100%. I just don't have the time and resources. However I do want to see an OpenAPI move forward, as well as a wealth of open source resources for deploying, integrating, and aggregating around threat intelligence sharing. This work is bigger than any single player, and is something that needs to be open, spanning thousands of providers, not controlled by a handful of gatekeepers. Players in the threat intelligence sharing game need to be able to decide who they consume and share threat intelligence with, something that will require a federated world of APIs that all speak in a common language. [The Cyber Threat Intelligence Technical Committee](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=cti) is off to a great start. I just want to contribute with some cycles to help bring their work in alignment with what is going on in the mainstream world of APIs, while also beating a drum so that I can bring more attention to any work going on in this important area. Our world is going to need significant investment in the area of threat intelligence sharing if we are going to be successful online in coming years.
