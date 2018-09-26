---
title: "Custom Variables"
excerpt: ""
---
[Custom variable settings](#section--custom-variable-settings-)
[&nbsp;&nbsp;&nbsp;Variable Identifier](#section--variable-identifier-)
[&nbsp;&nbsp;&nbsp;Variable Data Type](#section--variable-data-type-)
[&nbsp;&nbsp;&nbsp;Variable Type](#section--variable-type-)
[&nbsp;&nbsp;&nbsp;Value replacement](#section--value-replacement-)
<br>

Custom variables are a very powerful tool that can be defined within the Library of the Campaign Builder whose main uses are for example:
- capture data from a webpage to auto-fill a data collection form
[➡ Read about the "Data capture variables" in our documentation](doc:vcb-data-collection#section--automatic-filling-)
- set Proactive rules
[➡ Read about the "Proactive rules" in our documentation](doc:vcb-web-engagement-widgets#section--proactive-rules-)
- configure engagement widgets responding to events that can occur in a webpage.
[➡ Read about the "Event handlers" in our documentation](doc:vcb-event-handlers)
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2a30269-cv-list.png",
        "cv-list.png",
        1436,
        823,
        "#c8c8c8"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
To add a new custom variable or edit an existing one click on the **Add new** button or on the corresponding variable shown in the list in order to open the variable configuration panel
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/1ef7637-cv-main-panel.png",
        "cv-main-panel.png",
        1097,
        691,
        "#faf9f9"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
#**Custom variable settings**
a new custom variable has few settings to define
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/89652b5-cv-config_panel_2.png",
        "cv-config_panel_2.png",
        1128,
        309,
        "#fafafa"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
##**Variable Identifier**
a name to identify the variable. 

##**Variable Data Type**
The data type it represents. The available types selectable from the drop-down list are **String**, **Number**, **Boolean** 

##**Variable Type**
It defines how the variable captures the data. There are three different ways:

- **Selector:**
a variable can be of type selector, so it means that its value is fetched from an object present in a webpage it is available. After selecting it you have to insert the name of this selector (i.e: #id, .class)
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/101936e-cv-config_panel-3.png",
        "cv-config_panel-3.png",
        1121,
        338,
        "#f8f8f8"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
- **Javascript**
the type javascript allows to assign a value to a custom variable, calculated based on an implemented logic and executed from the browser. The code can be typed directly inline into the console that opens when you select the javascript type.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/defd298-cv-javascript-2.png",
        "cv-javascript-2.png",
        1058,
        514,
        "#b3b3b3"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
- **Web Service**
The value of a custom variable can be also returned from an external web service whose url must be provided
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/99cfcbe-cv-javascript-2.png",
        "cv-javascript-2.png",
        1058,
        514,
        "#b3b3b3"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
##**Value replacement**
The value in a custom variable can be replaced if it match a defined pattern by a provided regular expression, whether by specifying a replacement value that also support the regular expression variables.

You can check if you want remove the whitespace at the beginning and at the end of the result.

Depending of the type of data that is stored into the custom variable you can decide if you want to cache the value, if for example it remains always the same, if instead it must never be cached or if you want keep it for an interval of seconds that can be defined
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/48cbbb6-cv-replacement.png",
        "cv-replacement.png",
        1046,
        396,
        "#faf9f9"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]