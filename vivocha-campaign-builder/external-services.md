---
title: External Services
excerpt: ''
---

# External Services

[Twilio](external-services.md#section-twilio) [Webhook](external-services.md#section-webhook) [Mediahook](external-services.md#section-mediahook) [External Router](external-services.md#section-external-router) [Bot Agents](external-services.md#section-bot-agents) [   IBM Watson Assistant](external-services.md#section--ibm-watson-assistant-) [   Dialogflow](external-services.md#section--dialogflow-) [   Custom](external-services.md#section--custom-) [   Filters](external-services.md#section--filters-) [Bot Filters](external-services.md#section-bot-filters)   


Third Party Services are external services interfaced with Vivocha to change or extend its feature. Here you can set up different kind of services like Web Hooks, Media Hooks, External Routers, Bot Filters and Bot Agents.

Once configured these services can be used within the Campaigns to which they need to be linked. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/cb99724-Screen\_Shot\_2018-09-13\_at\_16.45.37.png](https://files.readme.io/cb99724-Screen_Shot_2018-09-13_at_16.45.37.png)", "Screen Shot 2018-09-13 at 16.45.37.png", 1422, 809, "\#c8c8c8" \], "border": true, "sizing": "80" } \] } \[/block\] To add a new External Services click on the Add new button in the main card. It will opens the Service settings section to start to configure the service giving it a **name**, a **description** and selecting its **type**. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/9bfa597-Screen\_Shot\_2018-09-13\_at\_17.19.35.png](https://files.readme.io/9bfa597-Screen_Shot_2018-09-13_at_17.19.35.png)", "Screen Shot 2018-09-13 at 17.19.35.png", 1090, 401, "\#f8f8f8" \], "sizing": "80", "border": true } \] } \[/block\] Further parameters to set up will be displayed depending on the selected type of service.

## Twilio

You can configure the integration between Vivocha and Twilio platform \(www.twilio.com\) to handle the voice services: Inbound, Outbound, SMS.

If you already have a Twilio account, you need to copy the **ACCOUNT SID** and **AUTH TOKEN** \(see the API Credentials in your Twilio account\) in the configuration page then click on the Save button to save it into the System. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/bda8fc6-Twilio.png](https://files.readme.io/bda8fc6-Twilio.png)", "Twilio.png", 1030, 632, "\#faf9f9" \], "border": true, "sizing": "80" } \] } \[/block\]

## Webhook

Webhooks, are web services that can be used for the CTI integrations by subscribing to the available events of new, end, change, finalized, message.

When the subscribed events occur in a campaign linked to the webhook, Vivocha notifies it with a HTTP\(S\) POST request to your web service that then can use these data, manage them to produce reports and statistics, ecc...

It's possible to not apply any authentication method or select one of the two options:

* Basic: it requires to enter the user and secret parameters.
* Bearer: it requires to enter the secret parameter.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/9449b36-Screen_Shot_2018-09-13_at_18.36.19.png",
    "Screen Shot 2018-09-13 at 18.36.19.png",
    1049,
    740,
    "#f9f9f9"
  ],
  "border": true,
  "sizing": "80"
  ```

    }

  \]

  }

  \[/block\]

  **Mediahook**

  Media hooks are a type of webhooks that allows you to use an external service to calculate agent availability, defining the way in which media are shown to the users on the Engagement.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/3d7b889-mediahook.png",
    "mediahook.png",
    1020,
    643,
    "#fbfbfb"
  ],
  "sizing": "80",
  "border": true
  ```

    }

  \]

  }

  \[/block\]

  **External Router**

  The External Router is also another type of webhook that allows external routing settings to be used, overwriting the Vivocha Routing settings.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/7c80e01-Screen_Shot_2018-09-13_at_18.58.50.png",
    "Screen Shot 2018-09-13 at 18.58.50.png",
    1060,
    597,
    "#fbfbfb"
  ],
  "border": true,
  "sizing": "80"
  ```

    }

  \]

  }

  \[/block\]

\[block:callout\] { "type": "warning", "body": "In order to use these three type of external services so configured with your Campaigns, you only have to access to the corresponding [Hooks](doc:vcb-routing#section--hooks-) section and set a link for each of them you want to use." } \[/block\] In order to use these three type of external services so configured with your Campaigns, you only have to access to the corresponding Hooks section and set a link for each of them you want to use.

## Bot Agents

You can configure integrations between Vivocha and external services represented by bots, built and trained using bot / NLP platform. E.g., Dialogflow, IBM Watson Assistant \(formerly Conversation\), Wit.ai, etc...

The bot agents services here configured can be used along with data collection forms to collect data before or after a contact without to really generate it.

[➡ Read about the "Bot Data Collection" in our documentation](doc:vcb-data-collection#section--bot-data-collection-)

Otherwise you may want to associate it to a virtual agent that acts as like a real agent able to chat with users, help them in solving common issues then ultimately close contacts or transfer to "really human" agents.

[➡ Read about the "How to set up a Virtual agent "](doc:bots)

Vivocha 6 out-of-the-box supports Dialogflow \(Google\) and IBM Watson Assistant \(formerly Conversation\), and Wit.ai \(Facebook\)\*\* Natural Language Platform \(NLP\) through the Vivocha Bot SDK. \[block:callout\] { "type": "info", "body": "Following this link you have access to the Vivocha TypeScript/JavaScript Bot SDK with code, resources and example along with a complete and detailed guide that describes how to create Vivocha Bot Agents and Filters [https://github.com/vivocha/bot-sdk](https://github.com/vivocha/bot-sdk)" } \[/block\] Once selected bot agent as type of service you have to set up the parameters for its configuration that vary depending of the bot engine used to develop it, and eventually set up also the bot filters that you intend to use with it. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/62767d1-Screen\_Shot\_2018-09-14\_at\_10.39.50.png](https://files.readme.io/62767d1-Screen_Shot_2018-09-14_at_10.39.50.png)", "Screen Shot 2018-09-14 at 10.39.50.png", 1040, 630, "\#f8f8f8" \], "border": true, "sizing": "80" } \] } \[/block\]

### **IBM Watson Assistant**

IBM Watson is en extremely poweful computing system for the ArtificiaI Intelligence, comprehensive of a range of products and services including **Assistant**, a platform to create applications that understand natural-language and able to respond to customers in a human-like conversation and in multiple languages. [**More info**](https://github.com/vivocha/bot-sdk#ibm-watson-assistant-integration-guidelines) \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/d036d01-wtason.png](https://files.readme.io/d036d01-wtason.png)", "wtason.png", 1057, 438, "\#f8f8f8" \], "border": true, "sizing": "80" } \] } \[/block\] In order to integrate an implementation of a bot builded with Assistant it is necessary to specify few settings:

The parameters marked with the \(\*\) mean that are mandatory.

**Workspace ID \*:**  A workspace is where the natural language processing takes place and the container for all the resources that define the conversation flow for an application. A workspace identifies a single Bot application and has its corresponding ID.

**Username \*:**  the username of the specific instance of the service IBM Watson Assistant in use.

**Password \*:**  the password of the specific instance of the service IBM Watson Assistant in use.

**Version:** The specific APIs version of Watson Assistant used to build the Bot.

### **Dialogflow**

Dialogflow is also a platform for developing human-computer interaction applications that allows to create conversation flows using machine learning to understand what users are saying. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/24201ac-dialogflow.png](https://files.readme.io/24201ac-dialogflow.png)", "dialogflow.png", 1060, 372, "\#f7f7f7" \], "border": true, "sizing": "80" } \] } \[/block\] Dialogflow required parameters are:

**Token \*:**  The access token for authentication associated to the bot.

**Start Event:** It is the name of the event that triggers the _intent_ that starts the bot. Must exists in Dialogflow a configured intent which exactly matches the start event. [**More info**](https://github.com/vivocha/bot-sdk#dialogflow-integration-guidelines)

### **Custom**

IBM Watson Assistant and Dialogflow are the Bot engines for which built-in drivers are provided. In addition to the out-of-the-box support for these two platforms, the Vivocha Bot SDK and the Vivocha Bot APIs also provide the possibility to implement new more drivers that allow to create and integrate new Bot agents using these drivers to directly communicate with different \(external\) Bot Platforms.

The Bot SDK also includes all the facilities to easily integrate **Wit.ai** based applications, speeding up the process of implementing the dialog flow and to write custom chat bots from scratch. [**More Info**](https://github.com/vivocha/bot-sdk#wit-ai-writing-chat-bots) \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/c9f68a5-custom.png](https://files.readme.io/c9f68a5-custom.png)", "custom.png", 1047, 742, "\#bababa" \], "border": true, "sizing": "80" } \] } \[/block\] In order to integrate a custom bot implementation it is necessary to provide some parameters and eventually specify few settings:

**URL \*:** The URL of a custom application implementing our Bot APIs according the SDK provided and that represents the bot.

**Settings:** a JSON object can contain couples of key-value settings necessary to integrate the custom bot.

**Authentication:** It's possible to not apply any authentication method or select one of the two options:

* **Basic auth**: requires to enter the _bot-user_ and _bot-secret_ parameters.
* **Bearer auth:** requires to enter the _bot-secret_ parameter.

### **Filters**

[Bot Filters](doc:vcb-external-services#section-bot-filter) are Web services that augment, adapt or transform the BotRequest before it is received by the Bot Agents and before they return back a BotResponse to the Vivocha platform.

In this panel you select which request and response filters you want to add to the Bot Agent you are configuring. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/ea3c2ca-Screen\_Shot\_2018-09-14\_at\_11.15.56.png](https://files.readme.io/ea3c2ca-Screen_Shot_2018-09-14_at_11.15.56.png)", "Screen Shot 2018-09-14 at 11.15.56.png", 1061, 726, "\#f9f9f9" \], "border": true, "sizing": "80" } \] } \[/block\]

\[block:callout\] { "type": "warning", "body": "Please note that the order the filters are added is important since they are run following a waterfall execution policy" } \[/block\]

## Bot Filters

The Bot SDK also allows to create the [**Filters**](https://github.com/vivocha/bot-sdk#bot-filters). These are applications that allow to work around the limitations intrinsic in some Bot platform, by adding the logic augmenting the Bot intelligence and its capabilities in carrying out some tasks and providing it with the ability to dynamically interact with the users. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/df273ba-Screen\_Shot\_2018-09-14\_at\_12.03.00.png](https://files.readme.io/df273ba-Screen_Shot_2018-09-14_at_12.03.00.png)", "Screen Shot 2018-09-14 at 12.03.00.png", 1075, 375, "\#f8f8f8" \], "border": true, "sizing": "80" } \] } \[/block\] Bot Filters are Web services that augment, adapt or transform the [**BotRequest**](https://github.com/vivocha/bot-sdk#botrequest) before it is received by the Bot Manager/Bot Agents and before they return back a [**BotResponse**](https://github.com/vivocha/bot-sdk#botresponse) to the Vivocha platform.

It is also possible to chain several Bot Filters in order to have specialized filters related to the application domain.

Examples of Bot Filters can be web services that:

* add skill-based routing rules.
* implement bounce back logics: if an agent does not respond you can make sure to send it to another bot.
* add information on the prediction of waiting times.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/400ae29-BotFilter.png",
    "BotFilter.png",
    1064,
    799,
    "#c5c5c5"
  ],
  "border": true,
  "sizing": "80"
  ```

    }

  \]

  }

  \[/block\]

  Filter's configuration requires to specify few settings:

**URL \*:** The URL of a web service application implementing our Bot APIs according the SDK provided and that represents the filter.

**Authentication:** It's possible to not apply any authentication method or select one of the two options:

* **Basic auth**: requires to enter the _bot-user_ and _bot-secret_ parameters
* **Bearer auth:** requires to enter the _bot-secret_ parameter

**Settings:** A Filter can explicit a set of specific settings inside a JSON object

