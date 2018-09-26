---
title: Vivocha APIs
excerpt: ''
---

# Vivocha APIs

APIs are the very heart of Vivocha and one of its most distinctive and valuable assets. The API are what give Vivocha the ability to allow any kind of integration and mash-up.

Through the API, Vivocha users can, for instance:

* Fully customize, or even rewrite, each user interface element \(the chat window, the surveys, the proactive popups, etc\);
* Create custom proactive rules, leveraging third party tools and platforms to take proactive decisions \(e.g. reading shopping cart status, getting realtime traffic or weather information, check the availability of stock and available delivery slots, etc\);
* Integrate Vivocha in mobile sites and apps or enrich advertising campaigns.

The API consists in a set a RESTful web services, plus a series of language bindings, including Javascript, ActionScript and iOS.

## Vivocha REST APIs

This set of APIs allows to access to the main features offered by the platform.

With these APIs you can subscribe your webhooks to the vivocha events, request new contacts bypassing the client interface, set a custom webservice for checking the agents availability, or simply get infos about pending contacts and current status.

We currently support two versions of the Vivocha REST APIs:

* [Vivocha REST APIs v1](https://vivocha.atlassian.net/wiki/display/VVCJ/Vivocha+REST+API)
* [Vivocha REST API v2](doc:vivocha-rest-api-v2)

## Vivocha Javascript SDKs

The Vivocha javascript SDKs enable you to customize and control the behaviour of both Visitors and Agent's interfaces. Differents SDKs are dedicated to different environments and use cases:

The  **Frontend SDK** you can create visitor side integrations and customizations, like Custom engagement widgets, proactive rules, ecommerce integrations and more.

The **Console Application SDK** is used to create Console Apps that are extensions to the Vivocha Agent Console used by default by the agents

The **Embedded Console SDK** is a special version of the Vivocha Console, designed to be easily integrated into existing third party Agent Desktops or Softphones. For more info go to [Embedded console](doc:embedded-console) document.

The **Agent SDK** is an advanced Javascript library that can be used to fully implement a Vivocha Agent Desktop from scratch, leveraging Vivocha's low-level communication protocols

The following link redirect you to the full documentation of the [**Vivocha Javascript SDKs**](doc:vivocha-sdks)

