---
title: "Interaction app"
excerpt: ""
---
[Settings](#section--settings-)
[Style](#section--style-)
[Translations](#section--translations-)
<br>

The Interaction app is the Vivocha component which manage the whole interaction between the agent and the user, the exchange of messages and the sending/receiving of attachment files, the displaying of data collection forms as well as the possibility to request a voice or a video call if the feature is enabled.

On the user side the widget of the Interaction app, just as the Engagement widget has its own style, settings and string translations that you can personalize in order to support all the languages used in the Campaign and so that it may better fit the aspect of the pages where it is supposed to display.

The Campaign Builder comes out with a default Interaction widget whose settings can be customized in three panels.
[block:callout]
{
  "type": "warning",
  "body": "in case you have different Interaction apps available in your account, in the first panel  named **General** you can select the one you want to use in the Campaign"
}
[/block]
#**Settings**
The Interaction app presents a series of settings that you can configure in order to change the aspect and some of the behaviours of its standards components or to settle whether one or more features have to be enabled or disabled.

All the parameters listed in Settings represent the properties of the Interaction app that can be configured by simply switching them on or off. These are settings that allow you to carry out some changes to the look and behaviours of the interaction app without having to modify nothing in its code.
[block:callout]
{
  "type": "info",
  "body": "The Interaction app default configuration is declared along with all the properties made configurable at design time in the **Manifest file** of the app itself, so that once the app is loaded in the account, you can set them up directly from this interface of Campaign Builder.<br>\nMore than a single interaction app, each one with its own features and properties may be pushed into an account and then used with the Campaigns"
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/d71432f-settings-2.png",
        "settings-2.png",
        1899,
        1200,
        "#fafafa"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
Here are the Interaction app default configuration parameters and their descriptions:

###**Ask confirm on close**
If enabled the user is asked if he really want to leave the chat when he clicks on close button; the message displayed in the close modal is set in the relative section in the Translations panel.
[block:image]
{
  "images": [
    {
      "image": []
    }
  ]
}
[/block]
###**Let the user see the transcript after close**
If enabled the interaction widget is not immediately closed after clicking the close button allowing the user to keep seeing the messages transcript

###**Hide upload button when connected with a BOT**
If enabled, the paperclip icon for the files' upload is hidden when the user is connect with a BOT.

###**Show avatar in the Topbar**
If enabled the avatar of the agent who takes the contact is shown in the topbar of the Interaction App.

###**Show agent info in the Topbar**
If enabled the name of the agent who takes the contact is shown in the topbar of the Interaction App. Otherwise if disabled, the Topbar will show a title and subtitle set by default in the Topbar section of the Translations panel.

###**Allow the visitor to display emoji panel**
If enabled the emoji panel is displayed to the visitor by clicking on the smiling face icon.

###**Allow the user to send file to the agent**
If enabled the user is allowed to send a file to the agent by clicking on the paperclip icon.

###**Allow the visitor to enter in chat before the agent (Early Chat)**
If enabled, when the user request for a chat the Interaction app opens without to show the contact request to agents: actually the contact has not started yet and the agents see it in the console only after the user has sent the first message.

To enabling this setting allows to implement the so called "Early Chat" feature. Also the following two settings in the panel allow to determine the way this feature has to work.

###**Show welcome message on Early Chat**
If enabled, when the Early Chat starts a welcome message is shown inviting the user to make his request.

###**Show connection to agent message (Early Chat)**
If enabled, when the Early Chat starts and after the user has sent his first message a further message is shown to him informing of  the connection to the first available agent 

###**Display welcome message when the agent is connected to the chat**
If enabled when the agent accepts the chat a default welcome message is shown. The message you want to appear is set up in in the Chat section of the Translations panel.

###**Show user avatar in chat message**
If enabled the avatar of the user is shown beside messages he is going to send. Consecutive messages are grouped and the avatar is shown only beside the one on top. Consecutive messages are grouped and the avatar is shown only beside the one on top with the sending time of the last message displayed under them.

###**Show arrow in the user balloon chat message**
If enabled the user's dialogue balloons are rendered with a tail pointing toward the user side in the Interaction app. Consecutive messages are grouped and the tail is shown only beside the one on top with the sending time of the last message displayed under them.

###**Show agent's avatar on chat**
If enabled the avatar of the agent who takes the contact is shown beside messages he is going to send. Consecutive messages are grouped and the avatar is shown only beside the one on top with the sending time of the last message displayed under them.

###**Show arrow's balloon for the agent**
If enabled the agent's dialogue balloons are rendered with a tail pointing toward the agent side in the Interaction app. Consecutive messages are grouped  and the tail is shown only beside the one on top with the sending time of the last message displayed under them.

###**Message received audio notification**
If enabled, messages sent by the agent are notified to the user by a chime sound effect.

#**Style**
The Style panel allow to configure the main graphical properties of the Interaction Widget and its theme settings.

In the first card you can edit the main color used within the Interaction app. Just like for the Engagement Widget you can take advantage of the HTML5 color picker component that allow you to change and the set the color 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/a684536-style-style.png",
        "style-style.png",
        830,
        404,
        "#e8e7e7"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
###**Asset File**
The logo can be changed by loading a default logo or the preferred immage as asset for the Interaction app
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/486ad1b-style-assets.png",
        "style-assets.png",
        820,
        433,
        "#fbfbfb"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
###**Custom CSS**
Just like for the Engagement Widget, also the Interaction app can be customized by adding custom CSS to apply style properties changes
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/a53bf3c-Screen_Shot_2018-03-20_at_13.29.29.png",
        "Screen Shot 2018-03-20 at 13.29.29.png",
        1004,
        588,
        "#f4f0f1"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
###**CSS Selector**
... you have to insert the name of this selector (i.e: #id, .class)


#**Translations**
For all the languages supported in the Campaign it is possible to configure the translations used by the Interaction app. This means that like for the Engagement Widget, you can provide the strings properly translated to better convey messages and information for each supported language.

The Interaction app is more complex than the Engagement widget and since it handles many features it also have many more messages and strings that may be displayed at  a specific moment and scenario.
[block:callout]
{
  "type": "info",
  "body": "Advanced tools for the developers introduced in Vivocha 6 allow the full access to the code of the Interaction app and allow to define further properties for the app making them configurable directly from the Campaign Builder, after you load it into the system."
}
[/block]
After selecting the language all the possible strings, whose translations need to be provided, are shown grouped in categories based on the functionality.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/177af52-Screen_Shot_2018-03-21_at_11.58.52.png",
        "Screen Shot 2018-03-21 at 11.58.52.png",
        843,
        756,
        "#f6f6f6"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
So you can provide the right translations for the strings shown when media tools are in use or for the messages that appear when specific actions are carried out
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/6ea59f3-VCB-IntApp-translations_3.png",
        "VCB-IntApp-translations 3.png",
        1440,
        980,
        "#fcfcfc"
      ],
      "border": false,
      "sizing": "full"
    }
  ]
}
[/block]