---
title: "Vivocha 6.0 Release Notes"
excerpt: ""
---
[1. Campaign Builder a.k.a the new Foundry](#section-1-campaign-builder-a-k-a-the-new-foundry)
[2. New Engagement Widgets and Interaction App](#section-2-new-engagement-widgets-and-interaction-app)
[3. Bot integration](#section-3-bot-integration)
[4. Messages Templates](#section-4-messages-templates)
[5. Agent Console improvements](#section-5-agent-console-improvements)
[6. New architecture based on containers](#section-6-new-architecture-based-on-containers)
<br>


Here we are, time flows quickly and markets go ahead at a fast pace. 
The business and tech worlds are changing and our customers' needs changed as well. With Vivocha 5 we think we gave the perfect answer to our customers' requests but nowadays the scenarios are more complex than before and then we worked to improve the Vivocha experience. 

We gathered around the table and rethinked our product to make it more powerful, giving it a new look and new awesome features.

It's been a long year of study and development, a lot of work has been done by our team and now we are really proud to announce the new Vivocha 6!
Among the lots of features you can read about in the following lines we would like to highlight the brand new Campaign Builder which is the results of the experience gained over the years in the business and our customers' suggestions. To create it we had to rewrite our entire codebase and, trust us, it was not a piece of cake!

Our work has been motivated by the aim to make the interaction between users and agents easier and enjoyable. We tried our best to create the new interfaces that make it easy to create and setting up the new Campains and to improve your website users' experience with new beautiful engagement widgets and interaction apps.

Along with the Campaign Builder, we are releasing new tools that have been designed specifically for developers. It's now possible to download widgets' and interaction apps' source code, use it as boilerplate to create awesome new UIs and features and then upload it again to be served by Vivocha.


## 1. Campaign Builder a.k.a. the new Foundry
Simpler, smarter and more beautiful, once again!

The Campaign Builder is a brand new tool introduced with Vivocha 6 that allows administrators to define in a simple way a set of strategies and rules whose ultimate purpose is to let a group of agents to provide support by a variety of different Channels.

The Campaign Builder introduces a new set of concepts that are completely new on Vivocha, starting from the concept of *Campaign* itself, which the new Foundry is named after.

The *Campaign* extends the concept of *service* of the previous Foundry. Whereas services allowed the configuration of simple proactivity rules and the layout of a single Engagement Widget for each service, with the new Campaigns it is now possible to define a more complete and complex set of strategies and rules, applied to different interaction Channels.

We call Campaign a **set of engagement strategies, proactivity rules and specific constraints** that encloses defined business objectives and allows to a particular target of customers or prospects whom the Campaign is addressed, to reach a designated group of agents to receive online support.

So, differently from the services for which was often necessary to duplicate the rules as many times as the number of Engagement Widgets, languages and Channels (Mobile, Facebook, Web, etc.), a single Campaign can manage the configurations of many Entry Points, from different sites, languages, Media or communication Channels that share the same target of customers.

With the new Vivocha Campaign Builder, is easier and more effective than ever to interact with your customers.
With the previous Foundry the services were very easy to set up, but technical knowledge was required in order to make deeper customizations while with the new Campaign Builder it is **not necessary to own technical skills** to set up a Campaign. Its settings allow to do a deep customization without the use of a single line of code. As mentioned before, developers will have access to a deeper level of customisation.

New Campaigns are flexible and rich of features. An example? It's now possible to **activate or deactivated a Media** for the entire Campaign or only for a specific Channel or Engagement.
It's now possible to **start a contact with Voice or Video Media**, while with the previous version it was required to start a contact with a _chat_ and then perform a media upgrade. This opens to new possibilities on the user experience side.

We have also embedded in the Campaigns a new concept of  **opening hours** to help you optimize your business performance. With _opening hours_ you can tell Vivocha to start and stop automatically the entire Campaign, a specific Channel, Entry Point or Engagement by defining the contact center's business hours and its exceptional closures.

Last but not least, it's now possible to **make changes to a Campaign while it is active without interrupt it**. You can save the edited Campaign as **draft**, test it without stopping the production version and, only when you are sure, **publish** the changes and overwrite the previous version.

[➡ Read about the "Campaign Builder" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-campaign-builder-interface)

### 1.1. Multi-channel
The Campaign supports **different Channels** in which are applied the strategies and the rules that allow to request contacts. 

**What do we mean with *Channel*?**

A Channel can be, for example, the web but also a smartphone native app, a social network like Facebook, SMS and other messaging systems and telephony as well. A Campaign can use all or only some of the supported Channels. 

[➡ Read about "Channels" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-channels)

**From where contacts arrive to each Channel of my Campaign?**
Every Channel used in the Campaign can have one or more Entry Points. An **Entry Point** is the _source_ from where the contacts can actually be requested.

Specifically, an Entry Point for the web Channel is a website, for Facebook is a Facebook page and for SMS and telephony it is a phone number.

A single Campaign can use the following Channels:

#### Web
As in the past, the web Channel allows to engage websites' and web pages' visitors. The great news is that, setting up the web Channel, visitors can be engaged **from every kind of device** they are using to surf the web, be it a desktop, a tablet or a smartphone.

As said earlier, websites and web pages are the **Entry Points** for the web Channel. 

In a single Entry Point it is also possible to **include or exclude specific pages**, domains or **define limitations** based, for example, on specific words or paths. 
[block:callout]
{
  "type": "info",
  "body": "It is possible to create **multiple Entry Points** with different groups of web pages inclusions and exclusions and use them for different purposes."
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b8b8f4a-ep-web-rules.png",
        "ep-web-rules.png",
        500,
        438,
        "#f9f9f9"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
On this Channel, the interaction with a user starts through an **Engagement**. 
An Engagement consists in how (the Engagement's appearance) and where (the Entry Points associated to the Engagement) the users' attention will be captured.
[block:callout]
{
  "type": "info",
  "body": "It is possible to create multiple **Engagements** with different behaviours, Entry Points and look and feel to reach different business goals."
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b8fa286-widget.png",
        "widget.png",
        774,
        536,
        "#f2f3f2"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
The web Channel also allows to customize the **Interaction App** that users will use during the contact with the agents. The Interaction App is entirely customizable in features and look and feel: if you can imagine it, you can create it!
[block:callout]
{
  "type": "info",
  "body": "Engagement and Interaction App are responsive and allow to engage your visitors both from desktop and mobile devices."
}
[/block]
[➡ Read more about the "web Channel" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-web)

#### Smartphone
The smartphone Channel allows the agents to interact with users on **mobile native apps**.
**Apps are the Entry Points** for the smartphone Channel that supports iOS and Android apps and each app represents a smartphone Entry Point.
[block:callout]
{
  "type": "info",
  "body": "Each smartphone Entry Point corresponds to a single App."
}
[/block]
A new concept introduced for this Channel is the **theme**.

Smartphone Entry Points must be associated with a **theme**, which represents a set of customizable settings - including colors and labels - used by the mobile SDKs to engage and interact with your users.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/786b899-smartphone.png",
        "smartphone.png",
        1000,
        750,
        "#d2d8dd"
      ],
      "border": false,
      "sizing": "full"
    }
  ]
}
[/block]
[➡ Read more about the "smartphone Channel" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-smartphone)

#### Facebook
Facebook represents another Channel that it's possible to configure on a Campaign. As well as from the website, it allows the agents to be contacted by users from the Facebook page of your company, providing them the chance to send a message through the Messenger application.

On Vivocha, a **Facebook page represents a single Entry Point** for the Facebook Channel. It's possible to set as many Entry Points as the Facebook pages from where your users may contact the agents. This was made possible by the Vivocha integration with the Facebook Messenger platform.

[➡ Read more about the "Facebook Channel" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-facebook)

#### SMS
The SMS Channel makes possible to provide help to users using SMS and now it is possible to add it to a Campaign and handle this kind of contacts through the Vivocha Agent Console, as for the other kinds of contact.
[block:callout]
{
  "type": "info",
  "body": "This Channel is based on the Twilio technology, the same we use to manage inbound calls and callbacks."
}
[/block]
[➡ Read more about the "SMS Channel" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-sms)

#### Telephony
The telephony Channel allows agents to handle contacts that came from an inbound phone number and insert them into a specific Campaign's strategy. 
[block:callout]
{
  "type": "info",
  "body": "This Channel is based on the Twilio technology."
}
[/block]
### 1.2. Multi-media
Despite the foundry, the Campaign Builder allows to **choose which media are available and who can escalate** during the conversation (agent or user). Another news introduced by the interaction application it's the possibility to **start a contact automatically with the media video or voice**, without escalating from the chat.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/16512db-media.png",
        "media.png",
        500,
        298,
        "#fafbfa"
      ],
      "border": false,
      "sizing": "80"
    }
  ]
}
[/block]
With the Campaign Builder you can turn on a Media for all Campaign's Channels and it will be available only for the Channels from which they are supported by.
[block:callout]
{
  "type": "info",
  "body": "Though a Media is active and the Channel supports it, it will be available only if the agent and the customer owns the right hardware to support the Media."
}
[/block]
[➡ Read more about "Media" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-media)

#### Recontact options
Recontact options are another great news. They an extension of two features of the previous foundry: *Callback now/later* and *web leads*. That tools allow users to ask to be contacted from the agents in different ways.

The recontact options can be used in the way that suits better your business needs: 
- when the user requests it
- when all the agents are busy and nobody can handle the contact
- when a timeout or another error occurred
- always.

The Campaign builder allows to use **three different possibilities for the recontact**:
- E-mail 
- SMS
- Phone

With the SMS and phone recontact, the incoming contacts can be now handled in two different ways: 
- *manually*, using external accounts and supports
- directly on the Vivocha agent console, using a Twilio account.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/770caaf-recall-card.png",
        "recall-card.png",
        500,
        421,
        "#f9f9f9"
      ],
      "caption": "",
      "border": false,
      "sizing": "80"
    }
  ]
}
[/block]
For the phone requests it is also possible to accept **real time requests** or to allow customers to **book an appointment** to be recalled from an agent. In the second case it is necessary to configure the slots. 
[block:callout]
{
  "type": "info",
  "body": "> Slots can be configured using a webhook or manually creating intervals of time or slots, as preferred."
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/724f2ea-slot-settings.png",
        "slot-settings.png",
        500,
        325,
        "#f9f9f9"
      ],
      "border": false,
      "sizing": "80"
    }
  ]
}
[/block]
### 1.3. Multi-language
Finally the same Campaign can manage **multiple languages**. All the Widgets and the Interaction App can be configured inside the same Campaign to serve users from different countries without creating a specific Campaign for each one duplicating all the settings except the language.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/858f091-a8799f4-languages_2.png",
        "a8799f4-languages_2.png",
        500,
        359,
        "#fafaf9"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
#### Language Detection Strategies
To manage the multi-language support Vivocha already provides a set of language detection strategies out of the box.

- **Domain**: This strategy is based on recognizing the country code top-level domain (ccTLD).
- **User-agent**: This strategy is based on recognizing the language from the User-Agent info of the customer's browser.
- **GEOIP**: It's based on the geo localization of the IP address of the device used by the visitor.
- **URL**: It checks if in the URL is present a language code.

You can decide which strategies to use based on your web site architecture. You can also decide to use more than one strategy giving them the right priority or, otherwise you can decide to use a **Custom Javascript Code** that allows you to write the code to detect the language.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/79d41fb-bfd26a4-WEB-Entry_point_languages-8.png",
        "bfd26a4-WEB-Entry_point_languages-8.png",
        500,
        452,
        "#f4f4f4"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]

[block:callout]
{
  "type": "info",
  "body": "Please note that you can also add languages that are not directly supported by the configuration interface of the Vivocha platform."
}
[/block]
[➡ Read more about the "Languages" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-languages)

### 1.4. Hierarchical Configuration Settings
To made everything most simple and quick to set up, **some strategic settings are inherit and can be overwritten at different nesting level of a Campaign.

The hierarchy is the following:
- **Campaign**: is the first level of configuration and the most general. 
- **Channel**: 
	- **Entry Point**: this is the second level of configuration. By default it inherits the Campaign configurations but they can be overwritten to reach specific strategic purposes;
	- **Engagement**: this is a third level of configuration and it is specific for the web Channel. By default it inherits its Entry Points configurations but they can be overwritten to reach specific strategic purposes.
<br>
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/4603a29-hierarchy.png",
        "hierarchy.png",
        1587,
        622,
        "#8492a0"
      ],
      "border": false,
      "sizing": "80"
    }
  ]
}
[/block]
<br>
It follows that the configurations made on a web Engagement have more priority than the Campaign's one.

The settings on we are talking about are three:
- Media
- Routing
- Opening Hours

[➡ Read more about "Hierarchical configuration settings" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-campaign-builder-overview)

### 1.5. New Proactive engine
The new features introduced by the Campaign Builder have necessarily involved important changes on the way the proactive engine works on customer pages.

Rules are now checked continuously, and changes in the variables (whether you decide to use built-in rules or decide to create your own), are constantly tracked to show or hide the engagement widgets.

Everything is now managed by a brand new FSM that manages all the states of the customer interaction automatically returning to the starting point once a contact is closed or some values changed in the rules' variables.

#### 1.5.1 Rules based on Variables
It is now possible to engage your website visitors in the best moment of the user journey through the creations of specific *proactive rules*.

It is possible to define conditions by choosing between the variables of the builtin group or by creating custom variables. Builtin variables allow you to create conditions based on user's behaviours, country, spoken languages and a lot more.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/c0e60f9-rules.png",
        "rules.png",
        976,
        422,
        "#fafafa"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]

[block:callout]
{
  "type": "info",
  "body": "It is allowed the creation of multiple conditions, all in an _logical and_ relationship with each other, that need to be satisfied to engage the user."
}
[/block]
### 1.6. Library
Another great concept introduced in the Campaign Builder is the **Library**.

Library is like a toolbox for your Campaigns. Here you can create different kind of tools that you will use every time you need, when you are creating a Campaign. 

Here you can find: 
- Custom Variables
- Data Collections and Surveys

[➡ Read more about the "Library" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-campaign-builder-interface#section- -library-)

#### 1.6.1. Custom Variables
It is now possible to create different type of custom Variables:
- **Selector Variables**
- **Javascript Variables**
- **WebService Variables**
[block:callout]
{
  "type": "info",
  "body": "Custom Variables can be used for creating proactive rules or to autofill a Data Collection field."
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/e363151-variables.png",
        "variables.png",
        852,
        638,
        "#fcfcfc"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
[➡ Read more about the "Custom Variables" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-custom-variables)

#### 1.6.2. Data Collection
Data Collections allow to collect information about the user and are now more flexible and useful.
You can create different Data Collections and decide to use them to ask some data to your users **before the contact starts**, **when the contact ends** or **when they need to be recontacted**. The great thing is that now it is possible to get this data automatically using a variable and maybe ask to the user only to confirm them.

You can now associate the same Data Collection to one or more Engagements, even in different Campaigns, or use them as Surveys to know the users' satisfaction.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b2b6e59-data-collection.png",
        "data-collection.png",
        1413,
        882,
        "#c7c7c7"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
[➡ Read more about the "Data Collection" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-data-collection)

### 1.7. Developer tools
If on the one hand we have substantially simplified the Campaign creation, focusing on the definition of business configurations, proactive rules, and simple widget display settings, on the other hand we worked to build a set of tools that will be actually appreciated by developers.

Development tools released on Vivocha 6.0 are separated from the Campaign Builder and are strictly designed by developers for developers.

- Offline Widget development;
- Import/Export of custom Widgets
- Import/Export of translation strings

So developers can now download the widget code from Vivocha, edit the code from the favourite editor, test the widget using the Vivocha offline preview mode, and finally push the widget to the Vivocha servers. And everything can be done preserving (or adding new) configuration variables for the people who will then include the new widget in the Campaign Builder.

Developer Command Line tool is already available as NPM package for Node.js [vvc](https://www.npmjs.com/package/vvc). Sources are also available on GitHub [vvc](https://github.com/vivocha/vvc).
[block:code]
{
  "codes": [
    {
      "code": "npm install -g vvc",
      "language": "shell"
    }
  ]
}
[/block]
## 2. New Engagement Widgets and Interaction App
Are now available new **Engagement Widgets** with different styles that will help you to engage users in the best way. Each Engagement Widget is entirely customizable: it is possible to customize images, the brand logo, colors, fonts and much more. Is it not enough? It is possible to add your custom CSS!
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/f8c119f-widget-builder.png",
        "widget-builder.png",
        1414,
        880,
        "#a39b99"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
The current available Engagement Widgets are:
- Popup
- Sidetab
- Halo
- Button

[➡ Read more about the "Engagement Widgets" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-web#section- -engagement-widgets-doc-vcb-web-engagement-widgets-)
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2fc6f95-Screen_Shot_2018-03-30_at_18.59.12.png",
        "Screen Shot 2018-03-30 at 18.59.12.png",
        960,
        504,
        "#f0e9e8"
      ]
    }
  ]
}
[/block]
The **Interaction App** too is entirely customizable in its appearance and in its features. For example it is possible to decide if activate or not the **Emoji support** or the **file transfer**.

[comment]: <> (<-- TODO ![Interaction App](file missed) -->)

[➡ Read more about the "Interaction App" in our documentation](https://vivocha.readme.io/v6.0/docs/vcb-interaction-app)

## 3. Bot integration
Today, building conversational chatbots involves composing software applications able to understand natural-language inputs, and following a predefined decisional “script” in order to properly interact with customers and chat users, simulating a real human conversation. Under the hood, AI and Machine Learning algorithms are used to instruct chatbot systems and to improve their ability to understand what humans are saying or asking for in several application domains.

Vivocha 6.0 supports natively the bots integration and automatically manages the contact routing without the requirement of building complex orchestration apps to manage the bot communication and the transfer to human agents, as required on Vivocha version 5.4.

[➡ Read more about the "Bots" in our documentation](https://vivocha.readme.io/v6.0/docs/bots)

#### Bots as virtual agents
The bots are managed as virtual agents, so it's possible to manage the bot skills and routing priority assigning tags. It's also possible to transfer a contact from a human agent to a bot and vice versa just like transferring the contact between humans.

Reports are not changed. Bots activity and performances can be evaluated through the standard reporting for agents and contacts.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/ae1f690-screenshot_bot.png",
        "screenshot_bot.png",
        1392,
        912,
        "#d9d9d8"
      ],
      "border": false,
      "sizing": "80"
    }
  ]
}
[/block]
#### Data collection integration
Bot agents can be linked to Data collection objects. So a properly configured bot can collect customer data to speed up the job of the human agents. Another possibility is to use data already collected from the page, that can be provided by the customer or retrieved from variables, to give custom answers to the customer's requests (e.g. propose special offers based to geographical origin of the customer).

#### Multi-vendor support
Vivocha 6.0 provides out-of-the-box support for chat bots built using IBM Watson Assistant (formerly Conversation) and Dialogflow platforms. This means that it is possible to integrate these particular bots implementation with Vivocha simply using the Vivocha configuration app and specifying few settings, like authentication tokens and following some, very simple, mandatory guidelines when building the bots, at design time.
More vendors will be supported in the next versions. Meanwhile you can use the Bot SDK to build your own driver. The Vivocha Bot SDK also provides convenient facilities to write Vivocha compliant chat bots which use the Wit.ai NLP platform. Moreover, using the Bot SDK it is also possible to write vendor-neutral custom chat bots from scratch, integrating (or not) other bot / NLP platforms.

#### Bot REST API
The REST API allows to write Vivocha Bot Agents integrating existing bots, built and trained using your preferred bot / NLP platform (E.g., Dialogflow, IBM Watson Assistant, Wit.ai, etc...). By creating a BotManager it is possible to register multi-platform bot implementations and let Vivocha communicate with them through a well-defined, clear and uniform message-based interface.
We already provide an SDK for [node.js](https://nodejs.org), get it from the following link: [Vivocha Bot SDK](https://github.com/vivocha/bot-sdk)

#### Filters

In order to maximize the flexibility and the extensibility of its bot model, the Vivocha 6.0 platform introduces the concept of Bot Filter.
A Bot Filter is a chainable web microservice able to augment a Bot Request or a Bot Response (or both).
Therefore, thanks to BotFilters chains we can enrich / manipulate requests before they reach the Bot implementation or platform (like Watson Assistant or Dialogflow) and to manipulate / enrich / transform responses coming from a Bot implementation or platform before they reach the customer chat.
For example, a BotFilter can enrich a request coming from a user calling an external API or access to a database to get additional data before sending it to a Bot Agent, or it can filter a response coming from a Bot Agent to transform the data it contains before forwarding it to a user.

The Vivocha Bot SDK and REST APIs can be also used to quickly create Bot Filters.
(See more here: [bot filters](https://github.com/vivocha/bot-sdk#bot-filters)).

## 4. Messages Templates
Another great feature introduced by Vivocha 6, that is strictly linked to user experience with bot agents, are the message templates.
The message templates enrich the conversation experience giving the possibility to interact with images, buttons and links rather than plain text messages. Templates can be used for different purposes: speed up the interaction with some suggestion of supported quick answers, provide a visual example of a product proposed to the customer, or direct the user to a precise set of possible answers.

Below is the list of supported message templates:

#### Quick replies
It shows some suggestions to the customer, that can choose to select one of those instead of typing it in order to speed up the conversation. Clicking on a quick reply will result as the customer actually typed that text in the chat area.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b2e99ef-screenshot_quick.png",
        "screenshot_quick.png",
        350,
        579,
        "#e6f4ee"
      ],
      "border": true
    }
  ]
}
[/block]
#### Simple Buttons
Unlike the *quick replies* if the customer select one of the buttons options it will be sent a *postback* message to the other side.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/effb94a-screenshot_buttons.png",
        "screenshot_buttons.png",
        350,
        579,
        "#cfdce9"
      ],
      "border": true
    }
  ]
}
[/block]
#### Templates
Templates are structured to extend the simple buttons including a title, subtitle and an image.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/ab66169-screenshot_template.png",
        "screenshot_template.png",
        350,
        579,
        "#c7cdd3"
      ],
      "border": true
    }
  ]
}
[/block]
#### Templates with carousel
It's also possible to send more sets of buttons and templates with multimedia contents. In this case templates are shown in a carousel layout, providing the possibility to choose between multiple templates.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/f2d071b-screenshot_carousel.png",
        "screenshot_carousel.png",
        350,
        579,
        "#d0dcd5"
      ],
      "border": true
    }
  ]
}
[/block]
#### Custom actions
Buttons can also trigger custom actions that must be sent to the page instead of the usual *postback* message.
You can configure the custom action behavior using the *campaign builder* and configuring your your custom JavaScript code for the event *contact-custom-event*.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b928d75-screenshot_customev.png",
        "screenshot_customev.png",
        1232,
        854,
        "#a6a6a6"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
#### Multi-channel compatibility
Message templates are available for the following channels:
- Web
- Facebook Messenger
- Mobile SDK

This means that you can use the same bot to manage contacts coming from different channels that have the same routing rules.
In particular, the message template format is designed to be compliant with the Messenger templates provided by the Facebook API. See [here](https://developers.facebook.com/docs/messenger-platform/send-messages?locale=en_US) to have more info about the templates supported by Facebook Messenger.

## 5. Agent Console improvements
Vivocha 6 introduces three popular features requests into the chat area in the Agent Console:
- Multi-line messages
- Chat balloons
- Message timestamp
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/e3d2dff-screenshot_console.png",
        "screenshot_console.png",
        427,
        337,
        "#deebf5"
      ]
    }
  ]
}
[/block]
## 6. New architecture based on containers
This version introduces major changes in the back end architecture. In particular we organized our application in micro services and introduced a new server architecture based on containers.
In terms of advantages this new architecture grants an higher scalability and, at the same time, allow us to be more independent from the cloud provider.

[comment]: <> (stackedit_data: eyJoaXN0b3J5IjpbODk4OTY2NDQ1XX0=)
[block:callout]
{
  "type": "info",
  "body": "[Vivocha 5.0 Release Notes](http://docs.vivocha.com/v5.0/docs/release-notes) - your domain is mX.vivocha.com\n[Vivocha 5.2 Release Notes](http://docs.vivocha.com/v5.2/docs/version-52) - your domain is nX.vivocha.com",
  "title": "If you currently run a different version of the Platform, please read about the relative Release Notes:"
}
[/block]