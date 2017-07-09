---
title: Does Your API Sandbox Have Malicious Users?
date: 2017-07-06T11:00:00.000Z
published: true
layout: post
tags:
  - API Evangelist
  - Security
  - Virtualization
  - Reliability
image: >-
  https://s3.amazonaws.com/kinlane-productions/algo-rotoscope/stories/sand-hand_light_dali.jpg
---
<p><img src="https://s3.amazonaws.com/kinlane-productions/algo-rotoscope/stories/sand-hand_light_dali.jpg" align="right" width="40%" style="padding: 15px;" /></p>I have been going through [my API virtualization research](http://virtualization.apievangelist.com/), expanding the number of companies I'm paying attention to, and taking a look at industry specific sandboxes, mock APIs, and other approaches to virtualizing APIs, and the data and content they serve up. I'm playing around with some banking API sandboxes, getting familiar with PSD2, and learning about how banks are approaches their API virtualization--providing me with an example within a heavily regulated industry.

AS I'm looking through [Open Bank Project's PSD2 Sandbox](https://github.com/OpenBankProject/OBP-API/wiki/PSD2-Sandbox), and playing with [services that are targeting the banking industry with sandbox solution](https://www.sandboxbanking.com/developers.html), I find myself thinking about [Netflix's Chaos Monkey](https://github.com/Netflix/chaosmonkey), which is "a resiliency tool that helps applications tolerate random instance failures." Now I am wondering if there are any API sandboxes out there that have simulated threats built in, pushing developers to build more stable and secure applications with API resources.

There are [threat detection solutions that have APIs](https://www.fortinet.com/products/sandbox/fortisandbox.html), and some interesting [sandboxes for analyzing malware that have APIs](https://www.joesecurity.org/), but I don't find any API sandboxes that just have general threats available in them. If you know of any sandboxes that provide simulations, or sample data, please let me know. Also if you know of any APIs that specifically provide API security threats in their sandbox environments so that developers can harden their apps--I'd love to hear more about it. I depend on my readers to let me know of the interesting details from API operations like this.

I'm on the hunt for APIs that have sandboxes that assist application developers think about the resiliancy and security of their applications built on top of an API. Eventually I'd also love to see a sandbox emerge to emerge that could help API providers think about the resiliancy and security of their APIs. I'm feeling like this aspect of API virtualization is going to become just as critical as guidance on API design best practices, but helping API operaters better understand the threats they face as API operators, and quantify them against their API in a virtualized and simulated environment that isn't going to freak them out about the availability of their production environment.

I'll keep an eye out for more examples of this in the wild--if you know of anything please let me know--thanks!
