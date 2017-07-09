---
title: The Unknown Unknowns Of API Security
date: 2017-06-19 13:00:00 Z
tags:
- Security
- API Evangelist
image: https://s3.amazonaws.com/kinlane-productions/bw-icons/bw-security-unknown.png
---

<p><a href="http://security.apievangelist.com/"><img src="https://s3.amazonaws.com/kinlane-productions/bw-icons/bw-security-unknown.png" align="right" width="25%" style="padding: 15px;" /></a></p>I am trying to wrap my head around the next steps in the evolution of [API security](http://security.apievangelist.com/). I am trying to help separate some of the layers of what we collectively call API security, into some specific building blocks I can reference in my storytelling. I'm ramping up my API security research as I onboard a new API service provider partner, and will have more resources to invest in the API security discussion.

Let's start with the easy "Known Knowns":

* Encryption - Using encryption across all aspects of API operations from portal to base URL.
* API Keys - Making sure everyone who is accessing an API is keying up and passing along with each request.
* OAuth - Getting more granular with access by applying OAuth when there is access to 3rd party data and content.
* Rate Limiting - Limiting how much of a resource any single API consumer can access using rate limiting.

These are the first things that come to mind when the topic of API security is brought up. I'd say most conversation begin with encryption, but as someone progresses on their API journey they begin to understand how they can key things up, using OAuth, rate limiting, and other aspects of API management to secure their API operations.

Next, I want to think about some the "Known Unknowns", things like:

* Freeloaders - People with multiple accounts, and generally aren't healthy consumers.
* Errors - Errors, misconfigured, and malformed requests, responses, and anything that generally gums up the gears of operations.
* Vulnerabilities - Making sure all known software and hardware vulnerabilities are patched and communicated as part of operations.
* Attacks - Defending against the known attacks, staying in tune with OWASP and other groups who are actively identifying, studying, and sharing attacks.

These are the things we might not totally understand or have implemented, but they are known(ish). With the right amount of resources and expertise, any API team should be able to mitigate against these areas of security. There is always a lot of work to turn the unknowns into knowns in this area, but they are doable.

Now I want to think a little about the "Unknown Unknowns", likes like:

* DNS - What is happening at the DNS level as it pertains to my API security?
* Relationship - Relationship between requests, even if they are using different keys, IP addresses, and other elements--where is the overlap?
* Threats - What information is available to me regarding new and emerging threats that I'm only beginning to see, or maybe my partners and others in same space are seeing?
* Sharing - Are there opportunities to share information and see a bigger picture when it comes to vulnerabilities and threats?

These are just a handful of my initial thoughts on what the unknown unknowns might be. Things that are currently off the radar of my known API security practices. API management seems to dominate and in some cases terminate the API security conversation, but I have the feeling there are numerous other considerations out there that we are not seeing. I'm just looking to begin defining this new bucket of security considerations so I can keep adding items to it as I'm doing my research.

From your perspective, what are the biggest threats out there for API security that many API providers are completely unaware of? I'm looking to keep expanding on this frontline of API security and turn up the heat beneath [my research](http://security.apievangelist.com) while I have the resources to do so. I feel like the API security conversation has kind of stagnated after the last wave of API management growth, leaving many providers thinking they have everything covered.