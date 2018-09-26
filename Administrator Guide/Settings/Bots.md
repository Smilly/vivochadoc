---
title: "Bots"
excerpt: ""
---
[General](#section--general-)
[Agent](#section--agent-)
[Data Collection](#section--data-collection-)
[Transfer](#section--transfer-)
<br>

Concept is that Bots or chat bots in Vivocha can be seen as Virtual Agents. Thus, like real agents, they can chat with users, help them in solving common issues, perform data collection tasks, then ultimately close contacts or transfer to "really human" agents.

Vivocha Bot Agents are multi platform by design, that means you can configure a sort of chat bots or Bot Manager with multiple agents that use different Bot Implementation/platform: a chat bot can consists of a bot agent builded with IBM Watson Assistant for English language and, at the same time, by a Dialogflow-based agent for the Italian mother-tongue customers; it is also possible to build custom bots using other platforms or writing them from scratch.

[➡ Read about the "Bot Agents external services" in our documentation](doc:vcb-external-services#section-bot-agents)

The Vivocha settings section for Bots allows to:
- create a Bot Manager by setting a series of parameters necessary to add virtual agents that integrate multiple bot implementations/platforms
- register multi-platform virtual agents using different languages. 
- link data collection objects for collecting information from the chat bot users.
- configure transfer settings to human agents.

In this section of the Settings is the list with all the chat bots/Bot manager configured and the corresponding main information. 

Click on **New Bot** button to create a new one or on the corresponding &nbsp;:fa-cog:&nbsp; button in the actions on the right to edit an existing one. To delete permanently a chatbot click on the &nbsp;:fa-times-circle-o:&nbsp; button
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/98fcf4b-Screen_Shot_2018-09-14_at_12.35.03.png",
        "Screen Shot 2018-09-14 at 12.35.03.png",
        1434,
        698,
        "#e4e4e4"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
#**General**
In this panel are provided some general info about the chat bot you're going to configure.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/3123fcb-Screen_Shot_2018-09-14_at_12.31.46.png",
        "Screen Shot 2018-09-14 at 12.31.46.png",
        1255,
        781,
        "#e8e9ec"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
**Avatar**
Simply the image shown to the users when interacting with the chat bot.

**Name**
The mandatory field that identify the chat bot

**Nickname**
The name appearing to the users when interacting with the chat bot

**Language**
The default language associated to the chat bot. If not specified, language associated is the general one set for the account.
[block:callout]
{
  "type": "warning",
  "body": "You must configure at least one agent supporting the default language for the chat bot"
}
[/block]
**Tags**
The tags associated to the chat bot. Just as for a real agent, a chat bot and the relative agents need to have assigned a tag or a set of these, in order that incoming contacts from a Campaign can be distributed also to them.

#**Agent**
As mentioned chat bots in Vivocha are seen as virtual agents; in this panel you configure these bot agents that will interact with customers.

Each bot agent is identified by the couple ***Language-Engine***. That means that when you create a new bot agent you specify the language it will use to communicate with the chat users and the engine/Bot platform on which this implementation is based on.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/0798a77-Screen_Shot_2018-09-14_at_12.39.08.png",
        "Screen Shot 2018-09-14 at 12.39.08.png",
        1430,
        780,
        "#f0f0ef"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]

[block:callout]
{
  "type": "warning",
  "body": "**You cannot configure more than one bot agent for each language.**\n\nThus it means that you cannot have a bot agent builded with IBM Watson Assistant and at the same time a Dialogflow-based agent both answering to English customers."
}
[/block]
Click on **Add new agent** button above the list to add a new bot agent to the Bot manager or, if you want to edit an existing one, click the relative :fa-cog: button on the right. To delete permanently a bot agent click on the &nbsp;:fa-times-circle-o:&nbsp; button.

After selecting the language you have to choose one of the available Bot Agents configured in the External Services of the Library
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/5555cbd-Screen_Shot_2018-09-14_at_12.39.35.png",
        "Screen Shot 2018-09-14 at 12.39.35.png",
        1198,
        675,
        "#efeeee"
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
  "body": "In order to properly work with Vivocha and take advantage of the out-of-the-box support it provides, it is mandatory to follow the guidelines when building the bots at design time. <br>\nFor each of the Bot platform currently supported these are fully explained in the document at the section https://github.com/vivocha/bot-sdk#supported-bot-and-nlp-platforms."
}
[/block]
#**Data Collection**
Chat bots can be integrated with data collections and use them to communicate with chat bots users. Data collections are those set for the account and are configured in the **[Library within the Campaign Builder](doc:vcb-data-collection)**

So the information asked to fill the Data Collection widget presented at the time the contact starts, or that can be collected directly from a web page thanks to the definition of custom variables and then used to fill it automatically, can also be transmitted to the bot.
At this point it can use and modify them or eventually to ask for more info ,and at the end move them back to our system for the routing and distribution to a human agent.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/e2f642c-Screen_Shot_2018-09-14_at_12.51.35.png",
        "Screen Shot 2018-09-14 at 12.51.35.png",
        1019,
        648,
        "#eeeeed"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
#**Transfer**
The Bot can transfer a contact to an agent or to a group of agents that share the same tags. At the same way the bot can also receive a contact transferred from an agent.
[block:callout]
{
  "type": "info",
  "body": "If both real and bot agents are configured and have an equivalent *weight* to determine the distribution of the contact, the transfer to a real agent takes precedence. This happens when the routing strategy selected is the Broadcast; This routing algorithm assigns the same score to all agents and consequently contacts are distributed to all those available in the same moment."
}
[/block]
To let the bot performs the transfer, at design time it's necessary to define a **transfer-key**, whom is associated a value which in turn is mapped to a tag for transfer to a group of agents, or directly to an agent ID for the transfer to a single agent. A more detailed explanation about how a chat bot fires a transfer to a human agent can be find **[here](https://github.com/vivocha/bot-sdk#about-vivocha-bots-and-transfers-to-human-agents)**.

To add  new **transfer to tag** and **transfer to agent** rules click on the respective **Add** button.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/26a0cb3-Screen_Shot_2018-09-14_at_12.54.22.png",
        "Screen Shot 2018-09-14 at 12.54.22.png",
        1436,
        784,
        "#ededed"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]