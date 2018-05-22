---
published: true
layout: post
title: An OpenAPI Vendor Extension For Defining Your API Au
date: 2018-03-14T11:00:00.000Z
tags:
  - API Evangelist
  - Definitions
  - Evangelism
  - Security
  - Governance
image: >-
  http://kinlane-productions.s3.amazonaws.com/algorotoscope/builder/filtered/97_193_800_500_0_max_0_1_-1.jpg
---
<p><img src="{{ page.image }}" width="45%" align="right" style="padding: 15px;" /></p>The food delivery service Zalando has an interesting approach to classifying their APIs based upon who is consuming them. It isn't just about APIs being published publicly, or privately, they actually have standardized their definition, and have established an OpenAPI vendor extension, so that the definition is machine readable and available via their OpenAPI.

[According to the Zalando API design guide](http://zalando.github.io/restful-api-guidelines/index.html#219), "_each API must be classified with respect to the intended target audience supposed to consume the API, to facilitate differentiated standards on APIs for discoverability, changeability, quality of design and documentation, as well as permission granting. We differentiate the following API audience groups with clear organisational and legal boundaries._"

- **component-internal** - The API consumers with this audience are restricted to applications of the same functional component (internal link). All services of a functional component are owned by specific dedicated owner and engineering team. Typical examples are APIs being used by internal helper and worker services or that support service operation.
- **business-unit-internal** - The API consumers with this audience are restricted to applications of a specific product portfolio owned by the same business unit.
- **company-internal** - The API consumers with this audience are restricted to applications owned by the business units of the same the company (e.g. Zalando company with Zalando SE, Zalando Payments SE & Co. KG. etc.)
- **external-partner** - The API consumers with this audience are restricted to applications of business partners of the company owning the API and the company itself.
- **external-public** - APIs with this audience can be accessed by anyone with Internet access.

_**Note:** a smaller audience group is intentionally included in the wider group and thus does not need to be declared additionally. The API audience is provided as API meta information in the info-block of the Open API specification and must conform to the following specification_:

#/info/x-audience:
  type: string
  x-extensible-enum:
    - component-internal
    - business-unit-internal
    - company-internal
    - external-partner
    - external-public
  description: |
    Intended target audience of the API. Relevant for standards around
    quality of design and documentation, reviews, discoverability,
    changeability, and permission granting.

_**Note:** Exactly one audience per API specification is allowed. For this reason a smaller audience group is intentionally included in the wider group and thus does not need to be declared additionally. If parts of your API have a different target audience, we recommend to split API specifications along the target audience — even if this creates redundancies (rationale)._

Here is an example of the OpenAPI vendor extension in action, as part of the info block:

swagger: '2.0'
info:
  x-audience: company-internal
  title: Parcel Helper Service API
  description: API for <...>
  version: 1.2.4

Providing a pretty interesting way of establishing the scope and reach of each API in a way that makes each API owner think deeply about who they are / should be targeting with the service. Done in a way that makes the audience focus machine readable, and available as part of it's OpenAPI definition which can be then used across discovery, documentation, and through API governance and security.

I like the multiple views of who the audience could be, going beyond just public and private APIs. I like that it is an OpenAPI vendor extension. I like that they even have a schema crafted for the vendor extension--another interesting concept I'd like to see more of. Overall, making for a pretty compelling approach to define the reach of our APIs, and quantifying the audience we are looking to reach with each API we publish.
