---
published: true
title: Making An Account Activity API The Default
date: 2017-06-29T11:00:00.000Z
tags:
  - API Evangelist
  - Management
  - Authentication
  - Security
image: >-
  https://s3.amazonaws.com/kinlane-productions/twitter/twitter-account-activity-api-.png
---
<p><a href="https://dev.twitter.com/webhooks/account-activity"><img src="https://s3.amazonaws.com/kinlane-productions/twitter/twitter-account-activity-api-.png" align="right" width="40%" style="padding: 15px;" /></a></p>[I was reading an informative post about the Twitter Account Activity API](https://medium.com/@esfand/twitter-account-activity-api-8c59347380be), which seems like something that should be the default for ALL platforms. In today's cyber insecure environment, we should have the option to subscribe to a handful of events regarding our account or be able to sign up for a service that can subscribe and help us make sense of our account activity. 

An account activity API should be the default for ALL the platforms we depend on. There should be a wealth of certified aggregate activity services that can help us audit and understand what is going on with our platform account activity. We should be able to look at, understand, and react to the good and bad activity via our accounts. If there are applications doing things that don't make sense, we should be able to suspend access, until more is understood.

The Twitter Account Activity API Callback request contains three level of details:

* direct_message_events: An array of Direct Message Event objects.
* users: An object containing hydrated user objects keyed by user ID.
* apps: An object containing hydrated application objects keyed by app ID.

The Twitter Account Activity API provides a nice blueprint other API providers can follow when thinking about their own solution. While the schema returned will vary between providers, it seems like the API definition, and the webhook driven process can be standardized and shared across providers.

[The Twitter Account Activity API is in beta](https://dev.twitter.com/webhooks/account-activity), but I will keep an eye on it. Now that I have the concept in my head, I'll also look for this type of API available on other platforms. It is one of those ideas I think will be sticky, and if I can kick up enough dust, maybe other API providers will consider. I would love to have this level of control over my accounts, and it is also good to see Twitter still rolling out new APIs like this.
