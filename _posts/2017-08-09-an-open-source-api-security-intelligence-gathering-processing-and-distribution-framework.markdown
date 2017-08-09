---
published: true
layout: post
title: >-
  An Open Source API Security Intelligence Gathering, Processing, And
  Distribution Framework
date: 2017-08-09T16:00:00.000Z
tags:
  - API Evangelist
  - Security
  - Collaboration
  - Syndication
image: 'https://s3.amazonaws.com/kinlane-productions/GOSINT/gosint.gif'
---
<p><a href="https://blogs.cisco.com/security/open-source-threat-intel-gosint"><img src="https://s3.amazonaws.com/kinlane-productions/GOSINT/gosint.gif" align="right" width="40%" style="padding: 15px;" /></a></p>I was reading about GOSINT, [the open source intelligence gathering and processing framework over at Cisco](https://blogs.cisco.com/security/open-source-threat-intel-gosint). "GOSINT allows a security analyst to collect and standardize structured and unstructured threat intelligence. Applying threat intelligence to security operations enriches alert data with additional confidence, context, and co-occurrence. This means that you are applying research from third parties to your event data to identify similar, or identical, indicators of malicious behavior." The framework is written in Go, with a front-end in JavaScript frontend, and usage of APIs as threat intelligence sources.

[When you look at configuration section on the README for GOSINT](https://github.com/ciscocsirt/gosint), you'll see information for setting up threat intelligence feeds, including Twitter API, [Alien Vault the Open Threat Community API](https://otx.alienvault.com/api/), [VirusTotal API](https://www.virustotal.com/), and [the Collaborative Research Into Threats (CRITS)](https://crits.github.io/).  GOSINT acts as an API aggregator for a variety of threat information, which then allows you to scour the information for threat indicators, which you can evolve over time, providing a pretty interesting model for not just threat information sharing, but also API driven aggregation, curation and sharing.

GOSINT also has the notion of behaving as a "transfer station", where you can export refined data as CSV or CRITS format. Right here seems like an opportunity for some Github integration, adding continuous integration and deployment to open source intelligence and processing workflows. Making sure refined, relevant threat information is available where it is needed, via existing API deployment and integration workflows. Wouldn't take much to publish CSV, YAML, and JSON files to Github which can then be used to drive distributed dashboards, visualizations, and other awareness building tools. Plus, the refined threat information is now published as CSV/JSON/YAML on Github where it can be ingested by any system of application with access to the Github repository.

GOSINT is just one of the interesting tooling I'm coming across as I turn up the volume on [my API security research](http://security.apievangelist.com), thanks to [the investment of ElasticBeam my API security partner](https://www.elasticbeam.com/). They've invested in an API security guide, as well as white paper, which is something that will generate a wealth of stories like this along the way, as I find interesting API security artifacts. I'm looking to map out the API security landscape, but I'm also interested in understanding open source API aggregation, analysis, and syndication platforms that integrate with existing CI/CD workflows, to help feed [my existing human services API work](http://org.open.referral.adopta.agency/), and other city, state, and federal government API projects I'm working on.
