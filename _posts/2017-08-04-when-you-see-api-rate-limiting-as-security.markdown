---
published: true
layout: post
title: When You See API Rate Limiting As Security
date: 2017-08-04T16:00:00.000Z
tags:
  - API Evangelist
  - Security
  - Management
  - Rate Limiting
image: >-
  https://s3.amazonaws.com/kinlane-productions/algo-rotoscope/stories/art-museum/art-museum_copper_circuit_2.jpg
---
<p><img src="https://s3.amazonaws.com/kinlane-productions/algo-rotoscope/stories/art-museum/art-museum_copper_circuit_2.jpg" align="right" width="40%" style="padding: 15px;" /></p>I'm neck deep into my assessment of the world of API security this week, a process which always yields plenty of random thoughts, which end up becoming stories here on the blog. One aspect of API security I keep coming across in this research is the concept of API rate limiting as being security. This is something I've long attributed with API management service providers making their mark on the API landscape, but as I dig deeper I think there is more to this notion of what API security is (or isn't). I think it has more to do with API providers, than companies selling their warez to these API providers.

The API management service providers have definitely set the tone for API security conversation(good), by standing up a gateway, and providing tools for limiting what access is available--I think many data, content, and algorithmic stewards are very narrowly focus on security being ONLY about limiting access to their valuable resources. Many folks I come across see their resources as valuable, when they begin doing APIs they have a significant amount of concern around putting their resources on the Internet, and once you secure and begin rate limiting things, all security concerns appear to have been dealt with. Competitors, and others just can't get at your valuable resources, they have to come through the gate--API security done.

Many API providers I encounter have unrealistic views of the value of their data, content, and algorithms, and when you match this with their unrealistic views about how much others want access to this valuable content you end up with a vacuum which allows for some very narrow views of what API security is. To help support this type of thinking, I feel like the awareness generated from API management is often focused on generating revenue, and not always about understanding API abuse, and is also something can create blindspots when it comes to database, server, and DNS level logging and layers where security threats emerge. I'm assuming folks often feel comfortable that the API management layer is sufficiently securing things by rate limiting, and we can see all traffic through the analytics dashboard. I'm feeling that this one of the reasons folks aren't looking up at the bigger API security picture.

From what I'm seeing, assumptions that the API management layer is securing things can leave blind spots in other areas like DNS, threat information gathering, aggregation, collaboration, and sharing. I've come across API providers who are focused in on API management, but don't have visibility at the database, server, container, and web server logging levels, and are only paying attention to what their API management dashboard provides access to. I feel like API management opened up a new found awareness for API provides, something that has evolved and spread to [API monitoring](http://monitoring.apievangelist.com/), [API testing](http://testing.apievangelist.com/), and [API performance](http://performance.apievangelist.com/). I feel like the next wave of awareness will be in the area of API security. I'm just trying to explore ways that I can help my readers and clients better understand how to expand their vision of API security beyond their current field of vision.
