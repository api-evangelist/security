---
published: true
layout: post
title: Explaining API Security To Organizational Leadership
date: 2018-03-06T09:00:00.000Z
tags:
  - API Evangelist
  - Security
  - Politics of APIs
image: >-
  https://s3.amazonaws.com/kinlane-productions/algo-rotoscope/stories/castle-on-hill-edinburgh_propaganda_leaflets.JPG
---
<p><img src="https://s3.amazonaws.com/kinlane-productions/algo-rotoscope/stories/castle-on-hill-edinburgh_propaganda_leaflets.JPG" alIgn="right" width="45%" style="padding: 15px;" /></p>I've been tasked with helping explain API security to senior leadership, and wanted to work through my ideas here on the blog. For this audience, I'm not going to get down into the weeds regarding the technical specification behind OAuth, and other approaches, and try to keep things high level, introducing folks to the art that is API security. The phrase API security represents a balance of concepts because APIs are by nature about providing access, while security is about controlling and sometimes limiting access, resulting in a new way of getting business done on the open web.

**First, What Are APIs?**
APIs are not the latest trend, or vendor solution, they are the next evolution in the web. Web sites and applications return HTML via a URL, and meant to display information to humans in a browser, while APIs return JSON or XML of the same information, but meant to be used in other applications and systems. API security is designed to allow access to our digital resources using the web, while also securing it in a way to ensure only the intended audience is able to obtain  access. APIs are designed to securely provide access to data, content, media, and algorithms using the same web that us humans use to access information online via our browsers.

**Access Using Secure URLs**
APIs use web URLs get read and write data, content, media, and to allow engagement with algorithms. If you want a list of press releases, you visit https://api.example.com/press/. If you want a list of contacts from the CRM, you visit https://api.example.com/contacts/. The URL for all API resources should be encrypted by default, protecting all requests and responses in transit. Providing the first layer of security for APIs, ensuring only approved consumers can view data, content, media, and valuable algorithms being transmitted online.

**Registration Always Required For APIs**
A common misconcept about web APIs is that they are all like Twitter, and are publicly available on the web. However, almost all web APIs actually require that you register before you get any access to any resources. This process is the beginning of what is called API management, where developers have to sign up for an account, and in some cases be approved before they get access to APIs. Most of the time there is self-service, automatic registration, but developers only get limited access, which once they've been approved, proven their identity, or put in a credit card--will be able to obtain higher levels of access to resources.

**Application Keys For Each API Call**
Once developers have been approved for access, they can begin making API calls. However, each API will require that API keys, and required credentials are present with each call. Providing identification of every API consumer, and exactly what they are consuming. API keys are often seen as all that is needed to properly securing APIs, but in reality, they are much more about identifying and tracking what API consumers are doing. Going beyond just focusing on securing the digital resources, and really developing an awareness of who is accessing what, which will prove to be more valuable than just requiring registration to acess APIs alone.

**Suite Of Authentication Options**
There are a handful of approaches in use when it comes to requiring developers to authenticate and pass along their API keys with each response. Each approach has pros and cons, but the industry has widely settled in on four main ways to require API developers to authenticate themselves when using APIs:

- **Basic Auth** - Usage of the basic authentication format that is part of the standard HTTP operations, employing a username and password as credentials for accessing API resources.
- **Key Access** - Providing simple tokens, often called API key as a common way to access to APIs, issuing one to each developer and per application they register.
- **JSON Web Token** - JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.
- **oAuth** - Providing an oAuth layer to API operations, securing high value APIs, while also opening up a conversation between an API platform, developers, and end-users regarding the access of their content and data.

Depending on the security requirements of the resource, and whether or not users generated data and content is involved, you may select a different path for how you require API developers to authenticate. API keys via the URL or headers, as well as Basic Auth are the most common. with JSON Web Tokens, and OAuth being put to work in higher security environments, and where users data, and permission might be required.

**Logging Of All API Activity**
A essential aspect of securing APIs involves the logging of ALL API calls, no matter who the consumer is, what application it is serving, and whether it is for internal, or external cosumption. All API calls get logged equally, and when all API developers are required to authenticate and pass their keys with each API call, all the evidence needed to understand API activity and consumption is present. When you combine the API level logging with backend database logs, and front-end DNS logs, you can define a set of perimiters that will help ensure the security of your API resources.

**Modern API Management Solutions**
API management combines the authentication and logging described above with API plans, rate limiting, and analytics, to achieve a heightened awareness regarding who is accesss what API resources, and how they are putting them to use. Modern API management allows for the monitoring of API registrations, authentication, and consumption in real time, with controls for limiting or shutting off access whenever terms of service and security violations are identified. Providing API providers with the tools they need to monitor and respond to any security concerns, while staying in tune with exactly how resources are being accessed via APIs.

**Defining Access To APIs Using Service Composition**
API management also allows API providers to develop different levels of API access plans, which govern the APIs that developers will have access to, and how much they are entitled to consume. API service composition is all about organizing different APIs into different plans, and setting rate limits that govern how much a user can use per second, minute, days, or by the month. New users are often placed into plans with stricter limitations, while more trusted, partner, and internal consumers enjoy higher rate limits, and less restrictive plans. Service composition helps minimize the damage that occurs whenver there are bad actors present, or security incidents occur, keeping the breaches limited to a small subset of low value APIs, and limited amount of resources accessed.

**Monitoring All API Availability**
Beyond API management, and the analysis of API consumption, it is common for API providers to setup external monitors that keep an eye on whether APIs are up or down, and what their overall availability are. Providing a status dashboard showing whether APIs are available, which also often shows historical availability over time. The health and availability of an API is usually a barometer of the security of an API. Insecure, and compromised APIs often times have an unreliable availability and track record. Making monitoring critical to the overall security of API operations.

**Granular Testing of All APIs**
Augmenting API management and monitoring, the most mature and secure API providers out there also run recurring tests on APIs, going beyond just seeing if they are up and available, and actually making sure they respond, and deliver the data and content that is expected. These tests will sometimes go further and test for the ability to publish bad data to APIs, input incorrect or additional information, and push the boundaries of what an API will respond to. Mimicking some of the behaviors in which malicious users and applications will perform, and testing the quality of the surface area of API.

**Security Scans For All APIs**
Beyond granular tests for all APIs, more general security scans are regularly performed, looking beyond the potentially known security problems, and finding the more unknown issues. Scanning additional URLS, parameters, headers, and checking for holes, gaps, and other areas of the surface area for APIs which may have been overlooked or forgotten. Security scanning reflects the scanning that already occurs on most web and mobile applications, but will also consider many of the API specific vulnerabilities that we've seen behind breaches of the past, and those that are unique to API integration scenarios.

**API Security Is More About Building An Awareness**
While API security centers around establishing a defensive perimeter around API resources, policing and enforcing rules along this perimeter, and encrypting all traffic, most of API security is realized through an awareness around how APIs are being accessed. API management, logging, monitoring, testing, and analytics provide an approach to understanding how data, content, media, and algorithms are being used, or not being used. Providing an evolved level of awareness that goes well beyond legacy web services and database connectivity.

API security should center around encryption, and common approaches to authenticating APIs. However, if they are not being properly monitored, tested, analyzed, and audited, a strong security perimeter, encryption, and strong authentication will not mean much. It is important for all key stakeholders involved in API operations to understand that API security is a balance between allowing for access and consumption, while also locking down, encrypting, and defending the perimeter. The API providers who find the most success with their API operations tend to strike a balance between these two opposing personalities of API security, making sure everything is secure, while also making sure providers, developers, and end-users feel secure while also being able to get access the resource they need to do their job.
