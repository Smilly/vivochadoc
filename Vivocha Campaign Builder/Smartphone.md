---
title: "Smartphone"
excerpt: ""
---
[Smartphone Entry Points](#section--smartphone-entry-points-)
[&nbsp;&nbsp;&nbsp;&nbsp;App General Settings](#section--app-general-settings-)
[&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Bundle ID](#section--bundle-id-)
[&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Push notification](#section--push-notifications-)
[&nbsp;&nbsp;&nbsp;&nbsp;SDK Download](#section--sdk-download-)
[Themes](#section--themes-)
[&nbsp;&nbsp;&nbsp;&nbsp;Theme General Settings](#section--theme-general-settings-)
[&nbsp;&nbsp;&nbsp;&nbsp;Style](#section--style-)
[&nbsp;&nbsp;&nbsp;&nbsp;Translations](#section--translations-)
<br>

Mobile native apps, that here we'll call mobile apps or simply apps, represent another type of Entry Points and the Smartphone a further Channel that it's possible to support into a Campaign.

They allow you to communicate with users that browse your websites and also let you keeping to provide your best customer service even when they want to use your mobile app.

#**Smartphone Entry Points**
You can configure different apps as separate Entry Points for the smartphone Channel by integrating our **Android and iOS SDKs.**

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/8d6298c-Screen_Shot_2018-03-28_at_12.39.18.png",
        "Screen Shot 2018-03-28 at 12.39.18.png",
        1439,
        820,
        "#c3bebc"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
The Entry Points section presents all the configured mobile apps set in the Campaign.

To add a new one click on the **Add Android** or **Add iOS** button in the main card. It will opens the General section to set main settings of it. 

It's also possible to disable all the Entry Points in the Channel selecting the checkbox field.

Each mobile app is represented by a box reporting information such as the name, the activation flag, an icon showing the SDK type and the button &nbsp;:fa-ellipsis-v:&nbsp; that give access to the commands to disable it, edit its settings and delete it.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/fbd3787-entry_points-1.png",
        "entry points-1.png",
        837,
        550,
        "#f5f5f5"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
By clicking on the name in each box the mobile app configuration panel opens.

##**App General settings**
The General panel of a mobile app Entry Point looks the same for both the SDKs but it differentiates in some configuration options.

In the top configuration cards you set the name of the app and its state.

The state of the Entry Point determines if it's active or not. By disabling it stops receiving contacts from this mobile app.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/9dc0b1f-MobileApp-general.png",
        "MobileApp-general.png",
        837,
        699,
        "#f7f7f7"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
In the cards at the bottom you manage the bundle ID of a single application and eventually set the push notifications

###**Bundle ID** 
Is a string in reverse DNS format using only letters, periods and hyphens. It must be the same as the bundle ID for your iOS application that you would like to integrate with Vivocha.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/025f0fe-Screen_Shot_2018-03-28_at_13.06.55.png",
        "Screen Shot 2018-03-28 at 13.06.55.png",
        837,
        324,
        "#f8f8f7"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
###**Push Notifications** 
If activated when the app is closed the user will receive a notification for a message from the agent.

Depending on Android or iOS the configuration options are different.

**Android**
You must insert the server key string if you would like to use the push notifications. 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/7e950f3-Screen_Shot_2018-03-28_at_14.55.14.png",
        "Screen Shot 2018-03-28 at 14.55.14.png",
        832,
        444,
        "#f8f8f8"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
**iOS**
You must insert the certificate string and key string if you would like to use the push notifications
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/80b2132-Screen_Shot_2018-03-28_at_14.56.56.png",
        "Screen Shot 2018-03-28 at 14.56.56.png",
        832,
        484,
        "#f7f8f7"
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
  "body": "When **use a development server** checkbox is selected, given certificate and private key will be used with the *Apple Push Notification Service* Sandbox endpoint."
}
[/block]
##**SDK Download** 
From this panel it's possible to download the SDK's that you will use to integrate your Android and iOS applications in Vivocha. By clicking on the **Download SDK** button you can save the SDK's corresponding package in a folder in your file system.

Along with the relative SDKs versions, both for Android and iOS is provided a code sample that shows how to import it and how to add the call to the Vivocha function by specifying your Account ID and the ServID, which is composed by the ID's of the Campaign and of the mobile native Entry Point.

**Android**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/cba5876-Screen_Shot_2018-03-28_at_15.04.24.png",
        "Screen Shot 2018-03-28 at 15.04.24.png",
        840,
        501,
        "#f5f4f5"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
**iOS**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/1c6dbe5-Screen_Shot_2018-03-28_at_15.04.24.png",
        "Screen Shot 2018-03-28 at 15.04.24.png",
        840,
        501,
        "#f5f4f5"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
#**Themes**
Themes act as the engagements for the mobile native apps and they can be linked to one or more of them, so that different apps could share the same a configuration of colors and translations.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/efab29b-Screen_Shot_2018-03-28_at_13.16.28.png",
        "Screen Shot 2018-03-28 at 13.16.28.png",
        1436,
        825,
        "#c2bdbc"
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
  "body": "It's important to point out that a single Mobile application can be linked only with a theme at a time, whereas a single theme can shared by more applications"
}
[/block]
To configure a new theme click on the **Add theme** button in the main card. It will opens the General section to set main settings of it.

The Theme section presents all the configured themes for the smartphone Channel which can be associated to the existing apps that represent the Entry Points.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/ddab96b-Screen_Shot_2018-03-28_at_15.21.18.png",
        "Screen Shot 2018-03-28 at 15.21.18.png",
        839,
        544,
        "#f5f5f5"
      ],
      "border": false,
      "sizing": "80"
    }
  ]
}
[/block]
Each one is represented by a box reporting information such as the name, a series of icons providing further details on the state and the settings of the widget and the button &nbsp;:fa-ellipsis-v:&nbsp;    that give access to the commands to edit and remove it.

the &nbsp;<span style="color:#dd565a">:fa-filter:</span>&nbsp; icon indicates that this theme is not associated to any mobile app set for the Channel

##**Theme general settings**
The General panel allows to:
* set the name of the theme.
* bind it to one or more configured mobile app that share the same style.
* decide whether to use the custom theme or the one configured in the mobile app.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2d160ec-Screen_Shot_2018-03-28_at_15.19.04.png",
        "Screen Shot 2018-03-28 at 15.19.04.png",
        1380,
        942,
        "#f6f6f6"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
##**Style**

In this panel you can configure the color and layout properties for both the sidetab label, for the engagement, and interaction window of the mobile app

###**Colors**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/ab1953e-Style.png",
        "Style.png",
        840,
        756,
        "#f8f8f8"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
**Background color of your sidetab:** choose the background color of your sidetab

**Text color for your sidetab:** choose the text color for your sidetab

**Chat balloon background color for the agent :** choose the background color that the customers will see for the agent's balloon when chatting

**Chat balloon text color for the agent** choose the text color that the customers will see for the agent when chatting

**Background balloon color for customer:** choose the background color that the customers will see for their balloon when chatting

**Text balloon color for customer :** choose the text color that the customers will see for themselves when chatting

**System messages color** the color of the text that appears for system messages.

**Background Chat Color:** background color that appears behind the balloons

**Send button background color:** choose the color for the background of the send button

**Color of the send message button text ** choose the color for the text on the send button
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/362f1a6-Screen_Shot_2018-03-14_at_15.04.35.png",
        "Screen Shot 2018-03-14 at 15.04.35.png",
        734,
        470,
        "#e4e9ec"
      ],
      "sizing": "80"
    }
  ]
}
[/block]
###**Layout**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/9eee462-Style-layout.png",
        "Style-layout.png",
        836,
        602,
        "#f9f9f9"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
**Sidetab side position:** choose which side you would like your sidetab to appear on (top, bottom, left, right)

**Sidetab alignment position:** after choosing a side, decide how you would like your sidetab to be aligned (top, middle, bottom, left, right)

**Roundness of the corners of the chat balloon**: define the roundness of the corners of the chat balloon

**Chat background image name:** the name of the image present in the application bundle that will be used as the chat's background image
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/435b1b8-Screen_Shot_2018-03-14_at_14.56.26.png",
        "Screen Shot 2018-03-14 at 14.56.26.png",
        676,
        401,
        "#c9c9c9"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
##**Translations**
in the tab Translations you indicate the text you want to display in ther sidatab label of the Mobile app for all the languages enabled in the Campaign.

To apply the changes to the translations click the specific button.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/f99d79e-Translations.png",
        "Translations.png",
        842,
        661,
        "#f7f7f7"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]