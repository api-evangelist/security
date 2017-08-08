---
published: true
layout: post
title: Open Sourcing Your API Like VersionEye
date: 2017-08-08T11:00:00.000Z
tags:
  - API Evangelist
  - SDK
  - Monitoring
  - Security
  - Open Source
  - Deployment
image: >-
  https://s3.amazonaws.com/kinlane-productions/versioneye/version-eye-containers.png
---
<p><img src="https://s3.amazonaws.com/kinlane-productions/versioneye/version-eye-containers.png" align="right" width="40%" style="padding: 15px;" /></p>I'm always on the hunt for healthy patterns that I would like to see API providers, and API service providers consider when crafting their own strategies. It's what I do as the API Evangelist. Find common patterns. Understand the good ones, and the bad ones. Tell stories about both, helping folks understand the possibilities, and what they should be thinking about as they plan their operations.

One very useful API that notifies you about security vulnerabilities, license violations and out-dated dependencies in your Git repositories, [has a nice approach to delivering their API](https://www.versioneye.com/api/), as well as [the other components of their stack](https://github.com/versioneye). You can either use VersionEye in the cloud, or you can deploy on-premise:

- [versioneye-core](https://github.com/versioneye/versioneye-core) - Models, Services & Mails for VersionEye
- [crawl_r](https://github.com/versioneye/crawl_r) - VersionEye crawlers implemented in Ruby.
- [versioneye-security](https://github.com/versioneye/versioneye-security) - Security Crawler for VersionEye
- [versioneye-api](https://github.com/versioneye/versioneye-api) - JSON REST API for VersionEye
- [versioneye-tasks](https://github.com/versioneye/versioneye-tasks) - Thin wrapper around the versioneye-core.
- [versioneye](https://github.com/versioneye/versioneye) - VersionEye.com

[VersionEye also has their entire stack available as Docker images](https://hub.docker.com/u/versioneye/), ready for deployment anywhere you need them. I wanted have a single post that I can reference when talking about possible open source, on-premise, continous integration approaches to delivering API solutions, that actually have a sensible business model. VersionEye spans the areas that I think API providers should consider investing in, delivering SaaS or on-premise, while also delivering open source solutions, and generating sensible amounts of revenue.

Many APIs I come across do not have an open source version of their API. They may have open source SDKs, and other tooling on Github, but rarely does an API provider offer up an open source copy of their API, as well as Docker images. VersionEye's approach to operating in the cloud, and on-premise, while leveraging open source and APIs, as well as dovetailing with existing continous integration flows is worth bookmarking. I am feeling like this is the future of API deployment and consumption, but don't get nervous, there is still plenty of money to be be made via the cloud services.
