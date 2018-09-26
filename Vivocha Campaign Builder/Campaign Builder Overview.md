---
title: "Campaign Builder Overview"
excerpt: ""
---
The Vivocha Campaign Builder is a brand new tool introduced with Vivocha 6, that allows administrators to define in a simply way a set of strategies and rules whose ultimate purpose is to let a group of agents to provide support by a variety of different Channels.

The Campaign Builder is all about the concepts of Campaign, Channels, Entry Points, Engagements Widget and Interaction app, Layered Inheritance, Proactive rules, Event Handlers and many others.

New principles and goals have driven the development of the Campaign Builder to get a new smart, simple tool to work with, whose main features and peculiarities are:
- full customisation of the Campaigns and Widgets allowed to different levels
- developer and ops friendly
- advanced engagements supporting more multimedia scenarios without coding
- Multi language
- Custom Language Detection Strategies
- brand new Proactive Engine that runs continuously
- Rich set of builtin Data Capture Variables
- Custom Data Capture Variables
- Custom Event Handlers
- optional guided approach
- contextual documentation

We are going to describe all these mentioned features and their working in the different pages of this part of our documentation.

Before to go down on each section it's important to explain the main aspects and concepts and the first one is the Campaign. What is it a campaign? 

A Campaign is a set of engagement strategies, proactivity rules and specific constraints that enclose defined business objectives, that allow to a particular target of customers or prospects whom the campaign is addressed, to reach a designated group of agents to receive online support.

Starting from the outlined objectives, within the Campaign Builder you are provided a series of features to design a new Campaign by defining the desired strategies and  setting up rules and behaviours to establish the way it works and how you want provide online support to an audience of users that can be customers, prospects or simply the visitors of the official website and the company facebook page, or the users of the official mobile application.

This may consists for example in configuring:
- its validity, setting up an the interval in which the Campaign starts and stops
- business hours to limit hours and days in which agents receive contacts from the Campaign.
- the communication Channels through which contacts can be requested, and the media types they support to interact with the agents.
- the languages supported and the strategies to detect the correct one to use depending on situation.
-  a data collection form to obtain information that will help agents handle customers' requests.
-  a survey form to present at the end of the contact to evaluate the quality of the received support.

These and other configurations, including the possibility to adapt the 'Look & feel' of the Engagement and the Interaction app according the brand identity of the customer, are fully customisable without the necessity to write any code but simply by taking the advantage the rich set of features provided within the Campaign Builder.
[block:callout]
{
  "type": "info",
  "body": "In addition to the provided options within the Campaign Builder, new **advanced developer tools** introduced with Vivocha 6 allow to extend these options and to edit the HTML, CSS and JavaScript code of the Engagement Widgets and Interaction apps."
}
[/block]
The Campaign can have different Channels in which are applied the strategies and the rules that allow to request contacts. Each of these Channels used in the Campaign, in turn, can have one or more Entry Points from where contacts can actually be requested.

Channels are the web for example, but also a smartphone native app, social networks like Facebook, SMS and other messaging systems and naturally telephony as well.

Basically an Entry Point for the web Channel is a website, for Facebook is a Facebook page, whereas for SMS and telephony it is a telephone number.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2907faa-multlilayer_architecture-1.png",
        "multlilayer_architecture-1.png",
        1285,
        975,
        "#80898f"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
Depending on the type of Channel and Entry Point you can have a further sub-level which is the Presentation. For example in case of an organisation/company that want convey the Campaign's goals taking advantage of the web in such a way that the visitors from the website may get in touch with the help center, Presentation level is represented by the Engagement Widget and its relative graphical style.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/063a130-multlilayer_architecture-2.png",
        "multlilayer_architecture-2.png",
        1283,
        928,
        "#86888c"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
This model is so structured: the Campaign incorparate the Channels, which in turns incorporate the Entry Points that can furtherly incorparate more Presentation Widgets or eventually, if the Channel is different than web, another types of Engagements.

This allow to have a **Layered Inheritance** for the configurations that are set up at Campaign level going down to the available Channels, then to the Entry Points and the engagements widget.

At the same time many of the settings can be reconfigured in the lower levels, by modifying the general behaviours that are inherited from the Campaign, so you can create and set differently as many Channels and the associated Entry Points, depending on the specific needs and aims of the Campaign.

So you can have in website more than one Engagement Widget presented in different web pages or only if some determined conditions are satisfied.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/8678c45-multlilayer_architecture-3.png",
        "multlilayer_architecture-3.png",
        1283,
        947,
        "#848c91"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
The strategies of a Campaign could be applied on different websites.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/5d4199b-multlilayer_architecture-4.png",
        "multlilayer_architecture-4.png",
        1284,
        936,
        "#879197"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
Or, beyond the web, be implemented also on other Channels such Facebook on two different Facebook pages, or through a telephony service that could have one or more dedicated numbers.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/a906e07-multlilayer_architecture-5.png",
        "multlilayer_architecture-5.png",
        1285,
        945,
        "#83959e"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]