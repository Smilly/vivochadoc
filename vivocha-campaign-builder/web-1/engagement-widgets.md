---
title: Engagement Widgets
excerpt: ''
---

# Engagement Widgets

[General](engagement-widgets.md#section--general-) [    Web Entry Points](engagement-widgets.md#section--web-entry-points-) [    Widgets](engagement-widgets.md#section--widgets-) [Proposed media](engagement-widgets.md#section--proposed-media-) [Data Collection & Survey](engagement-widgets.md#section--data-collection-survey-) [Proactive Rules](engagement-widgets.md#section--proactive-rules-) [Events](engagement-widgets.md#section--events-)

An entry point, for the web channel, is a website and it needs one or more web engagement widgets to be associated with. They represent the presentation level and allow visitors to requests contacts.

Adding an engagement widget to an existing entry point consist in set how and where it will appear in the web page, defining its position and other style properties.

To add a new web engagement widget click on the **Add new** button in the main card. It will opens the [General](doc:vcb-web-engagement-widgets#section-general) section to set main settings of widget. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/6ebb03c-WEB-EW-main\_panel\_7.png](https://files.readme.io/6ebb03c-WEB-EW-main_panel_7.png)", "WEB-EW-main panel 7.png", 840, 566, "\#f4f4f4" \], "border": true, "sizing": "80" } \] } \[/block\] The Web Engagement Widgets section presents all the configured widgets for the Channel which can be associated to the existing entry points. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/a0ef3ac-WEB-EW-main\_panel\_8.png](https://files.readme.io/a0ef3ac-WEB-EW-main_panel_8.png)", "WEB-EW-main panel 8.png", 837, 243, "\#f2f2f2" \], "border": true, "sizing": "80" } \] } \[/block\] Each one is represented by a box reporting information such as the name, a series of icons providing further details on the state and the settings of the widget and the button  :fa-ellipsis-v:  that give access to the commands to edit and remove it.

The table reports the different icons that may be displayed for each engagement widget box and what they represent. \[block:parameters\] { "data": { "0-0": ":fa-filter:", "6-0": ":fa-bolt:", "3-0": ":fa-list-ul:", "5-0": ":fa-eye:", "0-1": "it indicates that this engagement widget is not associated to any entry points set for the channel", "3-1": "it indicates that this engagement widget has a data collection set", "5-1": "it indicates that this engagement widget has proactive rules configured", "6-1": "it indicates that this engagement widget has an event handler configured", "4-0": ":fa-star-half-empty:", "4-1": "it indicates that this engagement widget has a survey set", "1-0": ":fa-desktop:", "1-1": "it indicates that for this engagement widget a template has been selected", "2-0": ":fa-desktop:", "2-1": "it indicates that for this engagement widget a template has not been selected" }, "cols": 2, "rows": 7 } \[/block\] By clicking on the name in the box the engagement widget configuration panel opens.

## **General**

The General panel allows to set the name of the engagement widget, associate it to one or more entry points and to select the template you want to display for it. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/28a5ab3-WEB-EW-general\_2.png](https://files.readme.io/28a5ab3-WEB-EW-general_2.png)", "WEB-EW-general 2.png", 896, 764, "\#f5f6f6" \], "sizing": "80", "border": true } \] } \[/block\]

### **Web Entry Points**

There could be an entry point/website with more engagement widgets that have different styles and properties and it is also possible that a single engagement widget may be associated to more entry points and appear on different websites.

In the image below the engagement widget you want to add is associated to two entry point among the three available in Web Channel. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/9ec05f6-WEB-EW-general-EntryPoints.png](https://files.readme.io/9ec05f6-WEB-EW-general-EntryPoints.png)", "WEB-EW-general-EntryPoints.png", 837, 349, "\#f7f7f6" \], "sizing": "80", "border": true } \] } \[/block\]

\[block:callout\] { "type": "warning", "body": "A Web engagement widget initially may be also not associated to any Web entry points: it is set in web channel but never shown to visitors until it is not connected to at least an entry point, that is the website where it is supposed to be displayed.   
\nA Web engagement widget not associated to any entry point/website is marked out by the red icon :fa-filter: in the Web Engagement Widgets section list." } \[/block\]

### **Widgets**

By default the Campaign Builder provides 4 different styles for the engagement widget, each one with a different look and feel and properties, that you can select and immediately use for the associated entry point.

The possible styles provided by default for the web engagement widget are:

* the **Vivocha Popup** to engage the visitor by showing a multimedia popup.
* the **Vivocha Halo** to engage the visitor by showing an avatar image in the bottom right corner of the screen.
* the **Vivocha Sidetab** to engage the visitor by showing a side multimedia label.
* the **Vivocha Button** to engage the visitor by showing a button inside an HTML element of the page.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/f8f485b-WEB-EW-general-widget_2.png",
    "WEB-EW-general-widget 2.png",
    819,
    553,
    "#f1f2f2"
  ],
  "sizing": "80",
  "border": true
  ```

    }

  \]

  }

  \[/block\]

  When you click on the Configure button of the selected widget style a further tool opens: the [**Widget Builder**](doc:vcb-widget-builder).  

In it you have access to a preview of the widget showing how it will appear in page, and to the set of its properties that you can modify and which are different depending on the selected style. This is because each different type of widget declare what it is configurable and what it supports. \[block:callout\] { "type": "info", "body": "It's important to point out that the Widget Builder is a tool that allows to execute some types of customization in the widgets through a sort of wizard mode and a series of predefined setting fields, which vary depending on properties and peculiarities of that widget itself.   
\nIn addition to the the 4 default styles, Vivocha 6 introduces new advanced tools that allows to create new types of widgets, having the full access to the source code \(html, css, javascript\), test and manage them locally and import and export from and into the Campaign Builder.  
\nA brand new created widget will be available and selectable for web entry points, and just exactly as for a Vivocha default sidetab or a popup, their own properties can be configured inside the Widget Builder" } \[/block\]

## **Proposed media**

By default the widget displays the button for the chat, voice and video, depending on the agents' availability for each of these media: if there are not online agents available to manage a certain media, the widget does not show the relative button.

However it's possible to configure which media options to show in the widget both at the level of the Campaign accessing the [**Media Section**](doc:vcb-media) or at the level of every single engagement in its Proposed media section.

It's possible to configure different combination of the media to create multiple interaction proposals used according to specific engagement rules, events that might occur, based on the working hours, ecc...

Interaction modes so defined can be configured for each of this type of event, as explained below and shown in the next image:

* **Engagement:** when the widget is shown into the pages and users can request a contact.
* **No agents available:** when there are no more available agents to handle the contact request with the chosen media; the widget has firstly showed the button of the media, but at the moment of the connecting with an agent, there's no longer availability on it.
* **Timeout:** when the dissuasion timer expires. The contact request has not been accepted by no one of the agents to whom was proposed before the expiring of the dissuasion timeout configured for it.
* **Error:** when an error occurs during the interaction and the contact stops
* **Closed:**when the contact has closed by the agent or the user 

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/1c77409-Screen_Shot_2018-09-12_at_17.12.33.png",
    "Screen Shot 2018-09-12 at 17.12.33.png",
    843,
    562,
    "#f3f3f3"
  ],
  "sizing": "80",
  "border": true
  ```

    }

  \]

  }

  \[/block\]

  For all these events you can create a sequence of media to propose to the user; after selecting the event by clicking the Configure button a panel opens and you can create a sequence of media presets to propose to the user in multiple ways.

When you configure an Interaction mode the chat preset is added by default but you could also decide to add further presets and change the sequence of how they are proposed.

For example, instead of the chat you can choose to show the media Video at first, and the Chat and Voice only if Video is not available. If instead all the three media are not available then the weblead is proposed. The steps to configure this Interaction mode are:

1. Click the Preset Button and select the Video from the **Built-in Presets** list and **OR** operator 

   \[block:image\]

   {

   "images": \[

    {

      "image": \[

   ```text
    "https://files.readme.io/d1d5881-Screen_Shot_2018-09-13_at_10.52.43.png",
    "Screen Shot 2018-09-13 at 10.52.43.png",
    855,
    534,
    "#fafafa"
   ```

      \],

      "sizing": "80",

      "border": true

    }

   \]

   }

   \[/block\]

\[block:callout\] { "type": "info", "body": "Those in the list are the presets supported by default by the system: chat, voice, video, sms, weblead. The platform also allow to create new custom presets that can be used to configure the Interaction modes, just as you do with the the built-in ones.  
 [➡ Read more about the \"Media Presets\" in our documentation](doc:vcb-media-presets)" } \[/block\] 2. Click the **Group** button to add a new group and then add inside it the single presets of Voice **AND** Chat

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/022ff9b-Screen\_Shot\_2018-09-13\_at\_12.18.21.png](https://files.readme.io/022ff9b-Screen_Shot_2018-09-13_at_12.18.21.png)", "Screen Shot 2018-09-13 at 12.18.21.png", 754, 616, "\#fbfbfb" \], "sizing": "80", "border": true } \] } \[/block\] 3. Click the on **Preset Button on top** to add the Weblead outside the group and select **OR** as operator \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/02394b1-Screen\_Shot\_2018-09-13\_at\_12.03.25.png](https://files.readme.io/02394b1-Screen_Shot_2018-09-13_at_12.03.25.png)", "Screen Shot 2018-09-13 at 12.03.25.png", 730, 604, "\#fbfbfb" \], "sizing": "80", "border": true } \] } \[/block\]

\[block:callout\] { "type": "info", "body": "Basically adding a group of presets is like opening the brackets in the formula that represents the logic functioning of a presets sequence so configured" } \[/block\] This is the reported formula of the Interaction Mode \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/2a57120-Screen\_Shot\_2018-09-13\_at\_12.20.01.png](https://files.readme.io/2a57120-Screen_Shot_2018-09-13_at_12.20.01.png)", "Screen Shot 2018-09-13 at 12.20.01.png", 738, 160, "\#f9f9f9" \], "sizing": "80", "border": true } \] } \[/block\] Each presets in the sequence of the Interaction mode can be furtherly configured adding advanced settings by accessing the panel that opens by clicking the relative  :fa-ellipsis-v:  and then the **Edit** option among the available commands that allow to change it moving every single preset **up** or **down** in the sequence and **in** or **out** a group. Finally you can also **remove** it. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/960a545-Screen\_Shot\_2018-09-13\_at\_14.44.19.png](https://files.readme.io/960a545-Screen_Shot_2018-09-13_at_14.44.19.png)", "Screen Shot 2018-09-13 at 14.44.19.png", 702, 348, "\#fafafa" \], "border": true, "sizing": "80" } \] } \[/block\] In the advanced settings section of each media preset of the sequence it's also possible to associate a data collection to it. This functionality allows to use a data collection only for the media presets where it is configured and not with the other media presets which are in the Interaction mode of the engagement.

This is what appear the advanced settings section for the weblead: you can associate a data collection and provide a contact email where all the webleads need to be sent. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/f323655-Screen\_Shot\_2018-09-13\_at\_15.49.00.png](https://files.readme.io/f323655-Screen_Shot_2018-09-13_at_15.49.00.png)", "Screen Shot 2018-09-13 at 15.49.00.png", 796, 593, "\#fafafa" \], "sizing": "80", "border": true } \] } \[/block\] You can also define new business hours and working days rules that let to show different media of the same engagement in different moments during the day or in different days.

back to the Interaction modes main section you will see a set of icons indicating the settings eventually activated beside each preset. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/119529e-Screen\_Shot\_2018-09-13\_at\_15.52.53.png](https://files.readme.io/119529e-Screen_Shot_2018-09-13_at_15.52.53.png)", "Screen Shot 2018-09-13 at 15.52.53.png", 646, 200, "\#fbfbfb" \], "border": true, "sizing": "80" } \] } \[/block\]

## **Data Collection & Survey**

An engagement widget can be configured in order that when a contact is requested a data collection form is presented to the customer before he start to interact with an agent

In this section you can link the engagement widget to a Data Collection form and to a Survey, previously defined in their own configuration sections in the [Library](doc:vcb-data-collection). \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/bdb0b1c-WEB-EW-dataCollectionSurvey.png](https://files.readme.io/bdb0b1c-WEB-EW-dataCollectionSurvey.png)", "WEB-EW-dataCollection&Survey.png", 843, 644, "\#f6f6f6" \], "sizing": "80", "border": true } \] } \[/block\] Data collection is handled by the interaction widget and its fields are automatically showed in it depending on a series of parameters.

A data collection can be filled manually by the customer, or if information are available in the page \(i.e. after logged into a private area of a website\) these can be directly fetched and pre-fill the form without showing it to the customer. Furthermore in this case it's also possible present a pre-filled data collection to give the opportunity to change some of the information automatically fetched.

All these scenarios are supported and can be configured at the time of the data collection definition in the Library section.

## **Proactive Rules**

Proactive rules allow the Engagement Widget to be displayed if certain conditions are verified. It is possible to define multiple rules, eventually group them and implement the logic that regulates how to show the widget.

Rules and groups can be combined each other by using the **AND/OR** operators to formulate expressions that will be evaluated and will determine whether to show the engagement widget or not. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/c42a1bb-Screen\_Shot\_2018-09-19\_at\_17.21.18.png](https://files.readme.io/c42a1bb-Screen_Shot_2018-09-19_at_17.21.18.png)", "Screen Shot 2018-09-19 at 17.21.18.png", 837, 593, "\#f7f7f6" \], "border": true, "sizing": "80" } \] } \[/block\] Clicking on the **Rule** button and expanding the panel you can select the variable that you want to evaluate against the selected operator and to a constant value or eventually against the value of another variable.

The **Group** button instead allows to configure an expression with more rules inside a block between brackets.

variables are selectable from the drop down list where you have the built-in ones that are provided data and information about the user activities in the website and gathered directly from the browser or the device in use. A complete list of them is [**here**](doc:vcb-proactive-rules-list) provided \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/0cee13a-Screen\_Shot\_2018-09-20\_at\_17.21.58.png](https://files.readme.io/0cee13a-Screen_Shot_2018-09-20_at_17.21.58.png)", "Screen Shot 2018-09-20 at 17.21.58.png", 809, 720, "\#fbfafa" \], "border": true, "sizing": "80" } \] } \[/block\] In addition to the built-in variables you can create proactive rules by using the custom variables you may have defined to collect data from website pages, take the results of some operations or from an external web service. Custom variables are listed at the bottom of the drop down list.

Each rule in the sequence can be edited at later time from the panel that opens by clicking the Edit button in the commands menu accessible clicking on the relative  :fa-ellipsis-v:  button. Other buttons allow to move the rule **up** or **down** in the sequence and **in** or **out** a group. Finally you can also **remove** it. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/7e1d395-Screen\_Shot\_2018-09-20\_at\_18.03.55.png](https://files.readme.io/7e1d395-Screen_Shot_2018-09-20_at_18.03.55.png)", "Screen Shot 2018-09-20 at 18.03.55.png", 779, 258, "\#fbfbfb" \], "sizing": "80", "border": true } \] } \[/block\]

## **Events**

Besides a brand new Proactive Engine that take advantage of a rich set of built-in data capture variables and custom data variables, the personalizzation of a Campaign with all its channels, entry points and widgets can be achieved also thanks the further powerful tool od the Custom Events Handlers. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/ccf855a-WEB-EW-events-1.png](https://files.readme.io/ccf855a-WEB-EW-events-1.png)", "WEB-EW-events-1.png", 958, 514, "\#f7f7f7" \], "border": true, "sizing": "80" } \] } \[/block\] An Event Handler runs your custom JavaScript code when specific event occurs.

So you can select one event among the available in the dropdown list, related with the webpage loading or with the status of the engagement widget or the contact, and configure it by hooking pieces of code which for example can execute specific actions like for example the evaluating of data and the its storage in a custom variable.

You can insert the javascript custom code directly in a editor by selecting the handler type **inline** \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/96e2f08-WEB-EW-events-2.png](https://files.readme.io/96e2f08-WEB-EW-events-2.png)", "WEB-EW-events-2.png", 945, 493, "\#bfc0c0" \], "border": true, "sizing": "80" } \] } \[/block\] or to make a call to an external code by specifying the corresponding web service endpoint URL.

It is also possible to specify if the code must be run every time that event occurs or only at the first time, and whether it is run asynchronously or not.

To remove an Event Handler click on the corresponding **Remove** button. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/020e984-WEB-EW-events-4.png](https://files.readme.io/020e984-WEB-EW-events-4.png)", "WEB-EW-events-4.png", 841, 560, "\#f9f9f9" \], "sizing": "80", "border": true } \] } \[/block\]

