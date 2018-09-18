---
published: true
layout: post
title: "Sadly Stack Exchange Blocks API Calls Being Made From Any Of Amazon's IP Block"
date: 2018-09-17T09:00:00.000Z
tags:
  - API Evangelist
  - Rate limits
  - Management
  - DNS
  - Security
  - Politics of APIs
image: >-
  https://s3.amazonaws.com/kinlane-productions/stack-exchange/stack-exchange-api.png
---
<p><img src="{{ page.image }}" width="45%" align="right" style="padding: 15px;" /></p>I am developing an authentication and access layer for [the API Gallery](http://api.gallery.streamdata.io/) that I am building for [Streamdata.io](http://streamdata.io), while also federating it for usage as part of [my API Stack research.](http://theapistack.com) In addition to building out these catalogs for API discovery purposes, I'm also developing a suite of tools that allow users to subscribe to different topics from popular sources like [GitHub](http://subscribe.github.repository.search.streamdata.io/), [Reddit](http://subscribe.reddit.streamdata.io/), and [Stack Overflow (Exchange)](http://subscribe.stack.exchange.search.streamdata.io/). I've been busy adding one or two providers to my OAuth broker each week, until the other day I hit a snag with the Stack Exchange API.

I thought my Stack Exchange API OAuth flow had been working, it's been up for a few months, and I seem to remember authenticating against it before, but this weekend I began getting an error that my IP address was blocked. I was looking at log files trying to understand if I was making too many calls, or some other potential violation, but I couldn't find anything. Eventually I emailed Stack Exchange to see what their guidance once, to which I got a prompt reply:

_"Yes, we block all of Amazon's AWS IP addresses due to the large amount of abuse that comes from their services. Unfortunately we cannot unblock those addresses at this time."_

Ok then. I guess that is that. I really don't feel like setting up another server with another provider just so I can run an OAuth server from there. Or, maybe I guess I might have to if I expect to offer a service that provides OAuth integration with Stack Exchange. It's a pretty unfortunate situation that doesn't make a whole lot of sense. I can understand adding another layer of white listing for developers, pushing them to add their IP address to their Stack Exchange API application, and push us to justify that our app should have access, but blacklisting an entire cloud provider from accessing your API is just dumb.

I am going to weigh my options, and explore what it will take to setup another server elsewhere. Maybe I will start setting up individual subdomains for each OAuth provider I add to the stack, so I can decouple them, and host them on another platform, in another region. This is one of those road blocks you encounter doing APIs that just doesn't make a whole lot of sense, and yet you still have to find a work around--you can't just give in, despite API providers being so heavy handed, and not considering the impact of the moves on their consumers. I'm guessing in the end, the Stack Exchange API doesn't fit into their wider business model, which is something that allows blind spots like this to form, and continue.
