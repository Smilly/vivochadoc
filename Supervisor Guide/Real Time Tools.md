---
title: "Real Time Tools"
excerpt: ""
---
The Real Time Monitoring area is growing up with new features which allow supervisor to have a full control of what happens in his agents’ team. Indeed the Real Time Tools have been enhanced with the Silent Monitoring, so now the dashboard consists of three sections.

* [Website Insight](#section-website-insight)
* [Agents Activity](#section-agents-activity)
* [Silent Monitor](#section-silent-monitor)

##Website Insight

The Website Insight is a dashboard that contains a chart selector and a table that shows some metrics related to the selected charts.

The available charts are:

* [Contacts Trend](#section-contacts-trend)
* [Visitors and Widgets](#section-visitors-and-widgets)
* [Widgets and Contacts](#section-widgets-and-contacts)
* [Widgets related to visits](#section-widgets-related-to-visits)
* [Contacts related to widgets](#section-contacts-related-to-widgets)

###Contacts Trend
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/afbe8e2-Website_insight.001.png",
        "Website insight.001.png",
        1280,
        720,
        "#e8e9ea"
      ],
      "sizing": "full",
      "border": true
    }
  ]
}
[/block]
This chart is made by four series: 

* In progress - the trend of the contacts
* Manageable - the trend of how many contacts could be managed
* Waiting - the trend of the waiting contacts
* Potentials - the trend of the contacts prediction based on the visitors

When this chart is selected the table below the charts contains:

* Pages - the list of the top ten page
* Current - the active contacts on the related page

###Visitors and Widgets

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/a3cc70c-visitors_and_widgets.png",
        "visitors and widgets.png",
        793,
        271,
        "#7f7b7a"
      ],
      "border": true
    }
  ]
}
[/block]
This chart is made by two series: 

* Visitors - the trend of the visitors
* Widgets - the trend of the shown widgets

When this chart is selected the table below the charts contains:

* Pages - the list of the top ten page
* Visitors - the number of visitors on the page
* Widgets - the number of widgets on the page

###Widgets and Contacts

This chart is made by two series: 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/d4c2659-widgets_and_contacts.png",
        "widgets and contacts.png",
        794,
        277,
        "#7d7c78"
      ],
      "border": true
    }
  ]
}
[/block]
* Widgets - the trend of the shown widgets
* Contacts - the trend of the active contacts

When this chart is selected the table below the charts contains:

* Pages - the list of the top ten page
* Widgets - the number of widgets on the page
* Contacts - the number of contacts for the page

###Widgets related to visits
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/d67cc5f-widgets.png",
        "widgets.png",
        791,
        275,
        "#7f7b7a"
      ],
      "border": true
    }
  ]
}
[/block]
This chart is made by one serie: 

* Widgets - the trend of the widgets related to the visitors

When this chart is selected the table below the charts contains:

* % Widgets - the number of widgets related to the number of visitors


### Contacts related to widgets
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2712ade-contacts.png",
        "contacts.png",
        795,
        278,
        "#7b7d78"
      ],
      "border": true
    }
  ]
}
[/block]
This chart is made by one serie: 

* Contacts - the trend of assigned contacts

When this chart is selected the table below the charts contains:

* % Contacts - the contacts related to the shown widgets (engagement rate)

[block:callout]
{
  "type": "info",
  "body": "Part of the Real Time Tools are available also to the agents, so they are able to monitor their personal performance. See the corresponding doc in the Agent Guide at this link: **[Agent Real Time Tools](doc:agent-real-time-tools)**",
  "title": "Info"
}
[/block]
##Agents Activity

This section is used to monitor the agents activity and the daily trends, it is updated every 20 seconds and it is made by five widgets:

* [Contacts](#section-contacts)
* [Contacts of the day](#section-contacts-of-the-day)
* [Agent load](#section-agent-load)
* [Agent status](#section-agent-status)
* [Agents list](#section-agent-list)
* [Agent Details](#section-agent-details)
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/3c43f0d-Agents_activity.001.png",
        "Agents activity.001.png",
        1280,
        720,
        "#eae9e9"
      ],
      "sizing": "full",
      "border": true
    }
  ]
}
[/block]
###Contacts
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/a272e03-contacts.png",
        "contacts.png",
        345,
        252,
        "#7c7d7c"
      ],
      "border": true
    }
  ]
}
[/block]
This widget shows the following metrics:

* **In progress** - the assigned contacts
* **idle** - the number of assigned contacts with idle state
* **waiting** - the number of contacts that are in the agents' pending queue
* **manageable** - it is the sum of the contacts that your agents can currently manage. This is calculated taking into account the chat limit for each agent, if this is set, or alternatively the maximum throughput, which is the expected maximum number of contacts that an agent manages to sustain according the latest activities. 
* **expected** -  the algorithm that elaborates this info considers the **average engagement rate**, calculated during the last 10 minutes, and the number of widgets that are shown to visitors: it gives an estimation on the contacts that could be requested to the agents, based on the trend of activities in the website.
* **potential** - it is simply the multiplication of the average engagement rate in recent times by the current number of visitors. That is, the number of expected contacts if a widget was being shown to every visitor of the site
[block:callout]
{
  "type": "info",
  "body": "the **engagement rate** represents the ratio between the number of widgets that are shown to visitors in the website and the number of the requested contacts. it indicates how many of these widgets shown are turned into a contact request by a visitor that engages an agent."
}
[/block]
###Contacts of the day

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/6130f81-jAM0nl7iRIafYQYFyPFB_Schermata_2016-06-22_alle_11.33.55.png",
        "jAM0nl7iRIafYQYFyPFB_Schermata 2016-06-22 alle 11.33.55.png",
        352,
        216,
        "#f2e6e6"
      ]
    }
  ]
}
[/block]
This widget shows the contacts **trend of the day**, with a pie chart for the successful and failed contacts.

The bottom metrics are related to the different reasons of the failed contacts:

* **dissuaded** - when the contacts are rejected because the expiration of the dissuasion time
* **abandoned** - when the user abandon the contact in a period that goes from 10 seconds to the dissuasion time
* **cancelled** - when user has abandoned the contact before 10 seconds
* **no interaction** - when in a contacts there are no more than 3 messages (and at least one sent for each counterpart)
* **other** - the contact is failed for non detectable reasons (es: pc power off, browser closed without contact abandon)

[➡ Read more about the "contacts outcomes " in our documentation](https://docs.vivocha.com/docs/contacts-report#section-the-possible-outcomes-of-the-contacts-are-)

###Agent load
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/33a21ad-8Vuu3jHXSnisPPYILYGO_Schermata_2016-06-22_alle_11.33.00.png",
        "8Vuu3jHXSnisPPYILYGO_Schermata 2016-06-22 alle 11.33.00.png",
        448,
        187,
        "#d4d4d4"
      ]
    }
  ]
}
[/block]
This widget shows the load level for the agents and the suggestions of how much agents should be used to reach the manageable level of contacts.

###Agent status
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/cb97668-13zGGnxFQhmVMQdaHIXD_Schermata_2016-06-22_alle_11.32.11.png",
        "13zGGnxFQhmVMQdaHIXD_Schermata 2016-06-22 alle 11.32.11.png",
        354,
        191,
        "#7c7e7c"
      ]
    }
  ]
}
[/block]
This widget shows how many agents are currently online an how many agents are in pause mode.

###Agents list

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/ae602b4-Screen_Shot_2017-01-26_at_17.52.05.png",
        "Screen Shot 2017-01-26 at 17.52.05.png",
        1040,
        719,
        "#e5e5e5"
      ]
    }
  ]
}
[/block]
The table of agents lists all the agents that has a login for the current day. For each agents the following information are displayed:

* Agent - the nickname of the agent (if not set it shows firstname and lastname or the agent id)
* In progress - the number of contacts that are assigned to that agent
* Load - the level of load for the agent
* Successful - the successful contacts of the day for the agent
* Waiting - the average answer time for the agent
* Active media - the current status of the media for the agent

###Agent Details
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/8dabd0c-47BCrsSQ8eMEYjdfM9Ag_Schermata_2016-06-22_alle_11.16.51.png",
        "47BCrsSQ8eMEYjdfM9Ag_Schermata 2016-06-22 alle 11.16.51.png",
        799,
        199,
        "#5d7d8b"
      ]
    }
  ]
}
[/block]
The row of the agents list are expandable, an agent details card will appear by clicking the arrow down icon.

The agent card shows the following data:

* **Contacts by hour** - a column chart that shows the trending successful contacts by last 5 hours slots
* **Successful** - the successful contacts of the day
* **Used media** - which media and how many times this media has been used in all the contacts of the day that a user has managed 
* **Working time** - the time that an agent spent in working or paused mode
* **Average** - the average answer time and the average interaction time

##Silent Monitor
This section opens showing the list of the contacts in progress, when present, reporting some summary info about each of them:

- name of the Agent
- name of the customer, if available
- Data Collection
- Media used
- duration 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/13c84a4-Screen_Shot_2017-02-21_at_14.53.02.png",
        "Screen Shot 2017-02-21 at 14.53.02.png",
        1437,
        616,
        "#e9e9e9"
      ],
      "sizing": "full",
      "border": true
    }
  ]
}
[/block]
A supervisor can now monitor how each of these contacts is being handled by the agents of his group. he can access to information about the customer, notes, data collection and, of course, the conversation between customer and agent and for a more consistent experience, the Silent Monitor has the same new interface of a contact transcript that you can find in the report area
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/4619c0c-silent_monitor.png",
        "silent_monitor.png",
        1021,
        576,
        "#6a7275"
      ],
      "sizing": "full"
    }
  ]
}
[/block]