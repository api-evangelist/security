---
published: true
layout: post
title: VersionEye SDK Security Notifications
date: 2017-09-13T11:00:00.000Z
tags:
  - API Evangelist
  - Security
  - SDK
image: 'https://s3.amazonaws.com/kinlane-productions/versioneye/versioneye-logo.jpeg'
---
<p><a href="https://www.versioneye.com/"><img src="https://s3.amazonaws.com/kinlane-productions/versioneye/versioneye-logo.jpeg" align="right" width="30%" style="padding: 15px;" /></a></p>I've written about [VersionEye](https://www.versioneye.com/) a couple of times. They help you monitor the 3rd party code you use, keeping an eye on dependencies, license violations, and security issues. [I've written about the license portion of this equation](http://apievangelist.com/2017/08/01/api-sdk-licensing-notifications-using-versioneye/), but they came up again while doing my API security research, and I wanted to make sure I revisited what they were up to in this aspect of the API lifecycle, floating them up on my radar.

VersionEye is keeping an eye on multiple security databases and helps you monitor the SDKs you are using in your application. Inversely, if you are an API provider generating SDKs for your API consumers to put to use, it seems like you should be proactively leverage VersionEye to help you be the eye on the security aspects of your SDK management. They even help developers within their existing CI/CD workflows, which is something that you should be considering as you plan, craft, and support your APIs. Making it as easy for you to leverage your APIs SDKs in your own workflow, and doing the same for your consumers, while also paying attention to security at each step, breaking your CI/CD process when security is breached.

[I also wrote about how VersionEye has open sourced their APIs](http://apievangelist.com/2017/08/09/open-sourcing-your-api-like-version-eye/) a while back, highlighting how you can also deploy into any environment you desire. I'm fascinated by the model VersionEye provides for the API space. They are offering valuable services that help us manage our crazy worlds, with a viable commercial and open source offering, that integrates with your existing CI/CD workflow. Next, I'm going to study the dependency portion of what VersionEye offer, then take some time to better understand their business model and pricing. VersionEye is pretty close to what I like to see in a service provider. They don't have all the shine of a brand new startup, but they have all the important elements that really matter.