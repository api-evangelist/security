---
published: true
layout: post
title: The ElasticSearch Security APIs
date: 2017-08-15T12:00:00.000Z
tags:
  - API Evangelist
  - Security
  - Search
  - Authentication
  - Management
image: >-
  https://s3.amazonaws.com/kinlane-productions/elastic-search/elasticsearch-security-apis.png
---
<p><a href="https://www.elastic.co/guide/en/elasticsearch/reference/current/security-api.html"><img src="https://s3.amazonaws.com/kinlane-productions/elastic-search/elasticsearch-security-apis.png" align="right" width="40%" style="padding: 15px;" /></a></p>I was looking [at the set of security APIs over at Elasticsearch](https://www.elastic.co/guide/en/elasticsearch/reference/current/security-api.html) as I was diving into my API security research recently. I thought the areas they provide security APIs for the search platform was worth noting and including in not just my API security research, but also [search](http://search.apievangelist.com), deployment, and probably overlap with [my authentication research](http://authentication.apievangelist.com). 

- **Authenticate API** - The Authenticate API enables you to submit a request with a basic auth header to authenticate a user and retrieve information about the authenticated user.
- **Clear Cache API** - The Clear Cache API evicts users from the user cache. You can completely clear the cache or evict specific users.
- **User Management APIs** - The user API enables you to create, read, update, and delete users from the native realm. These users are commonly referred to as native users.
- **Role Management APIs** - The Roles API enables you to add, remove, and retrieve roles in the native realm. To use this API, you must have at least the manage_security cluster privilege.
- **Role Mapping APIs** - The Role Mapping API enables you to add, remove, and retrieve role-mappings. To use this API, you must have at least the manage_security cluster privilege.
- **Privilege APIs** - The has_privileges API allows you to determine whether the logged in user has a specified list of privileges.
- **Token Management APIs** - The token API enables you to create and invalidate bearer tokens for access without requiring basic authentication. The get token API takes the same parameters as a typical OAuth 2.0 token API except for the use of a JSON request body.

Come to think of it, I'll add this to my [API management research](http://management.apievangelist.com) as well. [Much of this overlaps with what should be a common set of API management services as well](http://apievangelist.com/2015/03/04/adding-four-new-building-building-blocks-providing-an-api-management-api-blueprint/). Like much of my research, there are many different dimensions to my API security research. I'm looking to see how API providers are securing their APIs, as well as how service providers are selling security services to APIs providers. I'm also keen on aggregating common API design patterns for security APIs, and quantity how they overlap with other stops along the API lifecycle.

While the cache API is pretty closely aligned with delivering a search API, I think all of these APIs provide a potential building block to think about when you are deploying any API, and represents the Venn diagram that is API authentication, management, and security. I'm going through the rest of the [Elasticsearch](https://www.elastic.co/) platform looking for interesting approaches to ensuring their search solutions are secure. I don't feel like there are any search specific characteristics of API security that I will need to include in my final API security industry guide, but Elasticsearch's approach has re-enforced some of the existing security building blocks I already had on my list.
