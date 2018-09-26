---
title: "Mobile Applications"
excerpt: ""
---
[Entry Points](#section--entry-points-)
[&nbsp;&nbsp;&nbsp;&nbsp;Entry points General Settings](#section--entry-points-general-settings-)
[&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Bundle ID](#section--bundle-id-)
[&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Push notification](#section--push-notifications-)
[&nbsp;&nbsp;&nbsp;&nbsp;SDK Download](#section--sdk-download-)
[Engagement](#section--engagement-)
[&nbsp;&nbsp;&nbsp;&nbsp;Engagement General Settings](#section--engagement-general-settings-)
[&nbsp;&nbsp;&nbsp;&nbsp;Style](#section--style-)
[&nbsp;&nbsp;&nbsp;&nbsp;Translations](#section--translations-)
<br>

Mobile Applications represent another channel that it's possible to support into a campaign.

They allow you to communicate not only with customers that browse your websites, but to continue giving your best customer service even when they use your mobile apps.

#**Entry Points**
You can configure different mobile applications as separate entry points by integrating our **Android and iOS SDKs.**

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/11b5f3c-Mobile_Applications.png",
        "Mobile Applications.png",
        1434,
        822,
        "#c3bebd"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
The Entry Points section presents all the configured Mobile Application entry points in the campaign.

To add a new one click on the **Add Android** or **Add iOS** button in the main card. It will opens the General section to set main settings of it. 

It's also possible to disable all the entry points in the channel selecting the checkbox field.

Each Mobile Application is represented by a box reporting information such as the name, the activation flag, an icon showing the SDK type and the button &nbsp;:fa-ellipsis-v:&nbsp; that give access to the commands to disable it, edit its settings and delete it.
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
By clicking on the name in each box the Mobile Application configuration panel opens.

##**Entry points General settings**
The General panel of a Mobile Application entry point looks the same for both the SDKs but it differentiates in some configuration options.

In the top configuration cards you set the name of the Mobile Application and its state.

The state of the Entry Point determines if it's active or not. By disabling it stops receiving contacts from this Mobile Application
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
      "image": []
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
        "https://files.readme.io/b733cc5-MobileApp-Push-Android.png",
        "MobileApp-Push-Android.png",
        837,
        484,
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
        "https://files.readme.io/833748d-MobileApp-Push-iOS.png",
        "MobileApp-Push-iOS.png",
        839,
        481,
        "#f7f7f7"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
The checkbox **use development server** allows to 

##**SDK Download** 
From this panel it's possible to download the SDK's that you will use to integrate your Android and iOS applications in Vivocha. By clicking on the Download SDK button you can save the corresponding package file in a folder in your file system.

Along with the relative SDKs versions, both for Android and iOS is provided a code sample that show how to import it and how to add the call to the Vivocha function by specifying your account id and your service id.

**Android**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/86a07ce-android_SDK.png",
        "android SDK.png",
        840,
        492,
        "#f6f5f6"
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
        "https://files.readme.io/5ae8ffe-iOS_SDK.png",
        "iOS SDK.png",
        839,
        459,
        "#f5f5f5"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
#**Engagement**
The mobile engagements allow you to link one or more Entry Point with a configuration of colors and translations to reuse for your apps.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/d0fb395-MobileApp-engagemts.png",
        "MobileApp-engagemts.png",
        1434,
        822,
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
  "body": "It's important to point out that a single Mobile application can be linked only with an engagement at a time, whereas a single engagement can shared by more applications"
}
[/block]
To configure a new engagement click on the **Add engagement** button in the main card. It will opens the General section to set main settings of it.

The Engagement section presents all the configured engagements for the Mobile App Channel which can be associated to the existing entry points.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/8f8035c-Screen_Shot_2018-03-07_at_17.14.51.png",
        "Screen Shot 2018-03-07 at 17.14.51.png",
        840,
        460,
        "#f5f5f5"
      ],
      "border": false,
      "sizing": "80"
    }
  ]
}
[/block]
Each one is represented by a box reporting information such as the name, a series of icons providing further details on the state and the settings of the widget and the button &nbsp;:fa-ellipsis-v:&nbsp;    that give access to the commands to edit and remove it.

the &nbsp;<span style="color:#dd565a">:fa-filter:</span>&nbsp; icon indicates that this engagement is not associated to any Mobile Application set for the channel

##**Engagement general settings**
The General panel allows to:
* set the name of the engagement
* bind it to one or more configured mobile applications that share the same style
* decide whether to use the custom theme or the one configured in the mobile application 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/1c5b557-MobileApp-engagemts-general.png",
        "MobileApp-engagemts-general.png",
        1382,
        947,
        "#f8f8f8"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
##**Style**

In this panel you can configure the color and layout properties for both the sidetab label (engagement) and interaction window of the Mobile application

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