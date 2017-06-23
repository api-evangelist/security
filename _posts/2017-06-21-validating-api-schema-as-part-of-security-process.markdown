---
title: Validating My API Schema As Part of My API Security Practices
date: 2017-06-21 13:00:00 Z
tags:
- Security
- Testing
- Monitoring
- API Evangelist
image: https://s3.amazonaws.com/kinlane-productions/fcc/fcc-makes-net-neutrality-commenters-email-addresses-public-through-api.png
---

<p><a href="https://arstechnica.com/information-technology/2017/06/psa-commenting-on-fcc-net-neutrality-plan-could-make-your-e-mail-public/"><img src="https://s3.amazonaws.com/kinlane-productions/fcc/fcc-makes-net-neutrality-commenters-email-addresses-public-through-api.png" align="right" width="40%" style="padding: 15px;" /></a></p>[I am spending more time thinking about the unknown unknowns when it comes to API security](https://apievangelist.com/2017/06/20/unknown-unknown-with-api-security/). This means thinking beyond the usual suspects when thinking about API security like encryption, API keys, and OAuth. As I monitor the API space I'm keeping an eye out for examples of what might be security concerns that not every API provider is thinking about. [I found one recently in ARS Technica, about the Federal Communication Commission (FCC) leaking the email addresses through the [CC API for anyone who submitted feedback as part of any issues like the recent Net Neutrality discussion](https://arstechnica.com/information-technology/2017/06/psa-commenting-on-fcc-net-neutrality-plan-could-make-your-e-mail-public/).

It sounds like the breach with the [FCC API](https://www.fcc.gov/ecfs/public-api-docs.html) was unintentional, but it provides a pretty interesting example of a security risk that could probably be mitigated with some basic API testing and monitoring, using common services like [Runscope](https://www.runscope.com/), or [Restlet Client](https://restlet.com/). Adding a testing and monitoring layer to your API operations helps you look beyond just an API being up or down. You should be validating that each endpoint is returning the intended/expected schema. Just this little step of setting up a more detailed monitor can give you that brief moment to think a little more deeply about your schema--the little things like whether or not you should be sharing the email addresses of thousands, or even millions of users.

[I'm working on a JSON Schema for my Open Referral Human Services API right now](https://openreferral.github.io/api-specification/definition/). I want to be able to easily validate any API as human services compliant, but I also want to be able to setup testing and monitoring, as well as security checkups by validating the schema. When it comes to human services data I want to be able to validate every field present, ensuring only what is required gets out via the API. I am validating primarily to ensure an API and the resulting schema is compliant with HSDS/A standards but seeing this breach at the FCC has reminded me that taking the time to validate the schema for our APIs can also contribute to API security--for those attacks that don't come from outside, but from within.

**Disclosure:** [Restlet Client](https://restlet.com/) and [Runscope](https://www.runscope.com/) are API Evangelist partners.