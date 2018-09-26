---
title: Vivocha 6.1 Release Notes
excerpt: ''
---

# Vivocha 6-1 Release Notes

[1. New conversational ways to collect your customers’ data](vivocha-6-1-release-notes.md#section-1-new-conversational-ways-to-collect-your-customers-data) [2. Boost your Campaign strategy](vivocha-6-1-release-notes.md#section-2-boost-your-campaign-strategy) [3. New Data Collection features](vivocha-6-1-release-notes.md#section-3-new-data-collection-features) [4. Interaction App](vivocha-6-1-release-notes.md#section-4-interaction-app) [5. Improve the effectiveness of your Webleads with the Interaction modes](vivocha-6-1-release-notes.md#section-5-improve-the-effectiveness-of-your-webleads-with-the-interaction-modes) [6. External Services](vivocha-6-1-release-notes.md#section-6-external-services)   


During the last months we spent our time listening to your feedbacks about our new Campaign Builder, that was released last March, and improving it. We focused about some important features for our customers and these are here summarized.

## Majors

### 1. New conversational ways to collect your customers’ data

A new important improvement of the Campaign Builder is about Data Collection. Until now, you could only collect your customer’s data during his visit on your website and exclusively using a form. Starting from this version, in addition to the form-based data collection you can also use two new different kinds of Data Collectors: \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/ee39e9f-01.png](https://files.readme.io/ee39e9f-01.png)", "01.png", 2457, 1025, "\#f9f8f8" \], "border": true, "sizing": "80" } \] } \[/block\]

* The first one is the Dialog Data Collector: you can generate on-the-fly a bot-like, dialog-based data collector in just a few clicks, by adding the information you need to collect and, if you want, customising the entire dialogue to ask data to your customers. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/3dd58d7-02.png](https://files.readme.io/3dd58d7-02.png)", "02.png", 2451, 1561, "\#fbfbfb" \], "border": true, "sizing": "80" } \] } \[/block\] _What’s the plus in using a Dialog Data Collector?_ First of all, it is now possible to collect data in a conversational way, more friendly for customers than forms. Secondly, through it can now to collect data in all channels, excepted for the Twilio Voice one. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/652e894-04.png](https://files.readme.io/652e894-04.png)", "04.png", 729, 1196, "\#bacce0" \], "border": true, "sizing": "smart" } \] } \[/block\] [➡ Read about the "Dialog Data Collector" in our documentation](doc:vcb-data-collection#section--dialog-data-collection-)
* The second one is a traditional bot that you can develop using Dialogflow, Watson or another AI engine and train it in the way you prefer to ask the needed information. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/aed305e-03.png](https://files.readme.io/aed305e-03.png)", "03.png", 2452, 1720, "\#fbfbfb" \], "border": true, "sizing": "80" } \] } \[/block\] [➡ Read about the "Bot Data Collector" in our documentation](doc:vcb-data-collection#section--bot-data-collection-)

### 2. Boost your Campaign strategy

#### Early chat: click and talk!

A new feature that will improve the effectiveness of your campaign is the Early Chat. The Early Chat allows to simulate, on the customer side, an ongoing chat even if the customer have not interact with it, while, on the agent side, the contact will only be enqueued after the first customer's message. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/7a69af0-05.png](https://files.readme.io/7a69af0-05.png)", "05.png", 730, 1194, "\#e2eaf2" \], "border": true, "sizing": "smart" } \] } \[/block\]

#### Differentiate your Media offer with Media Presets and Proposed Media

In the previous version of Vivocha, the available interaction modes were the same before and during the contact and, if the agent were not available or something went wrong, the customer simply received an apology message. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/fdd1df3-08.png](https://files.readme.io/fdd1df3-08.png)", "08.png", 2030, 1120, "\#f8f8f8" \], "border": true, "sizing": "80" } \] } \[/block\] You can now configure different interaction mode scenarios using the Media Presets in the Proposed Media section. Media presets are configurations of a single or multiple Media and each preset can have a set of configuration like Data Collection and Business hours. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/a68f627-07.png](https://files.readme.io/a68f627-07.png)", "07.png", 3346, 1604, "\#d0d0d0" \], "border": true, "sizing": "80" } \] } \[/block\] [➡ Read about the "Media Presets" in our documentation](doc:vcb-media-presets)

In the Proposed Media section, starting from a specific event \(like the Engagement, Timeout, No Agents, etc\) it is possible to create different Media configurations to be shown to the user, based on the available Media at the moment.

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/0f2aa34-06.png](https://files.readme.io/0f2aa34-06.png)", "06.png", 2102, 2130, "\#f8f8f8" \], "border": true, "sizing": "80" } \] } \[/block\] [➡ Read about the "Proposed media" in our documentation](doc:vcb-web-engagement-widgets#section--proposed-media-)

## Minors

### 3. New Data Collection features

New field types that allows to create an increasingly effective Data Collection are now available. A specific mention is required for two fields now available: break and section. The Break field allows to segment your Data Collection in multiple pages in order to create a pagination. The Section field, on the contrary, allows to merge multiple Data Collections, into a single one. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/7a24b69-09.png](https://files.readme.io/7a24b69-09.png)", "09.png", 2228, 932, "\#f8f8f8" \], "border": true, "sizing": "80" } \] } \[/block\]

### 4. Interaction App

The Interaction App's graphic style has been improved and its functionalities increased. It now supports more template messages and the screen sharing has a new and more useful layout. The Interaction app can also be embed in a specific area of your web page using a CSS selector. Use the power of the AI We improved the configuration of Bot Agents and connected Bot filters. Now it is possible to set up bots and filters to build a “library” and then separately connect filters to multiple bots only in a second instance, where needed. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/56f6765-10.png](https://files.readme.io/56f6765-10.png)", "10.png", 746, 1188, "\#d7e2ec" \] } \] } \[/block\]

### 5. Improve the effectiveness of your Webleads with the Interaction modes

Until now the Weblead could only be used in the Engagement phase. With the new Interaction modes configurable, at Engagement level, in the Proposed media section it is possible to use the Weblead to recover contacts that have been dissuaded or because there were no available agents or an error has occurred. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/6bedb62-11.png](https://files.readme.io/6bedb62-11.png)", "11.png", 1986, 1168, "\#fbfbfb" \], "border": true, "sizing": "80" } \] } \[/block\]

### 6. External Services

The Library has been enriched with the External Services section: an area where you can set up a lot of third party services like:

* Twilio
* Media hooks
* Web hooks
* External router
* Bot Agent
* Bot filter.

All settings have been simplified and the way Vivocha interfaces to third-party services has been standardised. We added the ability to configure Media Hooks and External routers globally in order to make it possible to use them in different Campaigns and we made it so easy that there is no need of technical skills to configure them. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/6932b50-12.png](https://files.readme.io/6932b50-12.png)", "12.png", 3346, 1172, "\#cdcdcd" \], "border": true, "sizing": "80" } \] } \[/block\] [➡ Read about the "External Services" in our documentation](doc:vcb-external-services)

