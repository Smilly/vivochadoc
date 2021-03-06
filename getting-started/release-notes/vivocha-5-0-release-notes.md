---
title: Vivocha 5.0 Release Notes
excerpt: ''
---

# Vivocha 5-0 Release Notes

_Summary_

* [Real time tools improvement](vivocha-5-0-release-notes.md#section-real-time-tools-improvement)
* [Browser sync](vivocha-5-0-release-notes.md#section-browser-sync)
* [Enhancements to the transfer functionality](vivocha-5-0-release-notes.md#section-enhancements-to-the-transfer-functionality)
* [Rest API v2](vivocha-5-0-release-notes.md#section-rest-api-v2)
* [JavaScript Reference API documentation](vivocha-5-0-release-notes.md#section-javascript-reference-api-documentation)

## Real time tools improvement

New data will allow you to know the potential of your team and your web site.

### Contacts

Discover how many contacts:

* your team is really able to manage;
* are expected, based on the average engagement rate;
* you are potentially able to manage, if all your customer could see the widget.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/a99adc9-5012959-1.png",
    "5012959-1.png",
    1730,
    891,
    "#3a3a3a"
  ]
  ```

    }

  \]

  }

  \[/block\]

  **Agents activity**

Discover:

* % of agent loading;
* n. of agent really required to manage all the contacts waited, based on the average engagement rate.

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/13c2428-22545a5-2.png](https://files.readme.io/13c2428-22545a5-2.png)", "22545a5-2.png", 1730, 891, "\#3a3a3a" \] } \] } \[/block\]

### Agents list

Details of agents list:

* a circle shows if the agent is online or if he is paused;
* n. of contacts he is managing;
* % of loading;
* n. of current day successes;
* average waiting time for take a contact;
* active media and number of contacts managed for each media;
* you have the chance to filter contacts using the defined parameters. 

  \[block:image\]

  {

  "images": \[

  {

    "image": \[

  ```text
  "https://files.readme.io/e33e3db-99f318e-3.png",
  "99f318e-3.png",
  1730,
  891,
  "#383838"
  ```

    \]

  }

  \]

  }

  \[/block\]

  **Agents performance**

Agent performance details:

* n. of contacts managed for each time slot;
* online time and paused time;
* n. of times each media has been used during the day;
* average waiting time for take a contact.

  \[block:image\]

  {

  "images": \[

  {

    "image": \[

  ```text
  "https://files.readme.io/aa0247c-299b958-4.png",
  "299b958-4.png",
  1730,
  891,
  "#3a3b3c"
  ```

    \]

  }

  \]

  }

  \[/block\]

  **Website insight**

Added a chart with information about potential, expected and manageable contacts:

* based on the number of current agents;
* based on website traffic.

  \[block:image\]

  {

  "images": \[

  {

    "image": \[

  ```text
  "https://files.readme.io/a5af716-412f181-website_insight.png",
  "412f181-website_insight.png",
  725,
  373,
  "#e6e8ea"
  ```

    \]

  }

  \]

  }

  \[/block\]

\[block:callout\] { "type": "info", "title": "For more details please read", "body": "[Reatime Tools](doc:realtime-tools)" } \[/block\]

## Browser sync

### SCENARIO

* An agent is on a phone call with a customer and cannot see what is really happening on the customer’s browser to give a proper support
* The browser sync allows the agents to use the sharing channel, to monitor and provide online support, to the customers who didn’t start the contact from Vivocha, or started it from a different media like a phone call

#### Two ways of engagement:

Start a new contact form scratch from a third party phone call. Add sharing to an existing Vivocha contact \(twilio call\) The agent has just to share the session pin, generated by the system, with the customer and ask to insert it in the browser. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/1675588-bc8970b-Screen\_Shot\_2016-07-19\_at\_11.38.23\_AM.png](https://files.readme.io/1675588-bc8970b-Screen_Shot_2016-07-19_at_11.38.23_AM.png)", "bc8970b-Screen\_Shot\_2016-07-19\_at\_11.38.23\_AM.png", 500, 586, "\#5690b4" \] } \] } \[/block\]

#### Quick start integration

The customer has just to paste the pin code in the address bar at the end of the page URL No further development job is required \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/f693a91-4ffa048-browser\_sync.png](https://files.readme.io/f693a91-4ffa048-browser_sync.png)", "4ffa048-browser\_sync.png", 780, 569, "\#dcdfe1" \] } \] } \[/block\] Browser sync is an API: \[block:code\] { "codes": \[ { "code": "vivocha.syncContact\(‘459942’, function\(err, contact\) { if \(err\) console.error\(err\);\n else showTools\(\); }\);", "language": "javascript" } \] } \[/block\] You can build your own customisation to show a box that ask to the customer to insert the code given by the agent and agree to start the sharing session. You can also add sharing tools that allow the customer to manage and end the sharing session whenever he wants. You can find a sample with this integration scenario on our documentation. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/a96809e-d2f0846-browser\_sync2.png](https://files.readme.io/a96809e-d2f0846-browser_sync2.png)", "d2f0846-browser\_sync2.png", 780, 569, "\#dadcde" \] } \] } \[/block\]

\[block:callout\] { "type": "info", "body": "[Browser Sync Widget](doc:browser-sync-widget)", "title": "For more details please read" } \[/block\]

## Enhancements to the transfer functionality

### What’s new

* Added Transfer groups to simplify the identification of a set of services/tags that describe the skills needed by the transfer recipients
* Configurable Transfer priority for groups
* Service/Groups availability and Agents status in the Transfer Console App
* Configurable Transfer bounce back \(fallback in case of busy agents\)
* Configurable Transfer to busy agents

### Transfer groups

Related tags can now be grouped together under a

A new configuration module allows the creation of transfer groups

A transfer group is a set of tags and a priority value \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/ec8d684-c274892-transfer\_groups.png](https://files.readme.io/ec8d684-c274892-transfer_groups.png)", "c274892-transfer\_groups.png", 775, 425, "\#e2e2e2" \] } \] } \[/block\] Tag groups are described by:

* name
* tag list
* priority

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/956a1e5-e640a34-transfer\_groups2.png](https://files.readme.io/956a1e5-e640a34-transfer_groups2.png)", "e640a34-transfer\_groups2.png", 775, 425, "\#e2e2e2" \] } \] } \[/block\]

### Transfer Console App

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/15285d6-43f776a-transfer\_groups3.png](https://files.readme.io/15285d6-43f776a-transfer_groups3.png)", "43f776a-transfer\_groups3.png", 775, 425, "\#ebebeb" \] } \] } \[/block\]

\[block:callout\] { "type": "info", "title": "For more details please read", "body": "[Transfer Groups](doc:transfer-groups)" } \[/block\]

## Rest API v2

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/eb972fa-5720bdb-rest-api.png](https://files.readme.io/eb972fa-5720bdb-rest-api.png)", "5720bdb-rest-api.png", 586, 407, "\#eaecea" \] } \] } \[/block\]

\[block:callout\] { "type": "info", "title": "For more details please read", "body": "[Vivocha REST API v2](doc:vivocha-rest-api-v2)" } \[/block\]

## JavaScript Reference API documentation

* Revision of the documentation and porting to a new platform to simplify the access for the end users and easily keep track of the version changes. 
* API and libraries with richest documentation, thought for a easier use by developers.
* New REST API, compliant with Swagger 2.0 \(OpenAPI Specification\) with OAuth 2 authentication.

  \[block:callout\]

  {

  "type": "info",

  "body": "[Vivocha Javascript SDKs](doc:vivocha-sdks)"

  }

  \[/block\]

