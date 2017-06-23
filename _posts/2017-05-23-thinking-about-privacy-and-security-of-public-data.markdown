---
title: Thinking About The Privacy And Security Of Public Data Using API Management
date: 2017-05-23 15:00:00 Z
tags:
- Privacy
- Security
- Data
- HSDS
- HSDA
image: https://s3.amazonaws.com/kinlane-productions/kin-lane/kin-lane-api-days-berlin-respect-privacy.jpg
---

<p><img style="padding: 15px;" src="https://s3.amazonaws.com/kinlane-productions/kin-lane/kin-lane-api-days-berlin-respect-privacy.jpg" align="right" width="35%" /></p>When I suggest modern approaches to API management be applied to public data I always get a few open data folks who push back saying that public data shouldn't be locked up, and needs to always be publicly available--as the open data gods intended. I get it, and I agree that public data should be easily accessible, but there are increasingly a number of unintended consequences that data stewards need to consider before they publish public data to the web in 2017.

I'm going through this exercise with my recommendations and guidance for municipal 211 operators when it comes to implementing [Open Referral's Human Services Data API (HSDA)](http://developer.open.referral.adopta.agency/documentation/). The schema and API definition centers around the storage and access to organizations, locations, services, contacts, and other key data for human services offered in any city--things like mental health resources, suicide assistance, food banks, and other things we humans need on a day to day basis. 

This data should be publicly available, and easy to access. We want people to find the resources they need at the local level--this is the mission. However, once you get to know the data, you start understanding the importance of not everything being 100% public by default. When you come across listings Muslim faith, and LGBTQ services, or possibly domestic violence shelters, and needle exchanges. They are numerous types of listings where we need to be having sincere discussions around security and privacy concerns, and possibly think twice about publishing all or part of a dataset.

This is where modern approaches to API management can lend a hand. Where we can design specific endpoints, that pull specialized information for specific groups of people, and define who has access through API rate limiting. [Right now my HSDA implementation has two access groups, public and private](http://developer.open.referral.adopta.agency/documentation/). Every GET path is publicly available, and if you want to POST, PUT, or DELETE data you will need an API key. As I consider my API management guidance for implementors, I'm adding a healthy dose of the how and why of privacy and security using existing API management solutions and practice.

I am not interested in playing decider when it comes to what data is public, private, and requires approval before getting access. I'm merely thinking about how API management can be applied in the name of privacy and security when it comes to public data, and how I can put tools in the hands of data stewards, and API providers that help them make the decision about what is public, private, and more tightly controlled. The trick with all of this is how transparent should providers be with the limits and restrictions imposed, and communicate the offical stance with all stakeholders appropriately when it comes to public data privacy and security.