---
published: true
layout: post
title: The Trusted Automated Exchange of Intelligence Information (TAXII)
date: 2017-08-01T09:00:00.000Z
tags:
  - API Evangelist
  - Security
  - Definitions
image: 'https://s3.amazonaws.com/kinlane-productions/taxii/taxii-logo.png'
---
<p><a href="https://oasis-open.github.io/cti-documentation/"><img src="https://s3.amazonaws.com/kinlane-productions/taxii/taxii-logo.png" align="right" width="30%" style="padding: 15px;" /></a></p>I recently wrote about [the opportunity around developing an aggregate threat information API](http://apievangelist.com/2017/07/10/opportunity-to-develop-a-threat-intelligence-apis-json/), and got some interest in both creating, as well as investing in some of the resulting products and services that would be derived from this security API work. As part of the feedback and interest on that post, I was pointed in the direction of [the Trusted Automated Exchange of Intelligence Information (TAXII)](https://oasis-open.github.io/cti-documentation/), as one possible approach to defining a common set of API definitions and tooling for the exchange of threat intelligence.

The description of TAXII from the project website describes it well:

> Trusted Automated Exchange of Intelligence Information (TAXII) is an application layer protocol for the communication of cyber threat information in a simple and scalable manner. TAXII is a protocol used to exchange cyber threat intelligence (CTI) over HTTPS. TAXII enables organizations to share CTI by defining an API that aligns with common sharing models. TAXII is specifically designed to support the exchange of CTI represented in STIX.

I breezed through [the documentation for TAXII version 2.0](https://docs.google.com/document/d/1eyhS3-fOlRkDB6N39Md6KZbvbCe3CjQlampiZPg-5u4/edit#heading=h.4do73o99e2l7), and it looks pretty robust, and a project that has made some significant inroads towards accomplishing what I'd like to see out there for sharing threat intelligence. I'm still understanding the overlap of TAXII, the transport mechanism for sharing cyber threat intelligence, and STIX, the structured language for cyber threat intelligence, but it looks like a robust, existing approach defining the schema and an API for sharing threat intelligence.

Next, I am going to gather my thoughts around both of these existing definitions, and look at establishing an OpenAPI that represents STIX and TAXII, providing a machine readable definition for sharing threat intelligence. I think having an OpenAPI will provide a blueprint that can be used to define a handful of server side implementations in a variety of programming languages. I was happy to be directed to this existing work, saving me significant time and energy when it comes to this conversation. Now I don't have to jumpstart it, I just have to contribute to, and augment the work that is already going on.
