---
published: true
layout: post
title: Considering How Machine Learning APIs Might Violate Privacy and Security
date: 2017-08-22T11:00:00.000Z
tags:
  - API Evangelist
  - Security
  - Privacy
  - Machine Learning
  - Dependencies
image: 'https://s3.amazonaws.com/kinlane-productions/290x195cloudsecurity2014.jpg'
---
<p><img src="https://s3.amazonaws.com/kinlane-productions/290x195cloudsecurity2014.jpg" align="right" width="40%" style="padding: 15px;" /></p>[I was reading about how Carbon Black, an endpoint detection and response (EDR) service, was exposing customer data via a 3r party API service they were using](http://gearsofbiz.com/carbon-black-edr-service-exposing-customer-data-through-cloud-scanning-update/7096). The endpoint detection and response provider allows customers to optionally scan system and program files using the VirusTotal service. Carbon Black did not realize that premium subscribers of the VirusTotal service get access to the submitted files, allowing an company or government agency with premium access to VirusTotal’s application programming interface (API) can mine those files for sensitive data.

It provides a pretty scary glimpse at the future of privacy and security in a world of 3rd party APIs if we don't think deeply about the solutions we bake into our applications and services. Each API we bake into our applications should always be scrutinized for privacy and security concerns, making sure end-users aren't being subjected to unnecessary situations. This situation sounds like it was both API provider and consumer contributing to the privacy violation, and adjusting platform access levels, and communicating with API consumers would be the best path forward.

Beyond just this situation, I wanted to write about this topic as a cautionary tale for the unfolding machine learning API landscape. Make sure we are thinking deeply about what data and content we are making available to platforms via artificial intelligence and machine learning APIs. Make sure we are asking the hard questions about the security and privacy of data and content we are running through machine learning APIs. Make sure we are thinking deeply about what data and content sets we are running through the machine learning APIs, and reducing any unnecessary exposure of personal data, content, and media.

It is easy to be captivated by the magic of artificial intelligence and machine learning APIs. It is easy to view APIs as something external, and not much of a privacy or security threat. However, with each API call we are inviting a 3rd party API into our databases, files, and other private systems. Let's make sure we have an honest conversation with our API providers about how data and content is accessed, stored, cached, and used as part of any AI or ML process. Let's make sure we get clarification on which partners, or other 3rd party providers are getting access to data and content that is indexed and executed as part of AI and ML API requests and responses. How long are videos or images stored? How long is data stored?

I'm seeing more discussion around dependencies going on in the API space. Which software libraries, and APIs are we depending on for our applications and services. I'm feeling like this conversation is going to continue expanding and security, privacy, and observability is going to become a more significant part of these dependency discussions. It will be a conversation that continues to push API deployment on-premise, and on-premise, being observable about how ML and AI API operations are being logged, stored, and track on. I'm going to keep watching how APIs are intentionally or unintentionally violating security and privacy like this, and keep an eye on the API dependency conversation to see how it evolves as part of this security and privacy discussion.
