---
title: "Network Connection Problems"
excerpt: ""
---
Network connection problems can occur both to the agent when he uses the vivocha console than the visitor of the website when he requests a contact.

When such problems occur, they can drop the active contacts if the offline status lasts for too much time.

Depending on what occurred and the events registered by the system, some different error messages are displayed into the console telling where the problem took place.

##**Red Triangle - agent side network problem**
The triangle with the exclamation mark in red background point out that the agent console is not able to connect correctly to the vivocha servers.

Messages so marked result “unsent”, that is that they are never received from our servers.

If the network problem persists for more than some seconds and the agent console is not able to correctly contact the Vivocha servers, agent will see the "disconnected" status and a message that notify that he is offline

This is typically due to a problem in the internal network, therefore it requires that a technical team to do a complete network and equipment check
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/ffda799-Screen_Shot_2017-04-07_at_11.54.58.png",
        "Screen Shot 2017-04-07 at 11.54.58.png",
        431,
        547,
        "#efe5e2"
      ],
      "border": true
    }
  ]
}
[/block]
##**Yellow triangle - visitor/customer side network problem**
when the customer has network connection issues, the agent can send messages correctly to the Vivocha servers but these are not received by the customer. In this case during a chat and near the agent messages, a clock icon will appear which turn into a triangle with yellow background and an exclamation mark (<span style="color:#fc7"> :fa-exclamation-triangle: </span>), to indicate that the messages were not delivered correctly to the customer. 

Possible cause of this problem can be:
* The customer have a network problem;
* The customer is changing the page (page refresh);
* The customer closed the browser;

In this case when the clock icon appears the unsent messages are however received and stored from our servers and, If contact is still on going, as soon as the customer side network problem go away, these messages received and stored in the servers are sent to the customer and the triangle icon disappear.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/3c8f314-Screen_Shot_2017-04-06_at_17.04.13.png",
        "Screen Shot 2017-04-06 at 17.04.13.png",
        423,
        327,
        "#dee0da"
      ],
      "border": true
    }
  ]
}
[/block]
##**Sad face error - network problem or unexpected event**
Typically the sad face icon appears when the system is unable to establish the communication between the customer and the agent and the requested contact is not initialized and does not start.

Possible cause of this problem can be:
* the customer closed the contact after the agent already picked up it.
* customer is experiencing network problems preventing him to connect to the agent;
* agent is experiencing network problems preventing him to connect to the customer;
etc, …

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/1dfc092-Screen_Shot_2018-06-05_at_10.35.38.png",
        "Screen Shot 2018-06-05 at 10.35.38.png",
        422,
        226,
        "#f1efee"
      ],
      "border": true
    }
  ]
}
[/block]
##**Diagnostic and Browser Developer Tools**
All these network events are handled by the platform that acts providing useful clues that help to give an idea of where the problem might reside.

To try to identify the cause, it might be helpful to analyze what messages are logged within the browser and take advantage of a whole range of Dev Tools.

Modern browsers like Chrome and Firefox provide a set of tools that allow developers and testers to debug of the javascript interaction on the pages. 
Very useful are in particular:
* **Console Panel:** displays any javascript errors or warnings and let you execute a collection of functions for performing common debugging tasks.
* **Network Panel:** shows the loading times for each resource on the page (style sheets, javascript files, images, ...), providing also a valid tool to check performances.

###**Chrome Developer Tools**
* Select More Tools > Developer Tools from Chrome's Main Menu.
* Right-click a page element and select Inspect.
* Press Command+Option+I (Mac) or Control+Shift+I (Windows, Linux).
* More info at: https://developers.google.com/web/tools/chrome-devtools/ 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/a7208cf-Screen_Shot_2018-06-05_at_10.50.35.png",
        "Screen Shot 2018-06-05 at 10.50.35.png",
        953,
        779,
        "#cee2e5"
      ],
      "sizing": "80"
    }
  ]
}
[/block]
###**Firefox Developer tools**
* Select  Developer from Firefox Main Menu, then Toggle Tools option
* Right-click a page element and select Inspect.
* Press Command+Option+I (Mac) or Control+Shift+I (Windows, Linux).
* More info at: https://developer.mozilla.org/en-US/docs/Tools 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/5fb790f-Screen_Shot_2018-06-05_at_10.50.54.png",
        "Screen Shot 2018-06-05 at 10.50.54.png",
        962,
        790,
        "#c4dce0"
      ],
      "sizing": "80"
    }
  ]
}
[/block]
###**How to take a screenshot of the problem**
The information obtained from the web console of the browser show which are the errors raised in the execution of the javascript code and provide useful elements to try to recreate the problem.

To accomplish this result, you should carry out tests on another account in the same world figuring out the steps that raised those errors.

Messages and data displayed in the browser console or in network panel have to be provided if required when you escalate the issue to the 2nd level of support.

It worth to point out that all these info must be readable in the screenshots that will be provided, so they can actually represent a helpful starting point to go deep in further inspections

It’s important that every captured screenshot from the Vivocha console contains as much information as possible .This allows to better analyze the behaviour occurred.

* **Date and time** are essential info.
* customer's name, when available, and also the agent's one, along with messages sent can permit to identity the contact in a more easy way.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/14b6f9e-Screen_Shot_2018-06-05_at_10.51.09.png",
        "Screen Shot 2018-06-05 at 10.51.09.png",
        966,
        557,
        "#d1dcde"
      ],
      "sizing": "80"
    }
  ]
}
[/block]