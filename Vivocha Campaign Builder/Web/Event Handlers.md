---
title: "Event Handlers"
excerpt: ""
---
[block:callout]
{
  "type": "warning",
  "body": "Event handlers are configurable on different levels in a hierarchical way: you can set them directly in the Channel to have it working in all the available entry points, or you can define them into a single engagement widget"
}
[/block]
Besides a brand new Proactive Engine that takes advantage of a rich set of built-in data capture variables and custom data variables, the personalization of a Campaign with all its channels, entry points and widgets can be achieved also thanks the further powerful tool od the Custom Events Handlers.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/0ffb043-WEB-Events_handlers_4.png",
        "WEB-Events handlers 4.png",
        897,
        466,
        "#f7f7f7"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
An Event Handler runs your custom JavaScript code when specific event occurs.

So you can select one event among the available in the dropdown list, related with the webpage loading or with the status of the engagement widget or the contact, and configure it by hooking pieces of code which for example can execute specific actions like for example the evaluating of data and the its storage in a custom variable.

You can insert the javascript custom code directly in a editor by selecting the handler type **inline**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2419f63-WEB-Events_Handlers_6.png",
        "WEB-Events Handlers 6.png",
        836,
        550,
        "#bababa"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
or to make a call to an external code by specifying the corresponding web service endpoint URL.

It is also possible to specify if the code must be run every time that event occurs or only at the first time, and whether it is run asynchronously or not.

To remove an Event Handler click on the corresponding **Remove** button.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/766b89d-WEB-Events_Handlers_8.png",
        "WEB-Events Handlers 8.png",
        836,
        491,
        "#f6f6f6"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]